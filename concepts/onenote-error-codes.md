---
title: Fehlercodes für OneNote-APIs in Microsoft Graph
description: Dieser Artikel beschreibt Fehlercodes, die von der OneNote-API zurückgegeben werden, wenn eine von der API gesendete Anfrage fehlschlägt.
ms.openlocfilehash: 265929be081ee61a88b8baf4f600e2c154797ec7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092265"
---
# <a name="error-codes-for-onenote-apis-in-microsoft-graph"></a>Fehlercodes für OneNote-APIs in Microsoft Graph

Dieser Artikel beschreibt Fehlercodes, die von der OneNote-API zurückgegeben werden, wenn eine von der API gesendete Anfrage fehlschlägt.

## <a name="error-response-example"></a>Fehlerantwort-Beispiel

Wenn Ihre Anforderung einen Fehler generiert, hält die OneNote-API die Ausführung der Anforderung an und gibt eine Fehlerantwort als JSON-Objekt zurück. Eine Fehlerantwort enthält den zugehörigen Fehlercode, eine Nachricht und einen Link zum entsprechenden Abschnitt dieses Artikels. Im folgenden Beispiel wird eine Fehlerantwort veranschaulicht.

```json
{
   "error":{
      "code":"10002",
      "message":"The service is currently unavailable. Please try again later.",
      "innerError": {
        "requestId": "request-id",
        "date": "date-time"
      }
   }
}
```

Weitere Informationen zu Microsoft Graph-Fehlern finden Sie unter [Microsoft Graph-Fehlerantworten und Ressourcentypen](errors.md).

## <a name="codes-from-10001-to-19999"></a>Codes von 10001-19999

Der Dienst hat Probleme oder sendet Informationen zur Anwendung.

### <a name="10001"></a>10001
Ein unerwarteter Fehler ist aufgetreten, und die Anforderung ist fehlgeschlagen.

### <a name="10002"></a>10002
Der Dienst ist derzeit nicht verfügbar.

### <a name="10003"></a>10003
Das Konto des aktuellen Benutzers hat die Maximalanzahl an aktiven Anforderungen überschritten. Ihre App muss die Anforderung wiederholen.

### <a name="10004"></a>10004
Der Dienst kann keine Seite im angeforderten Abschnitt erstellen, da der Abschnitt kennwortgeschützt ist.

### <a name="10005"></a>10005
Die Anforderung enthält mehr als die Maximalanzahl an Bildtags, wobei das **data-render-src**-Attribut eine PDF enthält. Siehe [Hinzufügen von Bildern und Dateien](onenote-images-files.md)

### <a name="10006"></a>10006
Die OneNote-API konnte keine Seite im angegebenen Abschnitt erstellen, da dieser Abschnitt beschädigt ist.

### <a name="10007"></a>10007
Der Server ist zu ausgelastet, um die eingehende Anforderung zu bearbeiten. Bitte versuchen Sie es später erneut.

### <a name="10008"></a>10008
Eine oder mehrere der Dokumentbibliotheken des OneDrive-Benutzers oder der -Gruppe enthalten mehr als 5.000 OneDrive-Elemente (Notizbücher, Abschnitte, Abschnittsgruppen) und können nicht mithilfe der API abgefragt werden. Stellen Sie sicher, dass keine der Benutzer- oder Gruppen-Dokumentbibliotheken mehr als 5.000 OneNote-Elemente enthält. Im [OneNote-Entwicklerblog](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/) finden Sie Informationen zur Reduzierung der Elemente.

### <a name="10012"></a>10012
Die Entität kann nicht erstellt oder aktualisiert werden, da aus der Bibliothek, die das Notizbuch enthält, Elemente ausgecheckt werden müssen, bevor diese bearbeitet werden können. Weitere Informationen finden Sie unter [Einrichten einer Bibliothek, um das Auschecken von Dateien erforderlich zu machen](https://support.office.com/de-DE/article/Configure-a-site-library-to-require-check-out-of-files-f63fcbdc-1db6-4eb7-a3eb-dd815500c9e7).

Entfernen Sie entweder die Anforderung zum Auschecken aus der Bibliothek oder verschieben Sie das Notizbuch.

### <a name="10013"></a>10013
Eine oder mehrere Dokumentbibliotheken in OneDrive des Benutzers oder der Gruppe enthalten mehr als 20.000 Elemente und können nicht für das Abfragen mithilfe der API indiziert werden. Stellen Sie sicher, dass keine der Dokumentbibliotheken des Benutzers oder der Gruppe mehr als 20.000 Elemente enthält. Schritte zur Lösung des Problems finden Sie im [OneNote Developer-Blog](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/).

### <a name="10014"></a>10014
Azure Key Vault ist zu ausgelastet, um die eingehende Anforderung zu bearbeiten. Versuchen Sie es später erneut.

### <a name="10015"></a>10015
SharePoint ist derzeit nicht verfügbar. Versuchen Sie es später erneut.

### <a name="10016"></a>10016
Die Dokumentbibliothek des OneDrive-Benutzers oder der -Gruppe hat den Sicherheitsschwellwert überschritten. Der Sicherheitsschwellwert von 50.000 für die Bibliothek darf nicht überschritten werden.

### <a name="10017"></a>10017
Ungültige Anforderung.

### <a name="19999"></a>19999
Die Anforderung ist fehlgeschlagen, da ein unbekannter Fehler aufgetreten ist.

## <a name="codes-from-20001-to-29999"></a>Codes von 20001 bis 29999

Der Anwendungscode hat einen Fehler gemacht.

### <a name="20001"></a>20001

In der Anforderung fehlt der erforderliche "Präsentation"-Teil. Es ist einer erforderlich. 

### <a name="20002"></a>20002
Die Anforderung enthält zwei oder mehr "Präsentation"-Teile. Es ist einer erforderlich.

### <a name="20003"></a>20003
Der Inhaltstyp des "Präsentation"-Teils kann nur Text/HTML oder Anwendung/XHTML + XML sein. 

### <a name="20004"></a>20004
Der HTML-Code des "Presentation"-Teils enthält ein Bildtag, bei dem sowohl die Eigenschaft **src** als auch die Eigenschaft **data-render-src** festgelegt ist. Die API ignoriert die Eigenschaft **src** und verwendet die Eigenschaft **data-render-src**. 

### <a name="20005"></a>20005
Die Anforderungs-URI ist zu lang. Der maximale Länge der Anforderungs-URI (einschließlich aller Parameter und Daten) beträgt 16 KB oder 16.384 Zeichen.

### <a name="20006"></a>20006
Die „Presentation”-Teil-HTML enthält ein Bild-Tag, für das weder eine src- noch eine **data-render-src**-Eigenschaft festgelegt wurde. Die API ignoriert das **image**-Tag. 

### <a name="20007"></a>20007
Die „Presentation”-Teil-HTML enthält eine Zeichenfolge mit Erstellungsdatum/-Uhrzeit, die keinem zulässigen Format entspricht. 

### <a name="20008"></a>20008
Die Anforderung ist zu groß. 

### <a name="20009"></a>20009
Die Anforderung enthält Teile mit identischen Namen. Teilnamen müssen eindeutig sein. 

### <a name="20010"></a>20010
Die Kopfzeile „Content-Disposition“ wurde nicht für den angegebenen Inhaltstyp festgelegt. 

### <a name="20011"></a>20011
Die Anforderung enthält eine ungültige mehrteilige Nutzlast. Das Problem kann durch fehlende Leerzeilen, eine fehlende letzten Zeile, falsch formatierte Teil-Trennzeichen usw. ausgelöst werden. Wenn Sie die mehrteilige Nachricht manuell erstellen, überprüfen Sie sorgfältig die Logik oder ziehen Sie eine Drittanbieter-Bibliothek hinzu. 

### <a name="20012"></a>20012
Die Anforderung stellt keinen Inhaltstyp für das angegebene Teil zur Verfügung. 

### <a name="20013"></a>20013
Die Anforderung stellt keinen Inhaltstyp und keine Kopfzeile für die Content-Disposition für das angegebene Teil zur Verfügung. 

### <a name="20014"></a>20014
Die Länge eines Teils in der mehrteiligen Nachricht überschreitet die maximale Größe von 25 MB. 

### <a name="20015"></a>20015
Die Anzahl der Teile in der mehrteiligen Nachricht überschreitet die Begrenzung von 500. 

### <a name="20016"></a>20016
Die Länge der mehrteiligen Nachricht überschreitet die maximale Größe von 75 MB. 

### <a name="20017"></a>20017
Die E-Mail-MIME ist fehlerhaft. 

### <a name="20018"></a>20018
Die Besprechungs-MIME oder -ICal ist fehlerhaft. 

### <a name="20019"></a>20019
Es wurde kein ICal gefunden. 

### <a name="20020"></a>20020
Es wurde ein fehlerhafter Json-Anforderungstext gefunden. 

### <a name="20100"></a>20100
Etwas stimmt mit der Syntax der Anforderung nicht. 

### <a name="20101"></a>20101
Die angeforderte Eigenschaft ist nicht vorhanden.

### <a name="20102"></a>20102
Sie haben eine Ressource angefordert, die nicht vorhanden ist.

### <a name="20103"></a>20103
Die **expand**-Abfrage wird für diese Anforderung nicht unterstützt. Siehe [Unterstützte Zeichenfolge-Optionen für OData-Anfragen](onenote-get-content.md#supported-odata-query-string-options).

### <a name="20104"></a>20104
Die **pagelevel**-Abfrageoption wird nur unterstützt, wenn Sie eine Abfrage für die Seitensammlung in einem Abschnitt oder für eine bestimmte Seite ausführen. Beispiel:  

```http
GET ../sections/{id}/pages?pagelevel=true
GET ../pages/{id}?pagelevel=true
```

### <a name="20106"></a>20106
Ihre Anforderung enthält einen Abfrageoperator, der nicht unterstützt wird. 

### <a name="20108"></a>20108
Die Anforderung enthält nicht unterstützte OData-Abfrageparameter.

### <a name="20109"></a>20109
Die Nutzlast in der PATCH-Anforderung wurde nicht ordnungsgemäß erstellt.

### <a name="20110"></a>20110
Bei Anfragen für die Erstellung von Seiten mit Datenteilen muss der Inhalt mehrteilig sein und einen „Präsentation“-Teil enthalten. 

### <a name="20111"></a>20111
Ihre Anforderung verwendet ein OData-Feature, das nicht unterstützt wird.

### <a name="20112"></a>20112
Ihre Anfrage enthält eine ungültige ID für das Ziel-Notebook, die Abschnittsgruppe, den Abschnitt oder die Seitenentität.

### <a name="20113"></a>20113
Die in der Anforderung angegebene Ressource wurde gelöscht.

### <a name="20115"></a>20115
Der Name enthält ungültige Zeichen. Der Name des Notizbuchs darf die folgenden Zeichen nicht enthalten: `? * \ / : < > | ' "`

### <a name="20117"></a>20117
Ein Element mit dem angegebenen Namen ist bereits im angegebenen Ort vorhanden.

### <a name="20119"></a>20119
Die HTML im „Presentation“-Teil enthält ein **data-attachment**-Attribut, das kein gültiges Format hat oder einen oder mehrere dieser ungültigen Zeichen für einen Dateinamen enthält: `\ / : * ? < > | "`. Die Anforderung hat den Wert in der Fehlermeldung ersetzt.

### <a name="20120"></a>20120
Die Anforderung gibt ein PATCH-Ziel an, das nicht gefunden werden kann.

### <a name="20121"></a>20121
Die Anforderung enthält ein ungültiges PATCH-Argument. Weitere Informationen finden Sie unter [Aktualisieren von Seiteninhalt](onenote-update-page.md).

### <a name="20122"></a>20122
Ihre Anforderung gibt eine nicht unterstützte PATCH-Aktion an. Weitere Informationen finden Sie unter [Aktualisieren von Seiteninhalt](onenote-update-page.md).

### <a name="20123"></a>20123
Die PATCH-Anforderung kann die angegebene Seite nicht ändern.

### <a name="20124"></a>20124
Die mehrteilige PATCH-Anforderung beinhaltet keinen „Befehle“-Teil mit der PATCH-Aktion-JSON-Struktur. Siehe [Aktualisieren von Seiteninhalt](onenote-update-page.md).

### <a name="20125"></a>20125
Die PATCH-Anforderung enthält keine Aktionen. Weitere Informationen finden Sie unter [Aktualisieren von Seiteninhalt](onenote-update-page.md).

### <a name="20126"></a>20126
Der Nachrichtentext enthält entweder falsch formatierten JSON-Code oder Felder, die für diesen Vorgang nicht unterstützt werden.

### <a name="20127"></a>20127
Die Anfrage gibt den Namen einer unbekannten Eigenschaft an.

### <a name="20128"></a>20128
Die Anforderung enthält einen OData-Syntaxfehler an der in der Nachricht angegebenen Position.

### <a name="20129"></a>20129
Die Anforderung enthält eine **top**-Abfrage-Zeichenfolgeoption, deren Wert zu hoch ist. Der Maximalwert für Seitenabfragen beträgt 100, und der Standardwert ist 20.

### <a name="20130"></a>20130
Die Anforderung enthält einen URI, der zu einer HTTP-Ressource zeigt, die nicht gefunden werden kann.

### <a name="20131"></a>20131
Die Anforderung enthält einen ungültigen Wert für den Inhaltstyp. Verwenden Sie den in der Nachricht angegeben Wert. 

### <a name="20132"></a>20132
Die Anforderung enthält ungültige Inhalte. Häufige Ursachen hierfür sind eine fehlende Kopfzeile für die Inhaltstyp-Anfrage und/oder keine Inhalte im Textkörper der Anfrage. 

### <a name="20133"></a>20133
Die Anforderung gibt ein PATCH-Ziel an, das nicht unterstützt wird. Siehe [Aktualisieren von Seiteninhalt](onenote-update-page.md).

### <a name="20134"></a>20134
Die Anforderung gibt ein ungültiges Element als Ziel der PATCH-Aktion an. Wenn das Ziel den **data-id**-Bezeichner verwendet, stellen Sie sicher, dass ein #-Symbol diesem vorangestellt ist. Weitere Informationen finden Sie unter [Aktualisieren von Seiteninhalt](onenote-update-page.md).

### <a name="20135"></a>20135
Die Anforderung gibt einen Entitätstyp an, der für den PATCH-Vorgang nicht unterstützt wird. Siehe [Aktualisieren von Seiteninhalt](onenote-update-page.md).

### <a name="20136"></a>20136
Ihre Anforderung enthält ein ungültiges oder fehlendes **data-render-src**- oder **data-render-method**-Attribut. Siehe [Extrahieren von Daten aus Bildschirmausschnitten](onenote-extract-data.md).

### <a name="20137"></a>20137
Die Zielseite unterstützt keine PATCH-Anforderungen.

### <a name="20138"></a>20138
Das Ziel in der PATCH-Anforderung unterstützt die angegebene **append**Aktion nicht. Weitere Informationen finden Sie unter [Aktualisieren von Seiteninhalt](onenote-update-page.md).

### <a name="20139"></a>20139
Die Anforderung enthält einen ungültigen **data-tag**-Attributwert. Weitere Informationen finden Sie unter [Verwenden von Notiztags](onenote-note-tags.md).

### <a name="20140"></a>20140
Die Anforderung enthält einen ungültigen **data-tag**-Statuswert. Kontrollkästchen-Notiztags können den Status **completed** besitzen. 

Beispiel:

```html
    <p data-tag="to-do:completed">To-do note tag in completed state (checked box in the UI)</p>
```
Siehe [Verwenden von Notiztags](onenote-note-tags.md).

### <a name="20141"></a>20141
Der Zielelementtyp in der PATCH-Anforderung unterstützt die angegebene Aktion nicht. Siehe [Aktualisieren von Seiteninhalt](onenote-update-page.md).

### <a name="20142"></a>20142
Ihre Anforderung enthält einen **expand**-Ausdruck für ein übergeordnetes Element untergeordneter Entitäten oder ein untergeordnetes Element übergeordneter Entitäten, der nicht unterstützt wird. Siehe [Unterstützte Zeichenfolge-Optionen für OData-Anfragen](onenote-get-content.md#supported-odata-query-string-options).

### <a name="20143"></a>20143
Die OData-Abfrage ist ungültig.

### <a name="20144"></a>20144
Die Anforderung enthält einen **expand**-Ausdruck für eine Nicht-Navigationseigenschaft. Nur Navigationseigenschaften können erweitert werden.

### <a name="20145"></a>20145
Der **select**- oder **expand**-Ausdruck in der Anforderung enthält einen ungültigen Term.

### <a name="20146"></a>20146
Das `style="position:absolute"`-Attribut wurde für ein Element angegeben, aber das **body**-Element gibt `data-absolute-enabled="true"` nicht an, das jedoch für die Unterstützung der Positionierung erforderlich ist. Alle Positionseinstellungen werden ignoriert. Siehe [Erstellen von absolut positionierten Elementen](onenote-abs-pos.md).

### <a name="20147"></a>20147
Das `style="position:absolute"`-Attribut ist für ein Element angegeben, das kein direkt untergeordnetes Element des **body**-Elemente ist, welches nicht unterstützt wird. Wenn das Element **div**, **img** oder **object** ist, muss es als untergeordnetes Element des Textkörpers angegeben werden; andernfalls werden die Positionseinstellungen ignoriert und die dazugehörigen Inhalte werden als absolut positioniertes div dargestellt. Siehe [Erstellen von absolut positionierten Elementen](onenote-abs-pos.md).

### <a name="20148"></a>20148
Das `style="position:absolute"`-Attribut ist für einen nicht unterstützten Elementyp angegeben. Nur **div**-, **img**- und **object**-Elemente, die direkt untergeordnete Elemente des Seitentextes sind, unterstützten die Positionierung. Siehe [Erstellen von absolut positionierten Elementen](onenote-abs-pos.md).

### <a name="20149"></a>20149
Die Anforderung gibt ein Zielelement an, das nicht gefunden werden kann.

### <a name="20150"></a>20150
Die Anforderung ist für diesen Authentifizierungstyp nicht gültig.  Verwenden Sie stattdessen den `../me/onenote/`-Pfad.

### <a name="20151"></a>20151
Die Anforderung ist für diesen Authentifizierungstyp nicht gültig. Verwenden Sie den `../me/onenote/section/{id}/pages`-Endpunkt, um eine Seite in einem bestimmten Abschnitt zu erstellen.

### <a name="20152"></a>20152
Für die Entität ist kein name-Wert angegeben. Der Name muss definiert werden, und er darf nicht nur aus Leerzeichen bestehen.

### <a name="20153"></a>20153
Der Entitätsname enthält ungültige Zeichen. Der Name darf die folgenden Zeichen nicht enthalten: `? * \ / : < > | & # " % ~`

### <a name="20154"></a>20154
Der Entitätsname darf nicht mit einem Leerzeichen beginnen.

### <a name="20155"></a>20155
Der Entitätsname ist zu lang. Namen für Notizbücher dürfen maximal 128 Zeichen lang sein. Andere Entitätsnamen dürfen maximal 50 Zeichen lang sein.

### <a name="20156"></a>20156
Die angegebene ID für die Zielressource ist nicht vorhanden.

### <a name="20157"></a>20157
Die angegebene ID für die Zielentität ist ungültig.

### <a name="20158"></a>20158
Die Metadaten für die Website-URL in der angegebenen Anfrage können nicht abgerufen werden. Überprüfen Sie das Format der angegebenen URL. Zu den unterstützten Formate gehören `https://domain.sharepoint.com/site-a` und `https://domain.com/sites/site-a`.

### <a name="20160"></a>20160
Es kann keine einheitliche Office 365-Gruppe mit der angegebenen ID gefunden werden.

### <a name="20161"></a>20161
Der Kontext gibt keine gültige Benutzer-ID an. Ein häufiger Fehler ist, dass die PUID/CID in Langform statt als Hexadezimalwert übergeben wurde.

### <a name="20166"></a>20166
Die Anwendung hat zu viele Anfragen im Auftrag eines Benutzers innerhalb eines kurzen Zeitraums ausgegeben. Um sicherzustellen, dass die OneNote-API stabil und reaktionsschnell bleibt, gibt die API den Statuscode 429 und diesen Fehler aus, wenn sie erkennt, dass eine Anwendung zu viele Ressourcen verwendet. 

Weitere Informationen finden Sie unter [Drosselung von OneNote-API und wie Sie dies vermeiden](https://blogs.msdn.com/b/onenotedev/archive/2016/01/13/onenote-api-throttling-and-best-practices.aspx).

### <a name="20168"></a>20168
Die in der Anfrage angegebene Video-Quelle wird nicht unterstützt. Eine aktuelle Liste finden Sie unter [Unterstützte Video-Websites](onenote-images-files.md#adding-videos).


## <a name="codes-from-30001-to-39999"></a>Codes von 30001 bis 39999
Etwas stimmt nicht mit dem Benutzerkonto.

### <a name="30101"></a>30101
Das Benutzerkonto hat das OneDrive-Kontingent überschritten. Siehe [OneDrive](https://onedrive.live.com/about/de-DE/).

### <a name="30102"></a>30102
Es kann nichts mehr zum angeforderten Abschnitt hinzugefügt werden, da dieser seine maximale Größe ereicht hat.

### <a name="30103"></a>30103
Der Ressourceverbrauch ist zu hoch für die Anforderung. Entweder weist das Benutzerkonto ein zu großes Datenset auf, oder der Dienst erhält eine große Anzahl konkurrierender Anforderungen für dieselbe Website (z. B. die persönliche Website des Benutzers oder eine Teamwebsite).

### <a name="30104"></a>30104
Das Benutzerkonto wurde angehalten.

### <a name="30105"></a>30105
Die persönliche OneDrive for Business-Website des Benutzers, die für den Zugriff auf Notizbücher erforderlich ist,  wird nicht bereitgestellt. Der OneNote-Dienst stellt die Seite jetzt bereit. Dieser Vorgang kann mehrere Minuten dauern.

### <a name="30106"></a>30106
OneDrive for Business wird für den Benutzer bereitgestellt.

### <a name="30108"></a>30108
Das persönliche OneDrive for Business des Benutzers konnte nicht abgerufen werden. Die folgende Tabelle enthält mögliche Ursachen.

| Ursache | Lösung |
|:------|:------|
| Die persönliche Website des Benutzers wurde nicht bereitgestellt. | Der Benutzer sollte OneDrive for Business öffnen und die Anweisungen befolgen, um die Website bereitzustellen. Wenn dies fehlschlägt, sollten er sich an seinen Office 365-Mandanten-Administrator wenden. |
| Die persönliche Website des Benutzers wird derzeit bereitgestellt. | Senden Sie die Anforderung später erneut. |
| Der Benutzer besitzt keine gültige OneDrive for Business-Lizenz. | Der Benutzer sollte sich an seinen Office 365-Mandanten-Administrator wenden. |
| Die Anfrage konnte aufgrund eines Netzwerkfehlers nicht erfolgreich versendet werden. | Senden Sie die Anforderung später erneut. |

### <a name="30109"></a>30109
Einige Benutzer in der Anforderung sind nicht vorhanden.

### <a name="30110"></a>30110
Student Information Services wurde nicht für diesen Mandanten registriert.

### <a name="30111"></a>30111
Es ist ein allgemeiner Fehler mit Student Information Services aufgetreten.

### <a name="30112"></a>30112
Mehrere Benutzer, die von dieser Anforderung betroffen waren, besitzen den gleichen Benutzernamen.

### <a name="30113"></a>30113
Das Notizbuch ist nicht für Einladungen konfiguriert.

### <a name="30114"></a>30114
Ein erforderlicher Parameter fehlt.

## <a name="codes-from-40001-to-49999"></a>Codes von 40001 bis 49999
Der Benutzer oder die Anwendung besitzt nicht die erforderlichen Berechtigungen.

### <a name="40001"></a>40001
Die Anforderung enthält kein gültiges OAuth-Token. Siehe [Notizberechtigungen](permissions-reference.md#notes-permissions).

### <a name="40002"></a>40002
Der Benutzer hat keine Berechtigung, an den angeforderten Ort zu schreiben.

### <a name="40003"></a>40003
Der Benutzer hat keine Berechtigung, auf die angeforderte Ressource zuzugreifen.

### <a name="40004"></a>40004
Das OAuth-Token hat nicht den erforderlichen Umfang, um die angeforderte Aktion durchzuführen. Siehe [Notizberechtigungen](permissions-reference.md#notes-permissions).

### <a name="40006"></a>40006 
Das OAuth-Token hat nicht den erforderlichen Umfang, um die angeforderte Aktion durchzuführen. Bearbeiten Sie die Berechtigung entsprechend. Siehe [Notizberechtigungen](permissions-reference.md#notes-permissions).

### <a name="40007"></a>40007
Der Benutzer hat nicht die Berechtigungen, auf diese Ressource zuzugreifen.

### <a name="40008"></a>40008
Der Zugriff ist für diese Ressource nicht zulässig.

### <a name="40009"></a>40009
Der Container wird bereits von einer anderen Ressource verwendet.

## <a name="see-also"></a>Siehe auch

- [Microsoft Graph-Fehlerantworten und -Ressourcentypen](errors.md)
- [OneNote-Referenz](/graph/api/resources/onenote?view=graph-rest-1.0)

