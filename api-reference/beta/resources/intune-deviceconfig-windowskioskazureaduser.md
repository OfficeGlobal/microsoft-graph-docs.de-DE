---
title: Ressourcentyp windowsKioskAzureADUser
description: Die Klasse verwendet, um ein Benutzerkonto AzureAD für die Konfiguration Kiosk identifizieren
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4497c6d42db45f518e3ef93e78e50d25f473ac00
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984143"
---
# <a name="windowskioskazureaduser-resource-type"></a>Ressourcentyp windowsKioskAzureADUser

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Die Klasse verwendet, um ein Benutzerkonto AzureAD für die Konfiguration Kiosk identifizieren

Erbt vom [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|userId|Zeichenfolge|Die ID des Benutzers, die mit dieser Konfiguration Kiosk gesperrt werden AzureAD|
|userPrincipalName|Zeichenfolge|Die Benutzerkonten, die mit dieser Konfiguration Kiosk gesperrt wird|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADUser",
  "userId": "String",
  "userPrincipalName": "String"
}
```





