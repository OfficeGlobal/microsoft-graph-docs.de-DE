---
title: Regel erstellen
description: 'Erstellen Sie ein  messageRule-Objekt, indem Sie eine Gruppe von Bedingungen und Aktionen angeben. '
ms.openlocfilehash: f725aa0a078938cf111782aedf1feb041a5a0e19
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065899"
---
# <a name="create-rule"></a>Regel erstellen

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Erstellen Sie ein  [messageRule](../resources/messagerule.md)-Objekt, indem Sie eine Gruppe von Bedingungen und Aktionen angeben. 

Outlook führt diese Aktionen aus, wenn eine eingehende Nachricht im Posteingang des Benutzers die angegebenen Bedingungen erfüllt.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | MailboxSettings.ReadWrite    |
|Delegiert (persönliches Microsoft-Konto) | MailboxSettings.ReadWrite    |
|Anwendung | MailboxSettings.ReadWrite |


## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messagerules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messagerules
```
## <a name="request-headers"></a>Anforderungsheader
| Name       | Beschreibung|
|:---------------|:----------|
| Authorization  | Bearer {token}. Erforderlich. |


## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext die Parameter an, die auf die Regel angewendet werden können. Nachfolgend finden Sie die Textparameter, die in der Regel beim Erstellen von Regeln verwendet werden. Sie können bei Bedarf im Anforderungstext beliebige andere schreibbare **messageRule**-Eigenschaften angeben.

| Parameter       | Typ|Beschreibung|
|:--------|:-------|:----------|
|Aktionen|[messageRuleActions](../resources/messageruleactions.md)|Aktionen, die auf eine Nachricht angewendet werden, wenn die entsprechenden Bedingungen (falls vorhanden) erfüllt sind. Erforderlich. |
|Bedingungen|[messageRulePredicates](../resources/messagerulepredicates.md)|Bedingungen, die bei Erfüllung die entsprechenden Aktionen für diese Regel auslösen. Optional.|
|displayName| Zeichenfolge  | Der Anzeigename der Regel. Erforderlich. |
|Ausnahmen| [messageRulePredicates](../resources/messagerulepredicates.md)| Ausnahmebedingungen für die Regel. Optional. |
|isEnabled | Boolescher Wert | Gibt an, ob die Regel auf Nachrichten angewendet werden kann. Optional. |
|sequence| Int32 | Gibt die Reihenfolge an, in der die Regel zusammen mit anderen Regeln ausgeführt wird. Erforderlich. |

## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs **messageRule** im Antworttext zurück.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "create_messagerule_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/mailFolders/inbox/messagerules
Content-type: application/json

{      
    "displayName": "From partner",      
    "sequence": 2,      
    "isEnabled": true,          
    "conditions": {
        "senderContains": [
          "adele"       
        ]
     },
     "actions": {
        "forwardTo": [
          {
             "emailAddress": {
                "name": "Alex Wilbur",
                "address": "AlexW@contoso.onmicrosoft.com"
              }
           }
        ],
        "stopProcessingRules": true
     }    
}

```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id":"AQAAAJ5dZqA=",
  "displayName":"From partner",
  "sequence":2,
  "isEnabled":true,
  "hasError":false,
  "isReadOnly":false,
  "conditions":{
    "senderContains":[
      "ADELE"
    ]
  },
  "actions":{
      "stopProcessingRules":true,
      "forwardTo":[
        {
          "emailAddress":{
            "name":"Alex Wilbur",
            "address":"AlexW@contoso.onmicrosoft.com"
          }
        }
      ]
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->