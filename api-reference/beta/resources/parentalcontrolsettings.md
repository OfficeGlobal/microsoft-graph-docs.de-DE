---
title: Ressourcentyp parentalControlSettings
description: Gibt die Jugendschutzeinstellungen für eine Anwendung an. Diese Einstellungen Steuern der Zustimmung wünschen.
localization_priority: Normal
ms.openlocfilehash: 52a808cd4c3e6f29e4d43c7c4ea5c9e30a81447b
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643003"
---
# <a name="parentalcontrolsettings-resource-type"></a>Ressourcentyp parentalControlSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Gibt die Jugendschutzeinstellungen für eine Anwendung an. Diese Einstellungen Steuern der Zustimmung wünschen.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
:---------------|:--------|:----------|
|countriesBlockedForMinors|String-Sammlung| Gibt die [zwei Buchstaben ISO-Ländercodes](https://www.iso.org/iso-3166-country-codes.html). Zugriff auf die Anwendung werden für Minderjährige aus den in dieser Liste angegebenen Ländern blockiert.|
|legalAgeGroupRule| String | Gibt die ALTER Legal Gruppenregel, die für Benutzer der app gilt. Kann auf einen der folgenden Werte festgelegt werden: <table><tr><th>Wert</th><th>Beschreibung</th></tr><tr><td>Allow</td><td>Standard. Erzwingt die rechtliche minimale. Dies bedeutet, dass die Zustimmung der Eltern für Minderjährige in der Europäischen Union und Korea erforderlich ist.</td></tr><tr><td>RequireConsentForPrivacyServices</td><td>Erzwingt den Benutzer zum Angeben von Geburtsdatum COPPA-Regeln einhalten. </td></tr><tr><td>RequireConsentForMinors</td><td>Erfordert Zustimmung der Eltern für Jahren unter 18, unabhängig davon Land minor Regeln.</td></tr><tr><td>RequireConsentForKids</td><td>Erfordert Zustimmung der Eltern für Jahren unter 14, unabhängig davon Land minor Regeln.</td></tr><tr><td>BlockMinors</td><td>Blöcke Minderjährige aus mithilfe der app.</td></tr></table> |

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

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
