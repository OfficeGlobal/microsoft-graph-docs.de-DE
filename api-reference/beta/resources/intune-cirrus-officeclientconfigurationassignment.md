---
title: Ressourcentyp officeClientConfigurationAssignment
description: Office-Client-Konfiguration Zuordnung.
author: tfitzmac
ms.openlocfilehash: c2b8dc231fb390cbb2bd5dbb93b5226540b84f5f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315994"
---
# <a name="officeclientconfigurationassignment-resource-type"></a>Ressourcentyp officeClientConfigurationAssignment

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Office-Client-Konfiguration Zuordnung.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste officeClientConfigurationAssignments](../api/intune-cirrus-officeclientconfigurationassignment-list.md)|[OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Auflistung|Listeneigenschaften und Beziehungen der [OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Objekte.|
|[Abrufen von officeClientConfigurationAssignment](../api/intune-cirrus-officeclientconfigurationassignment-get.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Lesen Sie Eigenschaften und Beziehungen des [OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Objekts.|
|[Erstellen von officeClientConfigurationAssignment](../api/intune-cirrus-officeclientconfigurationassignment-create.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Erstellen eines neuen [OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Objekts.|
|[OfficeClientConfigurationAssignment löschen](../api/intune-cirrus-officeclientconfigurationassignment-delete.md)|Keines|Löscht eine [OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).|
|[OfficeClientConfigurationAssignment aktualisieren](../api/intune-cirrus-officeclientconfigurationassignment-update.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Aktualisieren Sie die Eigenschaften eines [OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|ID des der OfficeConfigurationAssignment.|
|target|[officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|Die Ziel-Zuordnung, die durch den Administrator definiert|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```



