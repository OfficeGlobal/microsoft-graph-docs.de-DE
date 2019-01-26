---
title: Ressourcentyp parentalControlSettings
description: Gibt die Altersfreigabe Einstellungen für eine Anwendung. Diese Einstellungen Steuern der Zustimmung wünschen.
localization_priority: Normal
ms.openlocfilehash: 8a3a768cc9264b6d1a25532455da20d87a5bc4e8
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573872"
---
# <a name="parentalcontrolsettings-resource-type"></a>Ressourcentyp parentalControlSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Gibt die Altersfreigabe Einstellungen für eine Anwendung. Diese Einstellungen Steuern der Zustimmung wünschen.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
:---------------|:--------|:----------|
|countriesBlockedForMinors|Zeichenfolgenauflistung| Gibt die [zwei Buchstaben ISO-Ländercodes](https://www.iso.org/iso-3166-country-codes.html). Zugriff auf die Anwendung werden für Minderjährige aus den in dieser Liste angegebenen Ländern blockiert.|
|legalAgeGroupRule| String | Gibt die ALTER Legal Gruppenregel, die für Benutzer der app gilt. Kann auf einen der folgenden Werte festgelegt werden: <table><tr><th>Wert</th><th>Beschreibung</th></tr><tr><td>Allow</td><td>Standard. Erzwingt die rechtliche minimale. Dies bedeutet, dass die Zustimmung der Eltern für Minderjährige in der Europäischen Union und Korea erforderlich ist.</td></tr><tr><td>RequireConsentForPrivacyServices</td><td>Erzwingt den Benutzer zum Angeben von Geburtsdatum COPPA-Regeln einhalten. </td></tr><tr><td>RequireConsentForMinors</td><td>Erfordert Zustimmung der Eltern für Jahren unter 18, unabhängig davon Land minor Regeln.</td></tr><tr><td>RequireConsentForKids</td><td>Erfordert Zustimmung der Eltern für Jahren unter 14, unabhängig davon Land minor Regeln.</td></tr><tr><td>BlockMinors</td><td>Blöcke Minderjährige aus mithilfe der app.</td></tr></table> |

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- 
{
    "blockType": "resource",
    "@odata.type":"microsoft.graph.parentalControlSettings"
}
-->
```json
{
  "countriesBlockedForMinors": [ "String" ],
  "legalAgeGroupRule": "String"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/parentalcontrolsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
