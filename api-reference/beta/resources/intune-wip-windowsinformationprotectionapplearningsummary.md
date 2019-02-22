---
title: windowsInformationProtectionAppLearningSummary-Ressourcentyp
description: Windows Information Protection App Learning – Zusammenfassungsentität.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c42fbe9da221e9c41a29291d6a279b1144cd355
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169489"
---
# <a name="windowsinformationprotectionapplearningsummary-resource-type"></a>windowsInformationProtectionAppLearningSummary-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Windows Information Protection App Learning – Zusammenfassungsentität.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[windowsInformationProtectionAppLearningSummaries auflisten](../api/intune-wip-windowsinformationprotectionapplearningsummary-list.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekte.|
|[windowsInformationProtectionAppLearningSummary abrufen](../api/intune-wip-windowsinformationprotectionapplearningsummary-get.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)|Lesen von Eigenschaften und Beziehungen des [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekts.|
|[windowsInformationProtectionAppLearningSummary erstellen](../api/intune-wip-windowsinformationprotectionapplearningsummary-create.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)|Erstellen eines neuen [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekts.|
|[windowsInformationProtectionAppLearningSummary löschen](../api/intune-wip-windowsinformationprotectionapplearningsummary-delete.md)|Keine|Löscht ein [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekt.|
|[windowsInformationProtectionAppLearningSummary aktualisieren](../api/intune-wip-windowsinformationprotectionapplearningsummary-update.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)|Aktualisieren der Eigenschaften eines [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Eindeutiger Bezeichner für die WindowsInformationProtectionAppLearningSummary.|
|applicationName|String|Name der Anwendung|
|applicationType|[applicationType](../resources/intune-wip-applicationtype.md)|Anwendungstyp. Mögliche Werte sind: `universal` und `desktop`.|
|deviceCount|Int32|Geräteanzahl|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionAppLearningSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "id": "String (identifier)",
  "applicationName": "String",
  "applicationType": "String",
  "deviceCount": 1024
}
```




