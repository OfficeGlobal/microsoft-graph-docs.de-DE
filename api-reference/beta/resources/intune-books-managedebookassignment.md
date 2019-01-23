---
title: managedEBookAssignment-Ressourcentyp
description: Enthält Eigenschaften zum Zuweisen eines E-Books zu einer Gruppe.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f6d6cdc1cbe5b2eb7b734219dbb7c67152afe3a2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423545"
---
# <a name="managedebookassignment-resource-type"></a>managedEBookAssignment-Ressourcentyp

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

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




