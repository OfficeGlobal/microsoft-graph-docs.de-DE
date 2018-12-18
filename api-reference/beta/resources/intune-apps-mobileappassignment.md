---
title: mobileAppAssignment-Ressourcentyp
description: Eine Klasse, die die Eigenschaften für die Gruppenzuordnung einer mobilen App enthält.
author: tfitzmac
ms.openlocfilehash: 5f1413bc973d3721c7e9b01aa29e513028af9926
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320572"
---
# <a name="mobileappassignment-resource-type"></a>mobileAppAssignment-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Eine Klasse, die die Eigenschaften für die Gruppenzuordnung einer mobilen App enthält.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[mobileAppAssignments auflisten](../api/intune-apps-mobileappassignment-list.md)|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Objekte.|
|[mobileAppAssignment abrufen](../api/intune-apps-mobileappassignment-get.md)|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Lesen von Eigenschaften und Beziehungen des [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Objekts.|
|[mobileAppAssignment erstellen](../api/intune-apps-mobileappassignment-create.md)|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Erstellen eines neuen [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Objekts.|
|[mobileAppAssignment löschen](../api/intune-apps-mobileappassignment-delete.md)|Keine|Löschen einer [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).|
|[mobileAppAssignment aktualisieren](../api/intune-apps-mobileappassignment-update.md)|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Aktualisieren der Eigenschaften eines [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|intent|[installIntent](../resources/intune-shared-installintent.md)|Die vom Administrator definierte Installationspriorität. Mögliche Werte sind: `available`, `required`, `uninstall` und `availableWithoutEnrollment`.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Die vom Administrator definierte Zielgruppenzuordnung|
|settings|[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)|Die vom Administrator definierten Einstellungen für die Zielgruppenzuordnung.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "String (identifier)",
  "intent": "String",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```





