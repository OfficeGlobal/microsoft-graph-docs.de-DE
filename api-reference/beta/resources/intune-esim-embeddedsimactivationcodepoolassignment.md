---
title: Ressourcentyp embeddedSIMActivationCodePoolAssignment
description: Die eingebettete SIM Aktivierung Code Pool Zuordnung Entität weist eine bestimmte EmbeddedSIMActivationCodePool ein AAD Gerätegruppe.
ms.openlocfilehash: 27a7ed5a524d7033225ec8dfbafdf2f3f74b5ec8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058289"
---
# <a name="embeddedsimactivationcodepoolassignment-resource-type"></a>Ressourcentyp embeddedSIMActivationCodePoolAssignment

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Die eingebettete SIM Aktivierung Code Pool Zuordnung Entität weist eine bestimmte EmbeddedSIMActivationCodePool ein AAD Gerätegruppe.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste embeddedSIMActivationCodePoolAssignments](../api/intune-esim-embeddedsimactivationcodepoolassignment-list.md)|[EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Auflistung|Listeneigenschaften und Beziehungen der [EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Objekte.|
|[Abrufen von embeddedSIMActivationCodePoolAssignment](../api/intune-esim-embeddedsimactivationcodepoolassignment-get.md)|[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Lesen Sie Eigenschaften und Beziehungen des [EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Objekts.|
|[Erstellen von embeddedSIMActivationCodePoolAssignment](../api/intune-esim-embeddedsimactivationcodepoolassignment-create.md)|[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Erstellen eines neuen [EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Objekts.|
|[EmbeddedSIMActivationCodePoolAssignment löschen](../api/intune-esim-embeddedsimactivationcodepoolassignment-delete.md)|Keines|Löscht eine [EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).|
|[EmbeddedSIMActivationCodePoolAssignment aktualisieren](../api/intune-esim-embeddedsimactivationcodepoolassignment-update.md)|[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Aktualisieren Sie die Eigenschaften eines [EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner für die eingebettete SIM Aktivierung Code Pool Zuordnung. System generierten Wert, die beim Erstellen zugewiesen.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Der Typ der Zielgruppen vom eingebetteten SIM Aktivierung Code Pool.|

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





