---
title: Ressourcentyp parentalControlSettings
description: Gibt die Altersfreigabe Einstellungen für eine Anwendung. Diese Einstellungen Steuern der Zustimmung wünschen.
ms.openlocfilehash: 96f0fa96f9257187e404b61eaca877302d50ccee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059055"
---
# <a name="parentalcontrolsettings-resource-type"></a>Ressourcentyp parentalControlSettings

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Gibt die Altersfreigabe Einstellungen für eine Anwendung. Diese Einstellungen Steuern der Zustimmung wünschen.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
:---------------|:--------|:----------|
|countriesBlockedForMinors|Collection von Objekten des Typs „String“| Gibt die [zwei Buchstaben ISO-Ländercodes](https://www.iso.org/iso-3166-country-codes.html). Zugriff auf die Anwendung werden für Minderjährige aus den in dieser Liste angegebenen Ländern blockiert.|
|legalAgeGroupRule| String | Gibt die ALTER Legal Gruppenregel, die für Benutzer der app gilt. Kann auf einen der folgenden Werte festgelegt werden: <table><tr><th>Wert</th><th>Beschreibung</th></tr><tr><td>Allow</td><td>Standard. Erzwingt die rechtliche minimale. Dies bedeutet, dass die Zustimmung der Eltern für Minderjährige in der Europäischen Union und Korea erforderlich ist.</td></tr><tr><td>RequireConsentForPrivacyServices</td><td>Erzwingt den Benutzer zum Angeben von Geburtsdatum COPPA-Regeln einhalten. </td></tr><tr><td>RequireConsentForMinors</td><td>Erfordert Zustimmung der Eltern für Jahren unter 18, unabhängig davon Land minor Regeln.</td></tr><tr><td>RequireConsentForKids</td><td>Erfordert Zustimmung der Eltern für Jahren unter 14, unabhängig davon Land minor Regeln.</td></tr><tr><td>BlockMinors</td><td>Blöcke Minderjährige aus mithilfe der app.</td></tr></table> |

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

```json
{
  "countriesBlockedForMinors": [ "String" ],
  "legalAgeGroupRule": "String"
}

```
