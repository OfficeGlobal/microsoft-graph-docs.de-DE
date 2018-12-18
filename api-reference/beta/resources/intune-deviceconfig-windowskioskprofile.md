---
title: Ressourcentyp windowsKioskProfile
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: ce57b18e86f40a46053a5e0a0f41652763a6d055
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345353"
---
# <a name="windowskioskprofile-resource-type"></a>Ressourcentyp windowsKioskProfile

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Noch nicht dokumentiert
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|ID|String|Schlüssel der Entität|
|Profilname|String|Dies ist ein Anzeigename zur Identifizierung einer Gruppe von Anwendungen, das Layout von diese apps auf das Startmenü und die Benutzer, die diese Konfiguration Kiosk zugewiesen ist.|
|appConfiguration|[windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)|Die App-Konfiguration, die für diese Konfiguration Kiosk verwendet werden soll.|
|userAccountsConfiguration|[WindowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) -Auflistung|Die Benutzerkonten, die mit dieser Konfiguration Kiosk gesperrt werden. Diese Sammlung darf maximal 500 Elemente enthalten.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskProfile",
  "profileId": "String",
  "profileName": "String",
  "appConfiguration": {
    "@odata.type": "microsoft.graph.windowsKioskMultipleApps",
    "apps": [
      {
        "@odata.type": "microsoft.graph.windowsKioskUWPApp",
        "startLayoutTileSize": "String",
        "name": "String",
        "appUserModelId": "String",
        "appId": "String",
        "containedAppId": "String"
      }
    ],
    "showTaskBar": true,
    "disallowDesktopApps": true,
    "startMenuLayoutXml": "binary"
  },
  "userAccountsConfiguration": [
    {
      "@odata.type": "microsoft.graph.windowsKioskVisitor"
    }
  ]
}
```





