---
title: intuneBrandingProfileAssignment-Ressourcentyp
description: Diese Entität enthält die Eigenschaften, die zum Zuweisen eines Branding-Profils zu einer Gruppe verwendet werden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 956cf652167714270dfcaf348523db236fb62941
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151394"
---
# <a name="intunebrandingprofileassignment-resource-type"></a>intuneBrandingProfileAssignment-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Diese Entität enthält die Eigenschaften, die zum Zuweisen eines Branding-Profils zu einer Gruppe verwendet werden.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[IntuneBrandingProfileAssignments aufListen](../api/intune-wip-intunebrandingprofileassignment-list.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) -Objekte.|
|[IntuneBrandingProfileAssignment abrufen](../api/intune-wip-intunebrandingprofileassignment-get.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|Lesen von Eigenschaften und Beziehungen des [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) -Objekts.|
|[IntuneBrandingProfileAssignment erstellen](../api/intune-wip-intunebrandingprofileassignment-create.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|Erstellen eines neuen [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) -Objekts.|
|[IntuneBrandingProfileAssignment löschen](../api/intune-wip-intunebrandingprofileassignment-delete.md)|Keine|Löscht eine [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).|
|[IntuneBrandingProfileAssignment aktualisieren](../api/intune-wip-intunebrandingprofileassignment-update.md)|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|Aktualisieren der Eigenschaften eines [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner der Entität|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Zuordnungsziel, dem das Branding-Profil zugeordnet ist.|

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




