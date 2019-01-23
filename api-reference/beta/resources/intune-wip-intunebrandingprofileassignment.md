---
title: Ressourcentyp intuneBrandingProfileAssignment
description: Diese Entität enthält die Eigenschaften verwendet, um einer Gruppe ein branding Profil zuzuweisen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fcc0b625bc3918206a1d75ae7ef123484ae0357c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431523"
---
# <a name="intunebrandingprofileassignment-resource-type"></a>Ressourcentyp intuneBrandingProfileAssignment

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Diese Entität enthält die Eigenschaften verwendet, um einer Gruppe ein branding Profil zuzuweisen.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste intuneBrandingProfileAssignments](../api/intune-wip-intunebrandingprofileassignment-list.md)|[IntuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) -Auflistung|Listeneigenschaften und Beziehungen der [IntuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) -Objekte.|
|[Abrufen von intuneBrandingProfileAssignment](../api/intune-wip-intunebrandingprofileassignment-get.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|Lesen Sie Eigenschaften und Beziehungen des [IntuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) -Objekts.|
|[Erstellen von intuneBrandingProfileAssignment](../api/intune-wip-intunebrandingprofileassignment-create.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|Erstellen eines neuen [IntuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) -Objekts.|
|[IntuneBrandingProfileAssignment löschen](../api/intune-wip-intunebrandingprofileassignment-delete.md)|Keine|Löscht eine [IntuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).|
|[IntuneBrandingProfileAssignment aktualisieren](../api/intune-wip-intunebrandingprofileassignment-update.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|Aktualisieren Sie die Eigenschaften eines [IntuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner der Entität|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Zuordnungsfeld Ziel an, die das branding Profil zugewiesen ist.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.intuneBrandingProfileAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




