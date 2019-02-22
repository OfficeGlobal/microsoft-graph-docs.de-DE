---
title: deviceManagementUserRightsLocalUserOrGroup-Ressourcentyp
description: Stellt Informationen für einen lokalen Benutzer oder eine Gruppe dar, die für die Benutzerrechte Einstellung verwendet wird.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 68c514635540bcf12db27e8a9ca816573293d3ad
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174860"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a>deviceManagementUserRightsLocalUserOrGroup-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Stellt Informationen für einen lokalen Benutzer oder eine Gruppe dar, die für die Benutzerrechte Einstellung verwendet wird.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|name|Zeichenfolge|Der Name dieses lokalen Benutzers oder dieser Gruppe.|
|description|Zeichenfolge|Die Beschreibung des Administrators dieses lokalen Benutzers oder dieser Gruppe.|
|securityIdentifier|Zeichenfolge|Die Sicherheits-ID dieses lokalen Benutzers oder einer Gruppe (z. b. * S-1-5-32-544).|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
  "name": "String",
  "description": "String",
  "securityIdentifier": "String"
}
```




