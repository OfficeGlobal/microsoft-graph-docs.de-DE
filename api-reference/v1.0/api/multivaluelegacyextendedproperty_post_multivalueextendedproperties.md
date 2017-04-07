# <a name="create-multi-value-extended-property"></a>Mehrwertige erweiterte Eigenschaft erstellen

In diesem Artikel erläutern wir Ihnen,wie Sie eine oder mehrere mehrwertige erweiterte Eigenschaften in einer neuen oder vorhandenen Instanz einer Ressource erstellen können. 

Die folgenden Benutzerressourcen werden unterstützt:

- [message](../resources/message.md)
- [mailFolder](../resources/mailfolder.md)
- [event](../resources/event.md)
- [calendar](../resources/calendar.md)
- [contact](../resources/contact.md)
- [contactFolder](../resources/contactfolder.md) 

Darüber hinaus werden die folgenden Gruppenressourcen unterstützt:

- [event](../resources/event.md)-Ressourcen für Gruppen
- [calendar](../resources/calendar.md)-Ressourcen für Gruppen
- [post](../resources/post.md)-Ressourcen für Gruppen 

Unter [Überblick über erweiterte Eigenschaften](../resources/extended-properties-overview.md) finden Sie weitere Informationen dazu, wann Datenerweiterungen oder erweiterte Eigenschaften verwendet werden sollten und wie erweiterte Eigenschaften angegeben werden.

## <a name="prerequisites"></a>Voraussetzungen

Zur Ausführung dieser API ist einer der folgenden **Bereiche** erforderlich (je nachdem, in welcher Ressource Sie die erweiterte Eigenschaft erstellen):

- _Mail.ReadWrite_
- _Calendars.ReadWrite_
- _Contacts.ReadWrite_
- _Group.ReadWrite.All_
 
## <a name="http-request"></a>HTTP-Anforderung
Sie können erweiterte Eigenschaften in einer neuen oder vorhandenen Ressourceninstanz erstellen.

Verwenden Sie zum Erstellen einer oder mehrerer erweiterter Eigenschaften in einer _neuen_ Ressourceninstanz die gleiche REST-Anforderung wie zum Erstellen der Instanz, und fügen Sie die Eigenschaften der neuen Ressourceninstanz _und die erweiterte Eigenschaft_ zum Anforderungstext hinzu. Beachten Sie, dass für einige Ressourcen die Erstellung auf mehrere Weisen erfolgen kann. Weitere Informationen zum Erstellen dieser Ressourceninstanzen finden Sie unter den entsprechenden Themen zum Erstellen einer [Nachricht](../resources/message.md), eines [MailFolder](../api/user_post_mailfolders.md)-Elements, [Ereignisses](../api/user_post_events.md), [Kalenders](../api/user_post_calendars.md), [Kontakts](../api/user_post_contacts.md), [contactFolder](../api/user_post_contactfolders.md)-Elements, [Gruppenereignisses](../api/group_post_events.md) und eines [Gruppenbeitrags](../resources/post.md). 
 
So sieht die Syntax der Anforderungen aus: 

<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages

POST /me/mailFolders
POST /users/{id|userPrincipalName}/mailFolders

POST /me/events
POST /users/{id|userPrincipalName}/events

POST /me/calendars
POST /users/{id|userPrincipalName}/calendars

POST /me/contacts
POST /users/{id|userPrincipalName}/contacts

POST /me/contactFolders
POST /users/{id|userPrincipalName}/contactFolders

POST /groups/{id}/events

POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
POST /groups/{id}/threads
POST /groups/{id}/conversations
```

Um eine oder mehrere erweiterte Eigenschaften in einer vorhandenen Ressourceninstanz zu erstellen,müssen Sie die Instanz in der Anforderung angeben und die erweiterte-Eigenschaft zum Anforderungstext hinzufügen.

**Hinweis:** Sie können keine erweiterte Eigenschaft in einem vorhandenen Gruppenbeitrag erstellen.

<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id|userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}

PATCH /me/mailFolders/{id}
PATCH /users/{id|userPrincipalName}/mailFolders/{id}

PATCH /me/events/{id}
PATCH /users/{id|userPrincipalName}/events/{id}

PATCH /me/calendars/{id}
PATCH /users/{id|userPrincipalName}/calendars/{id}

PATCH /me/contacts/{id}
PATCH /users/{id|userPrincipalName}/contacts/{id}

PATCH /me/contactFolders/{id}
PATCH /users/{id|userPrincipalName}/contactFolders/{id}

PATCH /groups/{id}/events/{id}
```


## <a name="parameters"></a>Parameter
|**Parameter**|**Typ**|**Beschreibung**|
|:-----|:-----|:-----|
|_URL parameters_|
|id|string|Eine eindeutige ID für ein Objekt in der entsprechenden Sammlung. Erforderlich.|
|_Body parameters_|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) collection| Ein Array aus einer oder mehreren mehrwertigen erweiterten Eigenschaften |
|id|String|Geben Sie diesen Parameter für jede Eigenschaft in der **multiValueExtendedProperties**-Sammlung an, um die Eigenschaft zu identifizieren. Der Parameter muss einem der unterstützten Formate entsprechen. Weitere Informationen finden Sie unter [Outlook extended properties overview](../resources/extended-properties-overview.md) (Überblick über erweiterte Outlook-Eigenschaften). Erforderlich.|
|value|string|Geben Sie für jede Eigenschaft in der **multiValueExtendedProperties**-Sammlung den Eigenschaftswert an. Erforderlich.|


## <a name="request-headers"></a>Anforderungsheader
| Name       | Wert |
|:---------------|:----------|
| Authorization | Bearer %token%|
| Content-Type | application/json |

## <a name="request-body"></a>Anforderungstext

Geben Sie einen JSON-Text für jedes [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md)-Objekt in der **multiValueExtendedProperties**-Sammlung der Ressourceninstanz an.

Beim Erstellen einer erweiterten Eigenschaft in einer _neuen_ Ressourceninstanz müssen Sie zusätzlich zu der neuen **multiValueExtendedProperties**-Sammlung eine JSON-Darstellung der betreffenden Ressourceninstanz angeben (d. h. eine Ressource des Typs [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md) usw.).

## <a name="response"></a>Antwort

#### <a name="response-code"></a>Antwortcode
Ist die Operation zur Erstellung einer erweiterten Eigenschaft in einer neuen Ressourceninstanz erfolgreich, wird `201 Created` zurückgegeben. Ausnahme: In einem neuen Gruppenbeitrag kann die Operation je nach verwendeter Methode `200 OK` oder `202 Accepted` zurückgeben.

Eine erfolgreiche Erstellungsoperation in einer vorhandenen Ressourceninstanz gibt `200 OK` zurück. 


#### <a name="response-body"></a>Antworttext

Für alle unterstützten Ressourcen außer [Gruppenbeiträge](../resources/post.md) gilt: Wenn Sie eine erweiterte Eigenschaft erstellen, enthält die Antwort nur die neue oder bereits vorhandene Instanz, nicht jedoch die neue erweiterte Eigenschaft. Möchten Sie die neu erstellte erweiterte Eigenschaft sehen, [müssen Sie die um die erweiterte Eigenschaft erweiterte Instanz abrufen](../api/multivaluelegacyextendedproperty_get.md).

Beim Erstellen einer erweiterten Eigenschaft in einem _neuen_ Gruppenbeitrag enthält die Antwort nur einen Antwortcode, nicht aber den neuen Beitrag oder die erweiterte Eigenschaft. In bereits vorhandenen Gruppenbeiträgen können Sie keine erweiterten Eigenschaften erstellen.


## <a name="example"></a>Beispiel
##### <a name="request-1"></a>Anforderung 1

Im ersten Beispiel wird mit einer einzigen POST-Operation eine mehrwertige erweiterte Eigenschaft in einem neuen Ereignis erstellt. Abgesehen von den Eigenschaften, die Sie normalerweise für ein neues Ereignis definieren würden, enthält der Anforderungstext die **multiValueExtendedProperties**-Sammlung. Diese wiederum enthält eine erweiterte Eigenschaft. Der Anforderungstext enthält die folgenden Parameter für diese mehrwertige erweiterte Eigenschaft:

- **id**: Dieser Parameter definiert die Eigenschaft als ein Array von Zeichenfolgen mit der angegebenen GUID und dem Namen `Recreation`. 
- **value**: Dieser Parameter definiert `Recreation` als ein Array von 3 Zeichenfolgewerten, `["Food", "Hiking", "Swimming"]`.
 

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/events
Content-Type: application/json

{
  "subject": "Family reunion",
  "body": {
    "contentType": "HTML",
    "content": "Let's get together this Thanksgiving!"
  },
  "start": {
      "dateTime": "2015-11-26T09:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2015-11-29T21:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "attendees": [
    {
      "emailAddress": {
        "address": "Terrie@contoso.com",
        "name": "Terrie Barrera"
      },
      "type": "Required"
    },
    {
      "emailAddress": {
        "address": "Lauren@contoso.com",
        "name": "Lauren Solis"
      },
      "type": "Required"
    }
  ],
  "multiValueExtendedProperties": [
     {
           "id":"StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation",
           "value": ["Food", "Hiking", "Swimming"]
     }
  ]
}
```

##### <a name="response-1"></a>Antwort 1

Eine erfolgreiche Antwort wird mit dem Antwortcode `HTTP 201 Created` gekennzeichnet und enthält das neue Ereignis im Antworttext, ähnlich wie die Antwort, die zurückgegeben wird, wenn Sie [nur ein Ereignis erstellen](../api/user_post_events.md). Die Antwort enthält keine neu erstellten erweiterten Eigenschaften.

Möchten Sie die neu erstellte erweiterte Eigenschaft sehen, [müssen Sie das um die erweiterte Eigenschaft erweiterte Ereignis abrufen](../api/multivaluelegacyextendedproperty_get.md).


****

##### <a name="request-2"></a>Anforderung 2

Das zweite Beispiel erstellt eine mehrwertige erweiterte Eigenschaft für die angegebene Nachricht. Diese erweiterte Eigenschaft ist das einzige Element in der **multiValueExtendedProperties**-Sammlung. Der Anforderungstext enthält die folgenden Parameter für diese erweiterte Eigenschaft:

- **id**: Dieser Parameter definiert die Eigenschaft als ein Array von Zeichenfolgen mit der angegebenen GUID und dem Namen `Palette`.
- **value**: Dieser Parameter definiert `Palette` als ein Array von 3 Zeichenfolgewerten, `["Green", "Aqua", "Blue"]`.

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2_as77AACHsLrBBBA=')

Content-Type: application/json

{
  "multiValueExtendedProperties": [
      {
         "id":"StringArray {66f5a359-4659-4830-9070-00049ec6ac6e} Name Palette",
         "value":["Green", "Aqua", "Blue"]
      }
    ]
}
```

##### <a name="response-2"></a>Antwort 2

Eine erfolgreiche Antwort wird mit dem Antwortcode `HTTP 200 OK` gekennzeichnet und enthält die angegebene Nachricht im Antworttext, ähnlich wie die Antwort, die zurückgegeben wird, wenn Sie [eine Nachricht aktualisieren](../api/message_update.md). Die Antwort enthält nicht die neu erstellte erweiterte Eigenschaft.

Möchten Sie die neu erstellte erweiterte Eigenschaft sehen, [müssen Sie die um die erweiterte Eigenschaft erweiterte Nachricht abrufen](../api/multivaluelegacyextendedproperty_get.md).


<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create a single-value extended property",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->




