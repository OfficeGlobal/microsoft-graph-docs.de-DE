---
title: Aktualisieren von groupLifecyclePolicy
description: Aktualisieren Sie die Eigenschaften eines groupLifecyclePolicygroupLifecyclePolicy-Ressourcentyp-Objekts.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 69073693203981debbfa8010468df271ea65cef3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512080"
---
# <a name="update-grouplifecyclepolicy"></a>Aktualisieren von groupLifecyclePolicy

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Aktualisieren Sie die Eigenschaften eines groupLifecyclePolicy[groupLifecyclePolicy-Ressourcentyp](../resources/grouplifecyclepolicy.md)-Objekts.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).
 

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Directory.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt |
|Anwendung | Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
PATCH /groupLifecyclePolicies/{id}
```
## <a name="optional-request-headers"></a>Optionale Anforderungsheader
| Name | Beschreibung |
|:-----------|:-----------|
| Authorization | Bearer {token}. Erforderlich. |
| Content-Type  | application/json  |

## <a name="request-body"></a>Anforderungstext

Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.

| Eigenschaft | Typ | Beschreibung |
|:---------------|:--------|:----------|
|alternateNotificationEmails|Zeichenfolge| Liste der E-Mail-Adressen, an die Benachrichtigungen für Gruppen ohne Besitzer gesendet werden sollen. Mehrere E-Mail-Adressen können durch ein Semikolon voneinander getrennt definiert werden. |
|groupLifetimeInDays|Int32| Anzahl von Tagen, bis eine Gruppe abläuft und verlängert werden muss. Sobald die Gruppe verlängert wurde, wird der Ablaufzeitraum für die Gruppe um die Anzahl der definierten Tage verlängert. |
|managedGroupTypes|Zeichenfolge| Der Gruppentyp, für den die Ablaufrichtlinie gilt. Mögliche Werte sind **Alle**, **Ausgewählte** oder **Keine**. |

## <a name="response"></a>Antwort

Wenn erfolgreich ausgeführt, gibt diese Methode den Antwortcode `200 OK` und ein aktualisiertes [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)-Objekt im Antworttext zurück.
## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

<!-- {
  "blockType": "request",
  "name": "update_grouplifecyclepolicy"
}-->
```http
PATCH https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
Content-type: application/json
Content-length: 151

{
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
##### <a name="response"></a>Antwort
Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "id": "id-value",
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/grouplifecyclepolicy-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
