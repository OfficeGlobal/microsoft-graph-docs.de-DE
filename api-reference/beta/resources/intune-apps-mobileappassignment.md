---
title: mobileAppAssignment-Ressourcentyp
description: Eine Klasse, die die Eigenschaften für die Gruppenzuordnung einer mobilen App enthält.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 77816742d4e7d736cad2941c3a49f2f6350ebd84
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140635"
---
# <a name="mobileappassignment-resource-type"></a>mobileAppAssignment-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

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
|id|Zeichenfolge|Schlüssel der Entität|
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




