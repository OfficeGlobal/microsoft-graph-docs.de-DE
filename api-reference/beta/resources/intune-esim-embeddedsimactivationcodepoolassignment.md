---
title: embeddedSIMActivationCodePoolAssignment-Ressourcentyp
description: Die eingebettete Zuweisungs Entität SIM-Aktivierungscode Pool weist einer AAD-Gerätegruppe eine bestimmte embeddedSIMActivationCodePool zu.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 60b92a7b1232ba19a4166171fa118b18f7a263b8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163392"
---
# <a name="embeddedsimactivationcodepoolassignment-resource-type"></a>embeddedSIMActivationCodePoolAssignment-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die eingebettete Zuweisungs Entität SIM-Aktivierungscode Pool weist einer AAD-Gerätegruppe eine bestimmte embeddedSIMActivationCodePool zu.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[EmbeddedSIMActivationCodePoolAssignments aufListen](../api/intune-esim-embeddedsimactivationcodepoolassignment-list.md)|[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Objekte.|
|[EmbeddedSIMActivationCodePoolAssignment abrufen](../api/intune-esim-embeddedsimactivationcodepoolassignment-get.md)|[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Lesen von Eigenschaften und Beziehungen des [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Objekts.|
|[EmbeddedSIMActivationCodePoolAssignment erstellen](../api/intune-esim-embeddedsimactivationcodepoolassignment-create.md)|[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Erstellen eines neuen [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Objekts.|
|[EmbeddedSIMActivationCodePoolAssignment löschen](../api/intune-esim-embeddedsimactivationcodepoolassignment-delete.md)|Keine|Löscht eine [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).|
|[EmbeddedSIMActivationCodePoolAssignment aktualisieren](../api/intune-esim-embeddedsimactivationcodepoolassignment-update.md)|[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Aktualisieren der Eigenschaften eines [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Eindeutige ID für den eingebetteten SIM-Aktivierungscode-Pool-Zuweisung. Vom System generierter Wert, der bei der Erstellung zugewiesen wird.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Der Typ der Gruppen, die vom eingebetteten SIM-Aktivierungscode Pool abzielen.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.embeddedSIMActivationCodePoolAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




