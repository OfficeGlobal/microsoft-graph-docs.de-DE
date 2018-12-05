---
title: Datenerweiterung erstellen
description: Erstellen Sie eine open-Erweiterung (OpenTypeExtension-Objekt) und Hinzufügen von benutzerdefinierten Eigenschaften
ms.openlocfilehash: 80747559d310f033419fe3b24add1dc27debb90e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062439"
---
# <a name="create-open-extension"></a>Datenerweiterung erstellen

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Erstellen Sie eine open-Erweiterung ([OpenTypeExtension](../resources/opentypeextension.md) -Objekt) und fügen Sie benutzerdefinierte Eigenschaften in einer neuen oder vorhandenen Instanz einer unterstützten Ressource hinzu.

> **Hinweis:** Wenn beim Erstellen von open Extensions auf Outlook-Ressourcen finden Sie in [OpenTypeExtension Ressourcentyp](../resources/opentypeextension.md#outlook-specific-considerations) **Outlook-spezifischen Aspekte** .

## <a name="permissions"></a>Berechtigungen

Je nach der Ressource, die Sie die Erweiterung im erstellen und die Berechtigung Typ (delegierte oder-Anwendung) angefordert, die Berechtigung, die in der folgenden Tabelle angegebenen mit den geringsten ist erforderlich, um diese API aufzurufen. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).

| Unterstützte Ressource | Delegiert (Geschäfts-, Schul- oder Unikonto) | Delegiert (persönliches Microsoft-Konto) | Anwendung |
|:-----|:-----|:-----|:-----|
| [Gerät](../resources/device.md) | Directory.AccessAsUser.All | Nicht unterstützt | Device.ReadWrite.All |
| [event](../resources/event.md) | Calendars.ReadWrite | Calendars.ReadWrite | Calendars.ReadWrite |
| [group](../resources/group.md) | Group.ReadWrite.All | Nicht unterstützt | Group.ReadWrite.All |
| [group event](../resources/event.md) | Group.ReadWrite.All | Nicht unterstützt | Nicht unterstützt |
| [group post](../resources/post.md) | Group.ReadWrite.All | Nicht unterstützt | Group.ReadWrite.All |
| [message](../resources/message.md) | Mail.ReadWrite | Mail.ReadWrite | Mail.ReadWrite | 
| [organization](../resources/organization.md) | Directory.AccessAsUser.All | Nicht unterstützt | Nicht unterstützt |
| [personal contact](../resources/contact.md) | Contacts.ReadWrite | Contacts.ReadWrite | Contacts.ReadWrite |
| [user](../resources/user.md) | User.ReadWrite.All | User.ReadWrite | User.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

### <a name="create-an-extension-in-a-new-resource-instance"></a>Erstellen einer Erweiterung in einer neuen Ressourceninstanz

Verwenden Sie die gleiche REST-Anforderung, die Sie verwenden, um die Instanz zu erstellen.

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/events
POST /users/{id|userPrincipalName}/messages
POST /groups/{id}/events
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /users/{id|userPrincipalName}/contacts
```

>**Hinweis:** Diese Syntax enthält einige allgemeinen Bereitstellungsmethoden für die Ressourceninstanzen unterstützte zu erstellen. Andere POST-Syntax, die Sie erstellen diese Ressourceninstanzen können unterstützt erstellen open Erweiterungen in diese auf ähnliche Weise.

Im Abschnitt [Anforderungstext](#request-body) ist beschrieben, wie Sie die Eigenschaften der neuen Ressourceninstanz _und die Erweiterung_ in den Anforderungstext einschließen können.

### <a name="create-an-extension-in-an-existing-resource-instance"></a>Erstellen einer Erweiterung in einer vorhandenen Ressourceninstanz

Geben Sie die Ressourceninstanz in der Anforderung an, und wenden Sie den Befehl `POST` auf die Navigationseigenschaft **extensions** an.

<!-- { "blockType": "ignored" } -->
```http
POST /administrativeunits/{id}/extensions
POST /devices/{id}/extensions
POST /users/{id|userPrincipalName}/events/{id}/extensions
POST /groups/{id}/extensions
POST /groups/{id}/events/{id}/extensions
POST /groups/{id}/threads/{id}/posts/{id}/extensions
POST /users/{id|userPrincipalName}/messages/{id}/extensions
POST /organization/{id}/extensions
POST /users/{id|userPrincipalName}/contacts/{id}/extensions
POST /users/{id|userPrincipalName}/extensions
```

>**Hinweis:** Diese Syntax enthält einige allgemeinen Bereitstellungsmethoden für eine Ressourceninstanz identifizieren, um eine Erweiterung in es zu erstellen. Alle anderen Syntax, die Ihnen ermöglicht, diese Ressourceninstanzen identifizieren unterstützt das Erstellen von open Extensions darin auf ähnliche Weise.

Im Abschnitt [Anforderungstext](#request-body) wird beschrieben, wie Sie _die Erweiterung_ in den Anforderungstext einschließen können.

## <a name="path-parameters"></a>Pfadparameter

|**Parameter**|**Typ**|**Beschreibung**|
|:-----|:-----|:-----|
|id|string|Ein eindeutiger Bezeichner für ein Objekt in der entsprechenden Sammlung. Erforderlich.|

## <a name="request-headers"></a>Anforderungsheader

| Name       | Wert |
|:---------------|:----------|
| Authorization | Bearer {token}. Erforderlich. |
| Content-Type | application/json |

## <a name="request-body"></a>Anforderungstext

Bieten Sie ein JSON-Hauptteil eines [OpenTypeExtension](../resources/opentypeextension.md)die folgenden erforderlichen Name / Wert-Paare und zusätzlichen benutzerdefinierten Daten. Die Daten in der JSON-Nutzlast möglich Grundtypen oder Arrays von Grundtypen.

| Name       | Wert |
|:---------------|:----------|
| @odata.type | Microsoft.Graph.OpenTypeExtension |
| extensionName | %unique_string% |

Beim Erstellen einer Erweiterung in einer _neuen_ Ressourceninstanz müssen Sie zusätzlich zu dem neuen **openTypeExtension**-Objekt eine JSON-Darstellung der zur Erstellung einer solchen Ressourceninstanz erforderlichen Eigenschaften angeben.

## <a name="response"></a>Antwort

### <a name="response-code"></a>Antwortcode

Je nach Vorgang lautet der Antwortcode `201 Created` oder `202 Accepted`.

Beim Erstellen einer Erweiterungs mit den gleichen Vorgang, mit denen Sie eine Ressourceninstanz zu erstellen, gibt der Vorgang den gleichen Antwortcode, den es zurückgibt, wenn Sie den Vorgang zum Erstellen der Ressourceninstanz ohne die Erweiterung verwenden.
Finden Sie in den entsprechenden Themen für die Instanz als aufgeführten [oben](#create-an-extension-in-a-new-resource-instance)zu erstellen.

### <a name="response-body"></a>Antworttext

| Szenario       | Ressource  | Antworttext |
|:---------------|:----------|:--------------|
| Erstellen einer Erweiterung bei gleichzeitiger expliziter Erstellung einer _neuen_ Ressourceninstanz | [contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md) | Enthält die neue Instanz, erweitert um das [openTypeExtension](../resources/opentypeextension.md)-Objekt. |
| Erstellen einer Erweiterung bei gleichzeitiger impliziter Erstellung einer Ressourceninstanz | [post](../resources/post.md) | Die Antwort enthält nur einen Antwortcode, keinen Antworttext. |
| Erstellen einer Erweiterung in einer _vorhandenen_ Ressourceninstanz | Alle unterstützten Ressourcen | Enthält das **openTypeExtension**-Objekt. |

## <a name="example"></a>Beispiel

### <a name="request-1"></a>Anforderung 1

Im ersten Beispiel werden mit ein und demselben Aufruf eine Nachricht und eine Erweiterung erstellt. Der Anforderungstext enthält Folgendes:

- Die für eine neue Nachricht typischen Eigenschaften **subject**, **body** und **toRecipients**
- Daneben die folgenden Parameter der Erweiterung:

  - Den Typ `Microsoft.Graph.OpenTypeExtension`
  - Den Erweiterungsnamen „Com.Contoso.Referral“
  - Zusätzliche Daten, die als drei benutzerdefinierte Eigenschaften in der JSON-Nutzlast gespeichert werden: `companyName`, `expirationDate`, und `dealValue`.

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_1"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages

{
  "subject": "Annual review",
  "body": {
    "contentType": "HTML",
    "content": "You should be proud!"
  },
  "toRecipients": [
    {
      "emailAddress": {
        "address": "rufus@contoso.com"
      }
    }
  ],
  "extensions": [
    {
      "@odata.type": "Microsoft.Graph.OpenTypeExtension",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

### <a name="response-1"></a>Antwort 1

Unten sehen Sie die Antwort für Beispiel 1. Der Antworttext enthält die Eigenschaften der neuen Nachricht sowie die folgenden Parameter der neuen Erweiterung:

- Die Eigenschaft **id** mit dem vollqualifizierten Namen `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`
- Die in der Anforderung angegebene Standardeigenschaft **extensionName**
- Die in der Anforderung angegebenen benutzerdefinierten Daten, gespeichert als 3 benutzerdefinierte Eigenschaften

Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')",
  "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AAB88LOj\"",
  "id": "AAMkAGEbs88AAB84uLuAAA=",
  "createdDateTime": "2015-10-30T03:03:43Z",
  "lastModifiedDateTime": "2015-10-30T03:03:43Z",
  "changeKey": "CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AAB88LOj",
  "categories": [ ],
  "receivedDateTime": "2015-10-30T03:03:43Z",
  "sentDateTime": "2015-10-30T03:03:43Z",
  "hasAttachments": false,
  "subject": "Annual review",
  "body": {
    "contentType": "HTML",
    "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r
\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nYou should be proud!\r\n</body>\r
\n</html>\r\n"
  },
  "bodyPreview": "You should be proud!",
  "importance": "Normal",
  "parentFolderId": "AQMkAGEwAAAIBDwAAAA==",
  "sender": null,
  "from": null,
  "toRecipients": [
    {
      "emailAddress": {
        "address": "rufus@contoso.com",
        "name": "John Doe"
      }
    }
  ],
  "ccRecipients": [ ],
  "bccRecipients": [ ],
  "replyTo": [ ],
  "conversationId": "AAQkAGEFGugh3SVdMzzc=",
  "isDeliveryReceiptRequested": false,
  "isReadReceiptRequested": false,
  "isRead": true,
  "isDraft": true,
  "webLink": "https://outlook.office.com/owa/?
ItemID=AAMkAGEbs88AAB84uLuAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
  "inferenceClassification": "Focused",
  "extensions@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages
('AAMkAGEbs88AAB84uLuAAA%3D')/extensions",
  "extensions": [
    {
      "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
      "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
      "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

****

### <a name="request-2"></a>Anforderung 2

Das zweite Beispiel erstellt eine Erweiterung in der angegebenen Nachricht. Der Anforderungstext enthält die folgenden Parameter für die Erweiterung:

- Den Typ `Microsoft.Graph.OpenTypeExtension`
- Den Erweiterungsnamen „Com.Contoso.Referral“
- Zusätzliche Daten, die als 3 benutzerdefinierte Eigenschaften in der JSON-Nutzlast gespeichert werden sollen: `companyName`, `dealValue` und `expirationDate`

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_2"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions

{
  "@odata.type" : "Microsoft.Graph.OpenTypeExtension",
  "extensionName" : "Com.Contoso.Referral",
  "companyName" : "Wingtip Toys",
  "dealValue" : 500050,
  "expirationDate" : "2015-12-03T10:00:00.000Z"
}
```

### <a name="response-2"></a>Antwort 2

Die Antwort für das zweite Beispiel sehen Sie unten. Der Antworttext enthält die folgenden Parameter für die neue Erweiterung:

- Die Standardeigenschaft **extensionName**
- Die Eigenschaft **id** mit dem vollqualifizierten Namen `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`
- Die benutzerdefinierten Daten, die gespeichert werden sollen

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 201 Created
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
    "expirationDate": "2015-12-03T10:00:00.000Z"
}
```

****

### <a name="request-3"></a>Anforderung 3

Das dritte Beispiel erstellt eine Erweiterung in dem angegebenen Gruppenereignis. Der Anforderungstext enthält die folgenden Parameter für die Erweiterung:

- Den Typ `Microsoft.Graph.OpenTypeExtension`
- Den Erweiterungsnamen „Com.Contoso.Deal“
- Zusätzliche Daten, die als 3 benutzerdefinierte Eigenschaften in der JSON-Nutzlast gespeichert werden sollen: `companyName`, `dealValue` und `expirationDate`

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_3"
}-->
```http
POST https://graph.microsoft.com/beta/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl17IsAAA=')/extensions

{
  "@odata.type" : "Microsoft.Graph.OpenTypeExtension",
  "extensionName" : "Com.Contoso.Deal",
  "companyName" : "Alpine Skis",
  "dealValue" : 1010100,
  "expirationDate" : "2015-07-03T13:04:00.000Z"
}
```

### <a name="response-3"></a>Antwort 3

Unten sehen Sie die Antwort auf die Anforderung im dritten Beispiel:

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 201 Created
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

### <a name="request-4"></a>Anforderung 4

Das vierte Beispiel erstellt eine Erweiterung in einem neuen Gruppenbeitrag, mit demselben **reply**-Aktionsaufruf, wie er für bereits vorhandene Gruppenbeiträge verwendet wird. Die Aktion **reply** erstellt einen neuen Beitrag und eine neue, in diesen Beitrag eingebettete Erweiterung. Der Antworttext enthält eine Eigenschaft **post** mit dem **Text** des neuen Beitrags sowie die folgenden Daten der neuen Erweiterung:

- Den Typ `Microsoft.Graph.OpenTypeExtension`
- Den Erweiterungsnamen „Com.Contoso.HR“
- Zusätzliche Daten, die als 3 benutzerdefinierte Eigenschaften in der JSON-Nutzlast gespeichert werden sollen: `companyName`, `expirationDate` und das Zeichenfolgen-Array `topPicks`

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_4"
}-->
```http
POST https://graph.microsoft.com/beta/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA==')/posts('AAMkADJiUg96QZUkA-ICwMubAAC1heiSAAA=')/reply

{
  "post": {
    "body": {
      "contentType": "html",
      "content": "<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>"
    },
  "extensions": [
    {
      "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
      "extensionName": "Com.Contoso.HR",
      "companyName": "Contoso",
      "expirationDate": "2015-07-03T13:04:00.000Z",
      "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
      ]
    }
  ]
  }
}
```

### <a name="response-4"></a>Antwort 4

Die Antwort für das vierte Beispiel sehen Sie unten. Wird eine Erweiterung in einem neuen Gruppenbeitrag erstellt, wird nur der Antwortcode „HTTP 202“ zurückgegeben.

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
Content-type: text/plain
Content-Length: 0
```

****

### <a name="request-5"></a>Anforderung 5

Das fünfte Beispiel erstellt in ein und derselben POST-Operation eine Erweiterung in einem neuen Gruppenbeitrag und eine Unterhaltung. Die POST-Operation erstellt eine neue Unterhaltung, einen neuen Thread, einen neuen Beitrag und eine neue, in diesen Beitrag eingebettete Erweiterung. Der Anforderungstext enthält die Eigenschaften **Topic** und **Threads** sowie ein untergeordnetes Objekt des Typs **post** der neuen Unterhaltung. Das **post**-Objekt wiederum enthält den **Text** des neuen Beitrags sowie die folgenden Daten der Erweiterung:

- Den Typ `Microsoft.Graph.OpenTypeExtension`
- Den Erweiterungsnamen „Com.Contoso.HR“
- Zusätzliche Daten, die als 3 benutzerdefinierte Eigenschaften in der JSON-Nutzlast gespeichert werden sollen: `companyName`, `expirationDate` und das Zeichenfolgen-Array `topPicks`

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_5"
}-->
```http
POST https://graph.microsoft.com/beta/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations

{
  "Topic": "Does anyone have a second?",
  "Threads": [
    {
      "Posts": [
        {
          "Body": {
            "ContentType": "HTML",
            "Content": "This is urgent!"
          },
          "Extensions": [
            {
              "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
              "extensionName": "Com.Contoso.Benefits",
              "companyName": "Contoso",
              "expirationDate": "2016-08-03T11:00:00.000Z",
              "topPicks": [
                "Employees only",
                "Add spouse or guest",
                "Add family"
              ]
            }
          ]
        }
      ]
    }
  ]
}
```

### <a name="response-5"></a>Antwort 5

Unten sehen Sie die Antwort für das fünfte Beispiel mit der neuen Unterhaltung und einer Thread-ID. Dieser neue Thread enthält einen automatisch erstellten Beitrag, der wiederum die neue Erweiterung enthält.

Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.

Zum Abrufen der neuen Erweiterung [rufen Sie zunächst alle Beiträge](../api/conversationthread-list-posts.md) in diesem Thread ab. Anfangs sollte es nur einen Beitrag geben. Wenden Sie dann die Beitrags-ID und den Erweiterungsnamen `Com.Contoso.Benefits` an, um [die Erweiterung abzurufen](../api/opentypeextension-get.md).

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations/$entity",
    "id": "AAQkADJToRlbJ5Mg7TFM7H-j3Y=",
    "threads@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations('AAQkADJToRlbJ5Mg7TFM7H-j3Y%3D')/threads",
    "threads": [
        {
            "id": "AAQkADJDtMUzsf_PdhAAswJOhGVsnkyDtMUzsf_Pdg=="
        }
    ]
}

```

<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create extension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->