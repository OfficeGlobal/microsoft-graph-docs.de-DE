---
title: windowsKioskAzureADUser-Ressourcentyp
description: Die Klasse, die zum Identifizieren eines AzureAD-Benutzerkontos für die Kiosk Konfiguration verwendet wird.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: feda393a6bee1b3cfc55d16cc91d321a5b99d54d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168250"
---
# <a name="windowskioskazureaduser-resource-type"></a>windowsKioskAzureADUser-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die Klasse, die zum Identifizieren eines AzureAD-Benutzerkontos für die Kiosk Konfiguration verwendet wird.


Erbt von [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|userId|Zeichenfolge|Die ID des AzureAD-Benutzers, der für diese Kiosk Konfiguration gesperrt wird.|
|userPrincipalName|Zeichenfolge|Die Benutzerkonten, die für diese Kiosk Konfiguration gesperrt werden|

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




