---
title: iosSingleSignOnSettings-Ressourcentyp
description: iOS-Kerberos-Authentifizierungseinstellungen für einmaliges Anmelden
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b438ea8fadc30a0bf5fa3786e9b4cec3344093c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142623"
---
# <a name="iossinglesignonsettings-resource-type"></a>iosSingleSignOnSettings-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

iOS-Kerberos-Authentifizierungseinstellungen für einmaliges Anmelden

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|allowedAppsList|Collection von Objekten des Typs [appListItem](../resources/intune-deviceconfig-applistitem.md)|Liste der APP-IDs, die diese Anmeldung verwenden dürfen. Wenn dieses Feld nicht angegeben wird, gilt die Anmeldung für alle Anwendungen auf dem Gerät. Diese Collection darf maximal 500 Elemente enthalten.|
|allowedUrls|String collection|Liste der HTTP-URLs, die abgeglichen werden müssen, um diese Anmeldung zu verwenden. Mit iOS 9,0 oder höher können Platzhalterzeichen verwendet werden.|
|displayName|Zeichenfolge|Der Anzeigename der Anmeldeeinstellungen, die auf dem empfangenden Gerät angezeigt werden.|
|kerberosPrincipalName|Zeichenfolge|Ein Kerberos-Prinzipalname. Wenn nicht angegeben, wird der Benutzer während der Profilinstallation zur Eingabe eines Eintrags aufgefordert.|
|kerberosRealm|Zeichenfolge|Ein Kerberos-Bereichsname. Groß-/Kleinschreibung beachtet.|

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




