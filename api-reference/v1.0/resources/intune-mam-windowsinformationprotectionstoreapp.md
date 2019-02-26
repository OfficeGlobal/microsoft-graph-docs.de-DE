---
title: windowsInformationProtectionStoreApp-Ressourcentyp
description: Store-App für Windows-Informationsschutz
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e67e76dcec3390f172f4d2819bf7d22ee63f7da5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262545"
---
# <a name="windowsinformationprotectionstoreapp-resource-type"></a>windowsInformationProtectionStoreApp-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Store-App für Windows-Informationsschutz


Erbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|Zeichenfolge|Anzeigename der App. Geerbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
|description|String|Die Beschreibung der App. Geerbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
|publisherName|Zeichenfolge|Der Name des Herausgebers, geerbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
|productName|Zeichenfolge|Der Produktname. Geerbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|
|denied|Boolean|Bei „true“ wird der App der Schutz oder eine Ausnahme verweigert. Geerbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionStoreApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```



