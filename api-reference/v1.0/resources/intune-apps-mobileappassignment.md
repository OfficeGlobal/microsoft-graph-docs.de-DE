---
title: mobileAppAssignment-Ressourcentyp
description: Eine Klasse, die die Eigenschaften für die Gruppenzuordnung einer mobilen App enthält.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f0f3faff8a04709788e415b72013e32a850889ad
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251692"
---
# <a name="mobileappassignment-resource-type"></a>mobileAppAssignment-Ressourcentyp

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



