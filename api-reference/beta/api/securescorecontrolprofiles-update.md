---
title: Update secureScoreControlProfiles
description: Aktualisieren einer bearbeitbaren SecureScoreControlProfiles-Eigenschaft in eine integrierte Lösung verschiedene Eigenschaften, wie AssignedTo oder TenantNote ändern.
localization_priority: Normal
ms.openlocfilehash: 711fd29e906822def0a5f4b5fbca13a1d73732d6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510953"
---
# <a name="update-securescorecontrolprofiles"></a>Update secureScoreControlProfiles

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Aktualisieren einer bearbeitbaren **SecureScoreControlProfiles** -Eigenschaft in eine integrierte Lösung verschiedene Eigenschaften, wie **AssignedTo** oder **TenantNote**ändern.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) |   SecurityEvents.ReadWrite.All  |
|Delegiert (persönliches Microsoft-Konto) |  Nicht unterstützt  |
|Anwendung | SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a>Anforderungsheader

| Name       | Beschreibung|
|:-----------|:-----------|
| Authorization  | Bearer {code}. Erforderlich.|
|Prefer | zurückgeben = Darstellung. |

## <a name="request-body"></a>Anforderungstext

Geben Sie im Textkörper Anforderung eine JSON-Darstellung der Werte für die entsprechenden Felder, die aktualisiert werden soll. In der folgenden Tabelle werden die Felder, die für eine SecureScoreControlProfile aktualisiert werden können. Die Werte für vorhandene Eigenschaften, die nicht im Textkörper Anforderung enthalten sind, werden nicht geändert. Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.

| Eigenschaft   | Typ |Beschreibung|
|:---------------|:--------|:----------|
|assignedTo|String|Name des der Analyst das Steuerelement wird für die Ursachenanalyse, Implementierung und-Wartung zugewiesen.|
|tenantNote|String|Analyst von Kommentaren auf das Steuerelement (für Kunden Steuerelement Management).|
|controlStateUpdates| String|Analyst gesteuerte Einstellung für das Steuerelement. Mögliche Werte sind: `ignore`, `thirdParty` und `reviewed`.|


## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.

Wenn der optionale Anforderungsheader verwendet wird, gibt die Methode eine `200 OK` Antwortcode und der aktualisierten [SecureScoreControlProfiles](../resources/securescorecontrolprofiles.md) -Objekts in der Antworttext.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/secureScoreControlProfiles/AdminMFA
Content-type: application/json

{
  "assignedTo": "assignedTo-value",
  "controlStateUpdates": "controlStateUpdates-value",
  "tenantNote": "tenantNote-value"
}
```

### <a name="response"></a>Antwort

Es folgt ein Beispiel für eine erfolgreiche Antwort.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
} -->

```http
HTTP/1.1 204 No Content
```




<!--
{
  "type": "#page.annotation",
  "description": "Update secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/securescorecontrolprofiles-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
