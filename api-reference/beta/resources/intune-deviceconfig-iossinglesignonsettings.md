---
title: Ressourcentyp iosSingleSignOnSettings
description: iOS Kerberos-Authentifizierungseinstellungen für einmaliges Anmelden
ms.openlocfilehash: a63848dc27afd037a6834a67c0736f86c06ac1fe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064624"
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
|displayName|String|Der Anzeigename der Einstellungen für die Anmeldung auf dem empfangenden Gerät angezeigt.|
|kerberosPrincipalName|String|Ein Kerberos principal Name. Wenn nicht angegeben, wird der Benutzer während der Profilinstallation dazu aufgefordert.|
|kerberosRealm|String|Ein Kerberos-Realm-Name. Groß-/Kleinschreibung beachtet.|

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





