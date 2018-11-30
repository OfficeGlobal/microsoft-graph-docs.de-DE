---
title: Datenerweiterung abrufen
description: Dieser Artikel beschreibt, wie Sie eine offene Erweiterung (openTypeExtension-Objekt) basierend auf ihrem Namen oder ihrem vollqualifizierten Namen abrufen können.
ms.openlocfilehash: 599422384ed7e821f0ca50235fd164594bccd4d1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065093"
---
# <a name="get-open-extension"></a>Datenerweiterung abrufen

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Dieser Artikel beschreibt, wie Sie eine offene Erweiterung ([openTypeExtension](../resources/opentypeextension.md)-Objekt) basierend auf ihrem Namen oder ihrem vollqualifizierten Namen abrufen können.

In der folgenden Tabelle sind die drei Szenarien für den Abruf einer offenen Erweiterung aus einer unterstützten Ressourceninstanz aufgeführt.

|**GET-Szenario**|**Unterstützte Ressourcen**|**Antworttext**|
|:-----|:-----|:-----|
|Abrufen einer bestimmen Erweiterung aus einer bekannten Ressourceninstanz| [Administrative Einheit](../resources/administrativeunit.md), [Gerät](../resources/device.md), [Ereignis](../resources/event.md), [Gruppe](../resources/group.md), [Gruppe Ereignis](../resources/event.md), [Gruppe Post](../resources/post.md), [Nachricht](../resources/message.md), [Organisation](../resources/organization.md), [persönlichen Kontakt](../resources/contact.md), [Benutzer](../resources/user.md) | Nur offene Erweiterung|
|Abrufen einer bekannten Ressourceninstanz, erweitert um eine bestimmte Erweiterung|Administrative Einheit, Gerät, -Ereignis, Gruppe, Gruppe Ereignis, Gruppe Post, Nachricht, Organisation, persönlichen Kontakt, Benutzer |Eine um die offene Erweiterung erweiterte Ressourceninstanz|
|Suchen und Erweitern von Ressourceninstanzen mit einer bestimmten Erweiterung | Event, group event, group post, message, personal contact |Um die offene Erweiterung erweiterte Ressourceninstanzen|

## <a name="permissions"></a>Berechtigungen

Je nach der Ressource, die die Erweiterung und die Berechtigung enthält Typ (delegierte oder-Anwendung) angefordert, die Berechtigung, die in der folgenden Tabelle angegebenen mit den geringsten ist erforderlich, um diese API aufzurufen. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).

| Unterstützte Ressource | Delegiert (Geschäfts-, Schul- oder Unikonto) | Delegiert (persönliches Microsoft-Konto) | Anwendung |
|:-----|:-----|:-----|:-----|
| [Gerät](../resources/device.md) | Directory.Read.All | Nicht unterstützt | Device.ReadWrite.All |
| [event](../resources/event.md) | Calendars.Read | Calendars.Read | Calendars.Read |
| [Gruppe](../resources/group.md) | Group.Read.All | Nicht unterstützt | Group.Read.All |
| [group event](../resources/event.md) | Group.Read.All | Nicht unterstützt | Nicht unterstützt |
| [group post](../resources/post.md) | Group.Read.All | Nicht unterstützt | Group.Read.All |
| [Nachricht](../resources/message.md) | Mail.Read | Mail.Read | Mail.Read | 
| [organization](../resources/organization.md) | User.Read | Nicht unterstützt | Nicht unterstützt |
| [personal contact](../resources/contact.md) | Contacts.Read | Contacts.Read | Contacts.Read |
| [Benutzer](../resources/user.md) | User.Read | User.Read | User.Read.All |

## <a name="http-request"></a>HTTP-Anforderung

In diesem Abschnitt finden Sie die Syntax für jedes der drei oben beschriebenen `GET`-Szenarien.

### <a name="get-a-specific-extension-in-a-known-resource-instance"></a>Abrufen einer spezifischen Erweiterung in einer bekannten Ressourceninstanz

Verwenden Sie die gleiche REST-Anforderung wie zum Abrufen der Ressourceninstanz, und geben Sie die Erweiterung in der Navigationseigenschaft **extensions** dieser Instanz an.

<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{Id}/extensions/{extensionId}
GET /devices/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/events/{Id}/extensions/{extensionId}
GET /groups/{Id}/extensions/{extensionId}
GET /groups/{Id}/events/{Id}/extensions/{extensionId}
GET /groups/{Id}/threads/{Id}/posts/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/messages/{Id}/extensions/{extensionId}
GET /organization/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/contacts/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/extensions/{extensionId}
```

### <a name="get-a-known-resource-instance-expanded-with-a-matching-extension"></a>Abrufen einer bekannten Ressourceninstanz, erweitert um eine übereinstimmende Erweiterung 

Für die Ressourcentypen „event“, „group event“, „group post“, „message“ und „personal contact“ können Sie die gleiche REST-Anforderung wie zum Abrufen der Ressourceninstanz verwenden. Suchen Sie zusätzlich per Filter nach einer Erweiterung mit dem gewünschten Wert in der Eigenschaft **id**, und erweitern Sie die Instanz mit der Erweiterung. Die Antwort enthält die meisten der Ressourceneigenschaften.

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
```


Für die Ressourcentypen „device“, „group“, „organization“ und „user“ müssen Sie auch einen `$select`-Parameter verwenden, um die Eigenschaft **Id** und alle anderen gewünschten Eigenschaften aus der Ressourceninstanz einzuschließen:

<!-- { "blockType": "ignored" } -->
```http
GET /devices/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /groups/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /organization/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /users/{Id|userPrincipalName}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
```


### <a name="filter-for-resource-instances-expanded-with-a-matching-extension"></a>Filtern nach Ressourceninstanzen, erweitert mit einer übereinstimmenden Erweiterung 

Verwenden Sie die gleiche REST-Anforderung wie zum Abrufen einer Sammlung der unterstützten Ressource. Filtern Sie die Sammlung nach Instanzen mit einer Erweiterung, die den gewünschten Wert in der Eigenschaft **id** aufweist, und erweitern Sie die betreffenden Instanzen um diese Erweiterung.

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
```

>**Hinweis:** Die obige Syntax zeigt mehrere häufig verwendete Möglichkeiten zum Identifizieren einer Ressourceninstanz oder -sammlung, um eine Erweiterung daraus zu löschen. Alle anderen Syntaxen, mit denen Sie diese Ressourceninstanzen oder -sammlungen identifizieren können, unterstützen das Löschen offener Erweiterungen daraus in einer ähnlichen Weise.


## <a name="path-parameters"></a>Pfadparameter
|**Parameter**|**Typ**|**Beschreibung**|
|:-----|:-----|:-----|
|Id|string|Platzhalter für einen eindeutigen Bezeichner eines Objekts in der entsprechenden Sammlung, z. B. einer Nachricht, eines Ereignisses oder eines Kontakts. Erforderlich. Nicht zu verwechseln mit der **id**-Eigenschaft einer **openTypeExtension**.|
|extensionId|string|Platzhalter für einen Erweiterungsnamen. Ein Erweiterungsname ist der eindeutige Textbezeichner einer Erweiterung oder ein vollqualifizierter Name, der den Erweiterungstyp und den eindeutigen Textbezeichner verkettet. Der vollqualifizierte Name wird beim Erstellen der Erweiterung in der Eigenschaft **id** zurückgegeben. Erforderlich.|

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter

Stellen Sie sicher, dass Sie für die Leerzeichen in der `$filter`-Zeichenfolge die [URL-Codierung](https://www.w3schools.com/tags/ref_urlencode.asp) verwenden.

|**Name**|**Wert**|**Beschreibung**|
|:---------------|:--------|:-------|
|$filter|string|Gibt Erweiterungen zurück, deren **id** dem Wert des Parameters `extensionId` entspricht.|
|$filter with **any** operator|string|Gibt Instanzen einer Ressourcensammlung zurück, die eine Erweiterung enthalten, deren **id** dem Wert des Parameters `extensionId` entspricht.|
|$expand|string|Erweitert eine Ressourceninstanz um eine Erweiterung. |

## <a name="request-headers"></a>Anforderungsheader
| Name       | Wert |
|:---------------|:----------|
| Authorization | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wird diese Methode erfolgreich ausgeführt, gibt Sie den Antwortcode `200 OK` und ein [openTypeExtension](../resources/opentypeextension.md)-Objekt im Antworttext zurück. Der genaue Antworttext ist je nach GET-Abfrage unterschiedlich.
## <a name="example"></a>Beispiel

#### <a name="request-1"></a>Anforderung 1

Das erste Beispiel zeigt 2 Möglichkeiten zur Referenzierung einer Erweiterung und ruft die Erweiterung in der angegebenen Nachricht ab. Es wird unabhängig von der zur Referenzierung der Erweiterung verwendeten Methode jeweils die gleiche Antwort zurückgegeben.

Die erste Möglichkeit ist der Abruf mithilfe des Namens: 

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_1"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Com.Contoso.Referral')
```

Die zweite Möglichkeit ist der Abruf mithilfe der ID (vollqualifizierter Name):

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')
```

#### <a name="response-1"></a>Antwort 1
Hier sehen Sie die Antwort für Beispiel 1:
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00Z"
}
```

****


#### <a name="request-2"></a>Anforderung 2

Das zweite Beispiel referenziert eine Erweiterung über ihren Namen und ruft die Erweiterung im angegebenen Gruppenereignis ab.

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_2"
}-->
```http
GET https://graph.microsoft.com/beta/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl17IsAAA=')/extensions('Com.Contoso.Deal') 
```

#### <a name="response-2"></a>Antwort 2

Die Antwort für das zweite Beispiel sieht so aus:

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl7IsAAA%3D')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```

****

#### <a name="request-3"></a>Anforderung 3

Im dritten Beispiel wird die angegebene Nachricht abgerufen und um eine von einem Filter zurückgegebene Erweiterung erweitert. Der Filter gibt die Erweiterung zurück, deren **id** dem angegebenen vollqualifizierten Namen entspricht.

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_3"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')?$expand=extensions($filter=id%20eq%20'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')
```


#### <a name="response-3"></a>Antwort 3

Unten sehen Sie die Antwort für das dritte Beispiel. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.

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
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM\"",
    "id": "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===",
    "changeKey": "CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM",
    "categories": [
    ],
    "createDateTime": "2015-06-19T02:03:31Z",
    "lastModifiedDateTime": "2015-08-13T02:28:00Z",
    "subject": "Attached is the requested info",
    "bodyPreview": "See the images attached.",
    "body": {
        "contentType": "HTML",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<style type=\"text/css\" style=\"display:none;\"><!-- P {margin-top:0;margin-bottom:0;} --></style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" style=\"font-size:12pt;color:#000000;background-color:#FFFFFF;font-family:Calibri,Arial,Helvetica,sans-serif;\">\r\n<p>See the images attached. <br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "importance": "Normal",
    "hasAttachments": true,
    "parentFolderId": "AQMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===QAAAA==",
    "from": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "sender": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "address": "wendy@contoso.com",
                "name": "Wendy Molina"
            }
        }
    ],
    "ccRecipients": [
    ],
    "bccRecipients": [
    ],
    "replyTo": [
    ],
    "conversationId": "AAQkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===mivdTmQ=",
    "receivedDateTime": "2015-06-19T02:05:04Z",
    "sentDateTime": "2015-06-19T02:04:59Z",
    "isDeliveryReceiptRequested": false,
    "isReadReceiptRequested": false,
    "isDraft": false,
    "isRead": true,
    "webLink": "https://outlook.office.com/owa/?ItemID=AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===%2FNJTqt5NqHlVnKVBwCY4MQpaFz9SbqUDe4%2Bbs88AAAAAAEJAACY4MQpaFz9SbqUDe4%2Bbs88AAApA4JMAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "Focused",
    "extensions@odata.context": "https://graph.microsoft.com/beta/$metadata#users('desmond40contoso.com')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions", 
    "extensions": [ 
      { 
        "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
        "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
        "extensionName": "Com.Contoso.Referral",
        "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
        "companyName": "Wingtip Toys",
        "dealValue": 500050,
        "expirationDate": "2015-12-03T10:00:00Z"
      }
     ]
}
```

****

#### <a name="request-4"></a>Anforderung 4

Das vierte Beispiel referenziert eine Erweiterung über ihren vollqualifizierten Namen und ruft die Erweiterung im angegebenen Gruppenbeitrag ab.

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_4"
}-->
```http
GET https://graph.microsoft.com/beta/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA==')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate') 
```

#### <a name="response-4"></a>Antwort 4

Die Antwort für das vierte Beispiel sieht wie folgt aus: 

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate",
    "extensionName": "Com.Contoso.Estimate",
    "companyName": "Contoso",
    "expirationDate": "2015-07-03T13:04:00Z",
    "Strings@odata.type": "#Collection(String)",
    "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
    ]
}
```


#### <a name="request-5"></a>Anforderung 5

Das fünfte Beispiel sucht unter allen Nachrichten im Postfach des angemeldeten Benutzers diejenigen mit einer Erweiterung, die dem definierten Filter entspricht. Anschließend werden die Nachrichten um die Erweiterung erweitert. Der Filter gibt Erweiterungen zurück, deren **id**-Eigenschaft dem Erweiterungsnamen `Com.Contoso.Referral` entspricht.

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_5"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=Extensions/any(f:f/id%20eq%20'Com.Contoso.Referral')&$expand=Extensions($filter=id%20eq%20'Com.Contoso.Referral')
```


####<a name="response-5"></a>Antwort 5

In der Antwort aus Beispiel 5 gibt es im Postfach des Benutzers nur eine Nachricht mit einer Erweiterung, deren **id** `Com.Contoso.Referral` entspricht.

Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages",
  "value": [
  {

    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM\"",
    "id": "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===",
    "changeKey": "CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM",
    "categories": [
    ],
    "createDateTime": "2015-06-19T02:03:31Z",
    "lastModifiedDateTime": "2015-08-13T02:28:00Z",
    "subject": "Attached is the requested info",
    "bodyPreview": "See the images attached.",
    "body": {
        "contentType": "HTML",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<style type=\"text/css\" style=\"display:none;\"><!-- P {margin-top:0;margin-bottom:0;} --></style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" style=\"font-size:12pt;color:#000000;background-color:#FFFFFF;font-family:Calibri,Arial,Helvetica,sans-serif;\">\r\n<p>See the images attached. <br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "importance": "Normal",
    "hasAttachments": true,
    "parentFolderId": "AQMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===QAAAA==",
    "from": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "sender": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "address": "wendy@contoso.com",
                "name": "Wendy Molina"
            }
        }
    ],
    "ccRecipients": [
    ],
    "bccRecipients": [
    ],
    "replyTo": [
    ],
    "conversationId": "AAQkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===mivdTmQ=",
    "receivedDateTime": "2015-06-19T02:05:04Z",
    "sentDateTime": "2015-06-19T02:04:59Z",
    "isDeliveryReceiptRequested": false,
    "isReadReceiptRequested": false,
    "isDraft": false,
    "isRead": true,
    "webLink": "https://outlook.office.com/owa/?ItemID=AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===%2FNJTqt5NqHlVnKVBwCY4MQpaFz9SbqUDe4%2Bbs88AAAAAAEJAACY4MQpaFz9SbqUDe4%2Bbs88AAApA4JMAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "Focused",
    "extensions@odata.context": "https://graph.microsoft.com/beta/$metadata#users('desmond40contoso.com')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions", 
    "extensions": [ 
      { 
        "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
        "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
        "extensionName": "Com.Contoso.Referral",
        "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
        "companyName": "Wingtip Toys",
        "dealValue": 500050,
        "expirationDate": "2015-12-03T10:00:00Z"
      }
     ]
  }
  ]
}

```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get openTypeExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
