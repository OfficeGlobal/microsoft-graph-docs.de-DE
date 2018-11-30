---
title: managedEBookAssignment-Ressourcentyp
description: Enthält Eigenschaften zum Zuweisen eines E-Books zu einer Gruppe.
ms.openlocfilehash: ecf79b4055ea87d710cb62ac4446bb5bd65793ee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018813"
---
# <a name="managedebookassignment-resource-type"></a>managedEBookAssignment-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

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
|id|String|Schlüssel der Entität|
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



