---
title: windowsInformationProtectionNetworkLearningSummary-Ressourcentyp
description: Windows Information Protection – Netzwerk-Schulungszusammenfassungsentität
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8ad392b2685d4322c5afc90f82c381a790ef8a46
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250488"
---
# <a name="windowsinformationprotectionnetworklearningsummary-resource-type"></a>windowsInformationProtectionNetworkLearningSummary-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Windows Information Protection – Netzwerk-Schulungszusammenfassungsentität

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[windowsInformationProtectionNetworkLearningSummaries auflisten](../api/intune-wip-windowsinformationprotectionnetworklearningsummary-list.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekte.|
|[WindowsInformationProtectionNetworkLearningSummary abrufen](../api/intune-wip-windowsinformationprotectionnetworklearningsummary-get.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)|Lesen von Eigenschaften und Beziehungen des [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekts.|
|[windowsInformationProtectionNetworkLearningSummary erstellen](../api/intune-wip-windowsinformationprotectionnetworklearningsummary-create.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)|Erstellen eines neuen [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekts.|
|[windowsInformationProtectionNetworkLearningSummary löschen](../api/intune-wip-windowsinformationprotectionnetworklearningsummary-delete.md)|Keine|Löscht ein [windowsInformationProtectionNetworkLearningSummary löschen](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekt.|
|[windowsInformationProtectionNetworkLearningSummary aktualisieren](../api/intune-wip-windowsinformationprotectionnetworklearningsummary-update.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)|Aktualisieren der Eigenschaften eines [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner für die WindowsInformationProtectionNetworkLearningSummary.|
|url|String|Website-URL|
|deviceCount|Int32|Geräteanzahl|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionNetworkLearningSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "String (identifier)",
  "url": "String",
  "deviceCount": 1024
}
```



