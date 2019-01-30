---
title: singleValueLegacyExtendedProperty abrufen
description: Sie können eine einzelne Ressourceninstanz erweitert mit einer bestimmten erweiterten Eigenschaft oder eine Auflistung von Resource-Instanzen abzurufen.
localization_priority: Normal
ms.openlocfilehash: ead4881737f4431138d444ffe8df131c22c131fc
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641407"
---
# <a name="get-singlevaluelegacyextendedproperty"></a>singleValueLegacyExtendedProperty abrufen

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Sie können eine einzelne, mit einer bestimmten erweiterten Eigenschaft erweiterte Ressourceninstanz oder eine Sammlung von Ressourceninstanzen abrufen, die einem Filter entsprechende erweiterte Eigenschaften enthalten.

Mit dem Abfrageparameter `$expand` können Sie die angegebene Ressourceninstanz, erweitert um die angegebene erweiterte Eigenschaft, abrufen. Wenden Sie einen `$filter`- und einen `eq`-Operator auf die **ID**-Eigenschaft an, um die erweiterte Eigenschaft anzugeben. Dies ist derzeit die einzige Möglichkeit zum Abrufen des [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)-Objekts, das eine erweiterte Eigenschaft darstellt. 

Um Ressourceninstanzen mit bestimmten erweiterten Eigenschaften abzurufen, verwenden Sie den Abfrageparameter `$filter`, und wenden Sie einen `eq`-Operator auf die **ID**-Eigenschaft an. Wenden Sie für nummerische erweiterte Eigenschaften zudem einen der folgenden Operatoren auf die Eigenschaft **Wert** an: `eq`, `ne`,`ge`, `gt`, `le` oder `lt`. Für erweiterte Eigenschaften vom Typ Zeichenfolge wenden Sie einen `contains`-, `startswith`-, `eq`-, oder `ne`-Operator auf den **Wert** an. 

Beim Filtern des Namens der Zeichenfolge (`Name`) in der **ID** einer erweiterten Eigenschaft wird die Groß-/Kleinschreibung beachtet. Beim Filtern der Eigenschaft **Wert** einer erweiterten Eigenschaft wird die Groß-/Kleinschreibung beachtet.

Die folgenden Benutzerressourcen werden unterstützt:

- [calendar](../resources/calendar.md)
- [contact](../resources/contact.md)
- [contactFolder](../resources/contactfolder.md) 
- [event](../resources/event.md)
- [mailFolder](../resources/mailfolder.md)
- [message](../resources/message.md) 
- [Outlook-Aufgabe](../resources/outlooktask.md)
- [Outlook-Ordner "Aufgaben"](../resources/outlooktaskfolder.md)

Darüber hinaus werden die folgenden Gruppenressourcen unterstützt:

- [calendar](../resources/calendar.md)-Ressourcen für Gruppen
- [event](../resources/event.md)-Ressourcen für Gruppen
- [post](../resources/post.md)-Ressourcen für Gruppen 

Im [Übersichtsartikel zu erweiterten Eigenschaften](../resources/extended-properties-overview.md) finden Sie weitere Informationen dazu, wann Sie offene Erweiterungen verwenden sollten und wann erweiterte Eigenschaften. Außerdem erfahren Sie dort, wie erweiterte Eigenschaften angegeben werden.

## <a name="permissions"></a>Berechtigungen
Je nach der Ressource kommen die erweiterte Eigenschaft aus und geben Sie die Berechtigung (delegierte oder-Anwendung) Sie Anforderung, die Berechtigung, die in der folgenden Tabelle angegeben ist mindestens erforderlich, um diese API-aufrufen. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).

| Unterstützte Ressource | Delegiert (Geschäfts-, Schul- oder Unikonto) | Delegiert (persönliches Microsoft-Konto) | Application |
|:-----|:-----|:-----|:-----|
| [Kalender](../resources/calendar.md) | Calendars.Read | Calendars.Read | Calendars.Read |
| [Kontakt](../resources/contact.md) | Contacts.Read | Contacts.Read | Contacts.Read |
| [contactFolder](../resources/contactfolder.md) | Contacts.Read | Contacts.Read | Contacts.Read |
| [event](../resources/event.md) | Calendars.Read | Calendars.Read |  Calendars.Read|
| [calendar](../resources/calendar.md)-Ressourcen für Gruppen | Group.Read.All | Nicht unterstützt | Nicht unterstützt |
| [event](../resources/event.md)-Ressourcen für Gruppen | Group.Read.All | Nicht unterstützt | Nicht unterstützt |
| [post](../resources/post.md)-Ressourcen für Gruppen | Group.Read.All | Nicht unterstützt | Group.Read.All |
| [mailFolder](../resources/mailfolder.md) | Mail.Read | Mail.Read | Mail.Read |
| [message](../resources/message.md) | Mail.Read | Mail.Read | Mail.Read |
| [Outlook-Aufgabe](../resources/outlooktask.md) | Tasks.Read | Tasks.Read | Nicht unterstützt |
| [Outlook-Ordner "Aufgaben"](../resources/outlooktaskfolder.md) | Tasks.Read | Tasks.Read | Nicht unterstützt |


## <a name="http-request"></a>HTTP-Anforderung

#### <a name="get-a-resource-instance-expanded-with-an-extended-property-that-matches-a-filter"></a>Abrufen einer Ressourceninstanz, erweitert um eine erweiterte Eigenschaft, die einem Filter entspricht
Hier sehen Sie, wie Sie eine Ressourceninstanz abrufen können, erweitert um die erweiterte Eigenschaft, deren **id**-Eigenschaft dem definierten Filter entspricht. Stellen Sie sicher, dass Sie für die Leerzeichen in der Filterzeichenfolge die [URL-Codierung](https://www.w3schools.com/tags/ref_urlencode.asp) verwenden.

Erhalten Sie eine Instanz der **Nachricht** :<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
Eine **MailFolder** -Instanz abrufen:<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

Rufen Sie eine Instanz **Ereignis** :<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
Eine **Kalender** -Instanz abrufen:<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

Abrufen einer Instanz **wenden Sie sich an** :<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
Eine **ContactFolder** -Instanz abrufen:<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

Erhalten Sie eine Instanz **OutlookTask** :<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
Erhalten Sie eine Instanz **OutlookTaskFolder** :<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

Eine Gruppe **Ereignis** Instanz abrufen:<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

Eine Gruppe **Buchen** -Instanz abrufen:<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-that-include-numeric-extended-properties-matching-a-filter"></a>Abrufen von Ressourceninstanzen, die numerische erweiterte Eigenschaften enthalten, die einem Filter entsprechen

Rufen Sie Instanzen einer unterstützten Ressource ab, die eine numerische erweiterte Eigenschaft besitzen, die einem Filter entspricht. Der Filter wendet einen `eq`-Operator auf die **ID**-Eigenschaft und einen der folgenden Operatoren auf die Eigenschaft **Wert** an: `eq`, `ne`,`ge`, `gt` , `le` oder `lt`. Stellen Sie sicher, dass Sie anwenden, stellen Sie sicher, dass Sie auf der folgenden Zeichen in der Filterzeichenfolge - Doppelpunkt, Schrägstrich und Speicherplatz anwenden [URL-Codierung](https://www.w3schools.com/tags/ref_urlencode.asp) .

Die folgenden Syntaxzeilen zeigen einen Filter, der den `eq`-Operator auf die ID anwendet, und einen `eq`-Operator, der auf den Eigenschaftswert angewandt wird. Sie können den `eq`-Operator, der auf den **Wert** angewandt wird, durch einen der anderen Operatoren (`ne`,`ge`, `gt`, `le` oder `lt`) ersetzen, die auf numerische Werte angewandt werden.

**Nachricht** Instanzen abgerufen:<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
**MailFolder** Instanzen abgerufen:<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

**Ereignis** -Instanzen abzurufen:<!-- { "blockType": "ignored" } -->
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
**Kalender** -Instanzen abzurufen:<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
**Wenden Sie sich an** Instanzen abgerufen:<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
**ContactFolder** Instanzen abgerufen:<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

Erhalten Sie eine Instanz **OutlookTask** :<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
Erhalten Sie eine Instanz **OutlookTaskFolder** :<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskGroups/{id}/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

Gruppe **Ereignis** Instanzen abgerufen:<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

Gruppe **Buchen** Instanzen abgerufen:<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

#### <a name="get-resource-instances-with-string-typed-extended-properties-matching-a-filter"></a>Abrufen von Ressourceninstanzen mit erweiterten Eigenschaften des Typs Zeichenfolge, die einem Filter entsprechen

Rufen Sie Instanzen der Ressource **Nachricht** oder **Ereignis** mit einer erweiterten Eigenschaft des Typs Zeichenfolge ab, die einem Filter entspricht. Der Filter wendet einen `eq`-Operator auf die **ID**-Eigenschaft und einen der folgenden Operatoren auf die Eigenschaft **Wert** an: `contains`, `startswith`, `eq` oder `ne`. Stellen Sie sicher, dass Sie für die folgenden Zeichen in der Filterzeichenfolge die [URL-Codierung](https://www.w3schools.com/tags/ref_urlencode.asp) verwenden: Doppelpunkte, Vorwärtsschrägstriche und Leerzeichen.


**Nachricht** Instanzen abgerufen:<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

**Ereignis** -Instanzen abzurufen:<!-- { "blockType": "ignored" } -->
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

Gruppe **Ereignis** Instanzen abgerufen:<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

## <a name="path-parameters"></a>Pfadparameter
|**Parameter**|**Typ**|**Beschreibung**|
|:-----|:-----|:-----|
|id_value|String|Die ID der erweiterten Eigenschaft, nach der gefiltert wird. Sie muss eins der unterstützten Formate aufweisen. Weitere Informationen finden Sie unter [Überblick über erweiterte Eigenschaften in Outlook](../resources/extended-properties-overview.md). Erforderlich.|
|property_value |String|Der Wert der erweiterten Eigenschaft, nach der gefiltert wird. Erforderlich, wo im Abschnitt **HTTP-Anforderung** oben aufgeführt. Wenn {property_value} keine Zeichenfolge ist, müssen Sie sicherstellen, dass `ep/value` explizit in den entsprechenden Edm-Datentyp beim Vergleich mit {property_value} umgewandelt wird. Beispiele finden Sie unter [Anforderung 4](#request-4) weiter unter. |

## <a name="request-headers"></a>Anforderungsheader
| Name      |Beschreibung|
|:----------|:----------|
| Authorization  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.

#### <a name="get-resource-instance-using-expand"></a>Abrufen von Ressourceninstanzen mithilfe von `$expand`
Der Antworttext enthält ein Objekt, das die angeforderte Ressourceninstanz darstellt, erweitert um das dem Filter entsprechende [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)-Objekt.
  
#### <a name="get-resource-instances-that-contain-an-extended-property-matching-a-filter"></a>Abrufen von Ressourceninstanzen mit einer erweiterten Eigenschaft, die einem Filter entspricht
Der Antworttext enthält ein oder mehrere Objekte, die Ressourceninstanzen darstellen, die einem dem Filter entsprechende erweiterte Eigenschaft enthalten. Der Antworttext enthält nicht die erweiterte Eigenschaft.

## <a name="example"></a>Beispiel
#### <a name="request-1"></a>Anforderung 1

Im ersten Beispiel wird die angegebene Nachricht abgerufen und um eine einwertige erweiterte Eigenschaft erweitert. Der Filter gibt die erweiterte Eigenschaft zurück, deren **id** der Zeichenfolge `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` entspricht (URL-Codierung hier zur besseren Lesbarkeit entfernt).

<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
#### <a name="response-1"></a>Antwort 1
Der Antworttext enthält alle Eigenschaften der angegebenen Nachricht und die vom Filter zurückgegebene erweiterte Eigenschaft.

Hinweis: Das hier gezeigte **message**-Objekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AACbyS4H\"",
    "id": "AAMkAGE1M2_bs88AACHsLqWAAA=",
    "subject": "RE: Talk about emergency prep",
    "sender": {
        "emailAddress": {
            "name": "Christine Irwin",
            "address": "christine@contoso.com"
        }
    },
    "from": null,
    "toRecipients": [
        {
            "emailAddress": {
                "name": "Christine Irwin",
                "address": "christine@contoso.com"
            }
        }
    ],
    "singleValueExtendedProperties@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages('AAMkAGE1M2_bs88AACHsLqWAAA%3D')/singleValueExtendedProperties",
    "singleValueExtendedProperties": [
        {
            "id": "String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color",
            "value": "Green"
        }
    ]
}
```

#### <a name="request-2"></a>Anforderung 2

Das zweite Beispiel ruft Nachrichten ab, die die im Filter spezifizierte einwertige erweiterte Eigenschaft vom Typ Zeichenfolge haben. Der Filter sucht nach der erweiterten Eigenschaft, die folgende Merkmale hat:

- Die **ID** entspricht der Zeichenfolge `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (URL-Codierung hier zur besseren Lesbarkeit entfernt).

- Der **Wert** ist gleich der Zeichenfolge `Green`.

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/Me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

#### <a name="response-2"></a>Antwort 2

Eine erfolgreiche Antwort ist durch den Antwortcode `HTTP 200 OK` gekennzeichnet. Der Antworttext enthält alle Eigenschaften der Nachrichten, die die dem Filter entsprechende erweiterte Eigenschaft haben. Der Antworttext ähnelt der Antwort beim [Abrufen einer Nachrichtensammlung](../api/user-list-messages.md). Die Antwort enthält nicht die dem Filter entsprechende erweiterte Eigenschaft.


#### <a name="request-3"></a>Anforderung 3

Das dritte Beispiel ruft Nachrichten ab, die die im Filter spezifizierte einwertige erweiterte Eigenschaft vom Typ Zeichenfolge haben. Der Filter sucht nach der erweiterten Eigenschaft, die folgende Merkmale hat:

- Die **ID** entspricht der Zeichenfolge `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (URL-Codierung hier zur besseren Lesbarkeit entfernt).

- Die **Wert**, der die Zeichenfolge `green` enthält. 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/Me/messages?$filter=singleValueExtendedProperties/any(ep:ep/Id eq 'String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color' and contains(ep/Value, 'green'))
```

#### <a name="response-3"></a>Antwort 3

Eine erfolgreiche Antwort ist durch den Antwortcode `HTTP 200 OK` gekennzeichnet. Der Antworttext enthält alle Eigenschaften der Nachrichten, die die dem Filter entsprechende erweiterte Eigenschaft haben. Wie zum Beispiel eine Nachricht, die eine einwertige erweiterte Eigenschaft mit einer **ID** besitzt, die der Zeichenfolge `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` entspricht, und der **Wert** `Light green` stimmt mit dem Filter überein und ist in der Antwort enthalten.

Der Antworttext ähnelt der Antwort beim [Abrufen einer Nachrichtensammlung](../api/user-list-messages.md). Die Antwort enthält nicht die dem Filter entsprechende erweiterte Eigenschaft.


#### <a name="request-4"></a>Anforderung 4

Die nächsten 2 Beispiele zeigen, wie Sie Nachrichten abrufen, die erweiterte einwertige Eigenschaften vom Typ Nicht-Zeichenfolge enthalten. Zur besseren Lesbarkeit ist die erforderliche URL-Codierung dort nicht enthalten.

Das folgende Beispiel zeigt einen Filter, der nach der erweiterte Eigenschaft mit den folgenden Merkmalen sucht:

- Die **id** entspricht der Zeichenfolge `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.

- Der **Wert** ist die GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`. Wenn Sie den Eigenschaftswert mit einer GUID vergleichen möchten, ändern Sie `ep/value` in `Edm.Guid`.


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid' and cast(ep/value, Edm.Guid) eq (b9cf8971-7d55-4b73-9ffa-a584611b600b))
```

Das folgende Beispiel zeigt einen Filter, der nach der erweiterte Eigenschaft mit den folgenden Merkmalen sucht:

- Die **id** entspricht der Zeichenfolge `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.

- Der **Wert** ist gleich der ganzen Zahl 12. Um den Eigenschaftswert mit einer ganzen Zahl zu vergleichen, ändern Sie `ep/value` in `Edm.Int32`.


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete' and cast(ep/value, Edm.Int32) eq 12)
```


#### <a name="response-4"></a>Antwort 4

Bei den zwei vorhergehenden Beispielen ist eine erfolgreiche Antwort durch den Antwortcode `HTTP 200 OK` gekennzeichnet. Der Antworttext enthält alle Eigenschaften der Nachrichten, die die dem Filter entsprechende erweiterte Eigenschaft haben. Der Antworttext ähnelt der Antwort beim [Abrufen einer Nachrichtensammlung](../api/user-list-messages.md). Die Antwort enthält nicht die dem Filter entsprechende erweiterte Eigenschaft.


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/singlevaluelegacyextendedproperty-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
