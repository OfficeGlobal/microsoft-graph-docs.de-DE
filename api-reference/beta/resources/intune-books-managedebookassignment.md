---
title: managedEBookAssignment-Ressourcentyp
description: Enthält Eigenschaften zum Zuweisen eines E-Books zu einer Gruppe.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7954dbb1208a59842dd0a743e18e4f81466e09f6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146879"
---
# <a name="managedebookassignment-resource-type"></a>managedEBookAssignment-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Eigenschaften zum Zuweisen eines E-Books zu einer Gruppe.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[managedEBookAssignments auflisten](../api/intune-books-managedebookassignment-list.md)|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)-Objekte.|
|[managedEBookAssignment abrufen](../api/intune-books-managedebookassignment-get.md)|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|Lesen von Eigenschaften und Beziehungen des [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)-Objekts.|
|[managedEBookAssignment erstellen](../api/intune-books-managedebookassignment-create.md)|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|Erstellen eines neuen [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)-Objekts.|
|[managedEBookAssignment löschen](../api/intune-books-managedebookassignment-delete.md)|Keine|Löscht ein [ManagedEBookAssignment](../resources/intune-books-managedebookassignment.md)-Objekt.|
|[managedEBookAssignment aktualisieren](../api/intune-books-managedebookassignment-update.md)|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|Aktualisieren der Eigenschaften eines [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Zuweisungsziel für das E-Book|
|installIntent|[installIntent](../resources/intune-shared-installintent.md)|Installationspriorität für das E-Book. Mögliche Werte: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBookAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "String"
}
```




