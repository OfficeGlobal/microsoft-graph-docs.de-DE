---
title: Ressourcentyp iosSingleSignOnSettings
description: iOS Kerberos-Authentifizierungseinstellungen für einmaliges Anmelden
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 189fb79be741bdf6b731b1e3c2b336934db8c86b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421319"
---
# <a name="iossinglesignonsettings-resource-type"></a>Ressourcentyp iosSingleSignOnSettings

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

iOS Kerberos-Authentifizierungseinstellungen für einmaliges Anmelden

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|allowedAppsList|Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)|Liste der app-Bezeichner, die dieser Anmeldung verwenden dürfen. Wenn dieses Feld nicht angegeben wird, gilt die Anmeldung auf alle Programme, auf dem Gerät. Diese Collection darf maximal 500 Elemente enthalten.|
|allowedUrls|Zeichenfolgenauflistung|Liste der HTTP-URLs, die übereinstimmen muss, um diesen Benutzernamen verwenden. IOS 9.0 oder höher können ein Platzhalterzeichen verwendet werden.|
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




