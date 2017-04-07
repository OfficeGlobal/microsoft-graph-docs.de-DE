# <a name="user-findmeetingtimes"></a>user: findMeetingTimes
Mit dieser Methode können Sie Vorschläge für Besprechungstermine abrufen. Die Vorschläge basieren auf der Verfügbarkeit des Organisators und der Teilnehmer sowie auf als Parameter spezifizierten Zeit- oder Ortseinschränkungen.

Wenn **findMeetingTimes** keine Besprechungsvorschläge zurückgeben kann, enthält die Antwort einen Grund, angegeben in der Eigenschaft **emptySuggestionsReason**. Ausgehend von diesem Wert können Sie die Parameter optimieren und **findMeetingTimes** erneut aufrufen.

**Hinweis**

Aktuell geht **findMeetingTimes** von folgenden Voraussetzungen aus:

- Jeder [Teilnehmer](../resources/attendee.md), bei dem es sich um eine Person handelt (nicht um eine Ressource), ist ein erforderlicher Teilnehmer. Geben Sie also für Personen `required` und für Ressourcen `resource` in der entsprechenden Eigenschaft **type** an. Diese Eigenschaft gehört zum Sammlungsparameter **attendees**.
- Alle Besprechungsvorschläge liegen innerhalb der Arbeitszeiten des Organisators oder der Teilnehmer. Die Eigenschaft **activityDomain** von Ressourcen des Typs [timeConstraint](../resources/timeConstraint.md) muss nicht angegeben werden. 


## <a name="prerequisites"></a>Voraussetzungen
Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Calendars.Read.Shared* oder *Calendars.ReadWrite.Shared*.
## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /me/findMeetingTimes
POST /users/{id|userPrincipalName}/findMeetingTimes
```
## <a name="request-headers"></a>Anforderungsheader
| Name       | Wert|
|:---------------|:----------|
| Authorization  | Bearer <code>|
| Prefer: outlook.timezone | Eine Zeichenfolge, die eine bestimmte Zeitzone für die Antwort festlegt, beispielsweise „Pacific Standard Time“ |


## <a name="request-body"></a>Anforderungstext
In der Tabelle unten sind alle unterstützten Parameter aufgeführt. Geben Sie abhängig von Ihrem jeweiligen Szenario für jeden notwendigen Parameter ein JSON-Objekt im Anforderungstext an. Ausgehend von den angegebenen Parametern überprüft **findMeetingTimes** den Frei-/Gebucht-Status im Hauptkalender des Organisators und in den Hauptkalendern der Teilnehmer. Die Aktion berechnet die bestmöglichen Besprechungstermine und gibt Besprechungsvorschläge zurück.


| Parameter       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|attendees|[attendeeBase](../resources/attendeebase.md) collection|Eine Sammlung von Teilnehmern oder Ressourcen für die Besprechung. Ist diese Sammlung leer, sucht **findMeetingTimes** nur für den Organisator nach freien Zeitfenstern.|
|locationConstraint|[locationConstraint](../resources/locationconstraint.md)|Die Anforderungen des Organisators bezüglich des Besprechungsorts, z. B. ob ein Vorschlag für einen Besprechungsort erforderlich ist oder nur bestimmte Besprechungsorte zulässig sind|
|timeConstraint|[timeConstraint](../resources/timeconstraint.md)|Die Start- und Endzeit des Zeitbereichs, in dem die Besprechung stattfinden soll. In den Eigenschaften **start** und **end** dieses Parameters können Sie eine Zeitzone festlegen. Diese Zeitzone gilt jedoch ausschließlich für den Parameter **timeConstraint**; alle eventuell in der Antwort zurückgegebenen Zeitwerte werden weiterhin standardmäßig als UTC angezeigt. Sie können mithilfe des Anforderungsheaders `Prefer: outlook.timezone` eine spezifische Zeitzone für die Zeitwerte in der Antwort festlegen. |
|meetingDuration|Edm.Duration|Die Dauer der Besprechung im Format [ISO8601](http://www.iso.org/iso/iso8601). 1 Stunde wird beispielsweise als „PT1H“ angegeben. Dabei ist „P“ der Bezeichner für die Dauer, „T“ der Bezeichner für die Zeit und „H“ der Bezeichner für die Zeiteinheit Stunde. Wenn keine Besprechungsdauer angegeben wird, verwendet **findMeetingTimes** den Standardwert von 30 Minuten. |
|maxCandidates|Edm.Int32|Die maximale Anzahl an zurückgegebenen Besprechungsterminvorschlägen|
|isOrganizerOptional|Edm.Boolean|`True`, wenn die Anwesenheit des Organisators nicht erforderlich ist, ansonsten `false`|
|returnSuggestionReasons|Edm.Boolean|`True`, wenn für jeden Besprechungsvorschlag ein Grund in der Eigenschaft **suggestionReason** zurückgegeben werden soll. Der Standardwert ist `false`, damit diese Eigenschaft nicht zurückgegeben wird.|
|minimumAttendeePercentage|Edm.Double| Die mindestens erforderliche [Konfidenz](#the-confidence-of-a-meeting-suggestion), damit ein bestimmtes Zeitfenster in der Antwort zurückgegeben wird. Hierbei handelt es sich um einen Prozentwert zwischen 0 und 100. |

## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200, OK` und eine Ressource des Typs [meetingTimeSuggestionsResult](../resources/meetingTimeSuggestionsResult.md) im Antworttext zurück. 

Eine Ressource des Typs **meetingTimeSuggestionsResult** enthält eine Sammlung von Besprechungsvorschlägen und eine Eigenschaft **emptySuggestionsReason**. Jeder Vorschlag ist als eine Ressource des Typs [meetingTimeSuggestion](../resources/meetingTimeSuggestion.md) definiert, für die die durchschnittliche Teilnahmekonfidenz der Teilnehmer bei 50 % oder einem spezifischen Prozentwert liegt, den Sie im Parameter **minimumAttendeePercentage** festgelegt haben. 

Standardmäßig wird jeder Besprechungsterminvorschlag in UTC zurückgegeben. 

### <a name="the-confidence-of-a-meeting-suggestion"></a>Die Konfidenz von Besprechungsvorschlägen

Die Eigenschaft **confidence** einer Ressource des Typs **meetingTimeSuggestion** liegt in einem Bereich von 0 % bis 100 %. Sie gibt an, wie wahrscheinlich es ist, dass alle Teilnehmer an der Besprechung teilnehmen können, und basiert auf den Frei-/Gebucht-Status der einzelnen Teilnehmer:

- Für jeden Teilnehmer gilt: Ist der Status für eine Besprechung „Frei“, liegt die Teilnahmewahrscheinlichkeit bei 100 %. Beim Status „Unbekannt“ liegt sie bei 49 %, beim Status „Gebucht“ bei 0 %.
- Zur Berechnung der Konfidenz eines Besprechungsterminvorschlags wird der Mittelwert aus den individuellen Teilnahmewahrscheinlichkeiten aller Besprechungsteilnehmer für die betreffende Besprechung gebildet.
- Gibt es mehrere Besprechungsterminvorschläge, ordnet die Aktion **findMeetingTimes** die Vorschläge zunächst nach ihrem berechneten Konfidenzwert, beginnend mit dem Vorschlag mit dem höchsten Wert. Haben mehrere Vorschläge jeweils denselben Konfidenzwert, ordnet die Aktion diese Vorschläge chronologisch.
- Mithilfe des optionalen Parameters **minimumAttendeePercentage** für **findMeetingTimes** können Sie festlegen, dass nur Besprechungsterminvorschläge mit einem bestimmten Mindestkonfidenzwert zurückgegeben werden. Beispielsweise können Sie eine **minimumAttendeePercentage** von 80 % festlegen, wenn Sie nur Vorschläge erhalten möchten, bei denen die Wahrscheinlichkeit, dass alle Teilnehmer teilnehmen können, bei mindestens 80 % liegt. Wenn Sie keine **minimumAttendeePercentage** festlegen, setzt **findMeetingTimes** einen Wert von 50 % an.

Hier ein Beispiel für einen Besprechungsterminvorschlag für 3 Teilnehmer mit den folgenden Frei-/Gebucht-Status:

|**Teilnehmer**|**Frei-/Gebucht-Status**|**Teilnahmewahrscheinlichkeit in %**|
|:-----|:-----|:-----|
|Dana | Frei | 100 % |
|John | Unbekannt | 49 % |
|Fanny | Gebucht | 0 % |

Die Konfidenz des Besprechungsterminvorschlags (durchschnittliche Teilnahmewahrscheinlichkeit) liegt hier bei (100 % + 49 % + 0 %) ÷ 3 = 49,66 %.

Wenn Sie eine **minimumAttendeePercentage** von 80 % in einer Operation des Typs **findMeetingTimes** festlegen, wird die Operation diesen Termin nicht in der Antwort vorschlagen, da 49,66 % < 80 % ist.

## <a name="example"></a>Beispiel

Das folgende Beispiel veranschaulicht, wie Sie einen Besprechungstermin für einen vorab festgelegten Ort finden und für jeden Vorschlag einen Grund anfragen. Dazu geben Sie im Anforderungstext folgende Parameter an:

- **attendees**
- **locationConstraint**
- **timeConstraint**
- **meetingDuration**
- **returnSuggestionReasons**
- **minimumAttendeePercentage**

Durch Setzen des Parameters **returnSuggestionReasons** wird für jeden Vorschlag auch eine Erklärung in der Eigenschaft **suggestionReason** vermerkt, sofern **findMeetingTimes** Vorschläge zurückgibt.

Beachten Sie: In der Anforderung gilt für die Zeit die Zeitzone PST. Die Antwort gibt Besprechungsterminvorschläge jedoch standardmäßig in UTC zurück. Sie können den Anforderungsheader `Prefer: outlook.timezone` verwenden, um auch für die Zeitwerte in der Antwort die Zeitzone PST festzulegen.

##### <a name="request"></a>Anforderung
Hier sehen Sie die Beispielanforderung:
<!-- {
  "blockType": "request",
  "name": "user_findmeetingtimes"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/findMeetingTimes
Content-type: application/json

{ 
  "attendees": [ 
    { 
      "type": "required",  
      "emailAddress": { 
        "name": "Fanny Downs",
        "address": "fannyd@a830edad905084922E16072013.onmicrosoft.com" 
      } 
    },
    { 
      "type": "optional",  
      "emailAddress": { 
        "name": "Dana Swope",
        "address": "danas@a830edad905084922E16072013.onmicrosoft.com" 
      } 
    } 
  ],  
  "locationConstraint": { 
    "isRequired": "false",  
    "suggestLocation": "false",  
    "locations": [ 
      { 
        "resolveAvailability": "false",
        "displayName": "Conf room Hood" 
      } 
    ] 
  },  
  "timeConstraint": { 
    "timeslots": [ 
      { 
        "start": { 
          "dateTime": "2016-10-20T07:00:00",  
          "timeZone": "Pacific Standard Time" 
        },  
        "end": { 
          "dateTime": "2016-10-20T17:00:00",  
          "timeZone": "Pacific Standard Time" 
        } 
      } 
    ] 
  },  
  "meetingDuration": "PT2H",
  "returnSuggestionReasons": "true",
  "minimumAttendeePercentage": "60"
}
```

##### <a name="response"></a>Antwort
Unten sehen Sie eine Beispielantwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json


{
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.meetingTimeSuggestionsResult",
   "meetingTimeSuggestions":[
      {
         "meetingTimeSlot":{
            "start":{
               "dateTime":"2016-10-20T15:00:00.0000000",
               "timeZone":"UTC"
            },
            "end":{
               "dateTime":"2016-10-20T17:00:00.0000000",
               "timeZone":"UTC"
            }
         },
         "confidence":100,
         "organizerAvailability":"free",
         "attendeeAvailability":[
            {
               "attendee":{
                  "type":"required",
                  "emailAddress":{
                    "name": "Fanny Downs",
                    "address": "fannyd@a830edad905084922E16072013.onmicrosoft.com" 
                  }
               },
               "availability":"free"
            },
            {
               "attendee":{
                  "type":"required",
                  "emailAddress":{
                    "name": "Dana Swope",
                    "address": "danas@a830edad905084922E16072013.onmicrosoft.com" 
                  }
               },
               "availability":"free"
            }
         ],
         "locations":[
            {
               "displayName":"Conf room Hood"
            }
         ],
         "suggestionReason":"Suggested because it is one of the nearest times when all attendees are available."
      },
      {
         "meetingTimeSlot":{
            "start":{
               "dateTime":"2016-10-20T17:00:00.0000000",
               "timeZone":"UTC"
            },
            "end":{
               "dateTime":"2016-10-20T19:00:00.0000000",
               "timeZone":"UTC"
            }
         },
         "confidence":100,
         "organizerAvailability":"free",
         "attendeeAvailability":[
            {
               "attendee":{
                  "type":"required",
                  "emailAddress":{
                    "name": "Fanny Downs",
                    "address": "fannyd@a830edad905084922E16072013.onmicrosoft.com" 
                  }
               },
               "availability":"free"
            },
            {
               "attendee":{
                  "type":"required",
                  "emailAddress":{
                    "name": "Dana Swope",
                    "address": "danas@a830edad905084922E16072013.onmicrosoft.com" 
                  }
               },
               "availability":"unknown"
            }
         ],
         "locations":[
            {
               "displayName":"Conf room Hood"
            }
         ],
         "suggestionReason":"Suggested because it is one of the nearest times when all attendees are available."
      }
   ],
   "emptySuggestionsReason":""
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: findMeetingTimes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->