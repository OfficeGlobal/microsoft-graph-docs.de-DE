---
title: Ressourcentyp iosSingleSignOnSettings
description: iOS Kerberos-Authentifizierungseinstellungen für einmaliges Anmelden
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 54c5656de6262692324cce8ab71a0e100672c050
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952671"
---
# <a name="iossinglesignonsettings-resource-type"></a>Ressourcentyp iosSingleSignOnSettings

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

iOS Kerberos-Authentifizierungseinstellungen für einmaliges Anmelden
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|allowedAppsList|Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)|Liste der app-Bezeichner, die dieser Anmeldung verwenden dürfen. Wenn dieses Feld nicht angegeben wird, gilt die Anmeldung auf alle Programme, auf dem Gerät. Diese Collection darf maximal 500 Elemente enthalten.|
|allowedUrls|Collection von Objekten des Typs „String“|Liste der HTTP-URLs, die übereinstimmen muss, um diesen Benutzernamen verwenden. IOS 9.0 oder höher können ein Platzhalterzeichen verwendet werden.|
|displayName|Zeichenfolge|Der Anzeigename der Einstellungen für die Anmeldung auf dem empfangenden Gerät angezeigt.|
|kerberosPrincipalName|Zeichenfolge|Ein Kerberos principal Name. Wenn nicht angegeben, wird der Benutzer während der Profilinstallation dazu aufgefordert.|
|kerberosRealm|Zeichenfolge|Ein Kerberos-Realm-Name. Groß-/Kleinschreibung beachtet.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosSingleSignOnSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosSingleSignOnSettings",
  "allowedAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "allowedUrls": [
    "String"
  ],
  "displayName": "String",
  "kerberosPrincipalName": "String",
  "kerberosRealm": "String"
}
```





