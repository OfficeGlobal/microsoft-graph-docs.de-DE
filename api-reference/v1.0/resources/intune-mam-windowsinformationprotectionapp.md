---
title: windowsInformationProtectionApp-Ressourcentyp
description: App für Windows-Informationsschutz
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 00d329baea829fa8fb7664895382a377f53461ab
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257036"
---
# <a name="windowsinformationprotectionapp-resource-type"></a>windowsInformationProtectionApp-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

App für Windows-Informationsschutz

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|Zeichenfolge|Anzeigename der App|
|description|String|Beschreibung der App|
|publisherName|Zeichenfolge|Name des Verlegers|
|productName|String|Produktname|
|denied|Boolean|Bei „true“ wird der App der Schutz oder eine Ausnahme verweigert.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```



