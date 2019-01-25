---
title: Liste der Registerkarten im Kanal
description: 'Rufen Sie die Liste der Registerkarten in den angegebenen Kanal innerhalb eines Teams ab. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b2af784eaaf22217e9e96769c106dfc49de74a2a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519514"
---
# <a name="list-tabs-in-channel"></a>Liste der Registerkarten im Kanal

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Rufen Sie die Liste der [Registerkarten](../resources/teamstab.md) in den angegebenen [DDE-Kanal](../resources/channel.md) in einem [Team](../resources/team.md)ab. 

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Group.ReadWrite.All, Group.Read.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
| Anwendung                            | Group.Read.All, Group.ReadWrite.All         |

> **Hinweis**: Diese API unterstützt Administratorberechtigungen. Globale Administratoren und Microsoft-Teams Dienstadministratoren können Teams zugreifen, denen sie nicht Mitglied sind.

## <a name="http-request"></a>HTTP-Anforderung

```http
GET /teams/{id}/channels/{id}/tabs
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter

Diese Methode unterstützt die $filter $select, und $erweitern [OData-Abfrageparameter](/graph/query-parameters) helfen, die Antwort anzupassen.

## <a name="request-headers"></a>Anforderungsheader
| Kopfzeile       | Wert |
|:---------------|:--------|
| Authorization  | Bearer {token}. Erforderlich.  |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort
Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [Registerkarten](../resources/teamstab.md) .

## <a name="example"></a>Beispiel
#### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs
```

#### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort.
>**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.
```http
HTTP/1.1 200 Success
Content-type: application/json

{
  "value": [
    {
      "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
      "name": "My Contoso Tab - updated",
      "teamsAppId": "06805b9e-77e3-4b93-ac81-525eb87513b8",
      "configuration": {
        "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
        "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
        "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
        "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
      },
      "sortOrderIndex": 20,
      "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
    },
    {
      "id": "b5d5f001-0471-49a5-aac4-04ef96683be0",
      "name": "My Trello Tab",
      "teamsAppId": "23134c6b-5e4b-439c-8f70-3ded1df20805",
      "configuration": null,
      "sortOrderIndex": 21,
      "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3a3709b35c-a0ba-467c-8001-0f66895fb9d3?label=My%20Trello%Tab"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List all tabs in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/teamstab-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
