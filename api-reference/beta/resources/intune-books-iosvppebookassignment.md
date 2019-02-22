---
title: iosVppEBookAssignment-Ressourcentyp
description: Enthält Eigenschaften zum Zuweisen eines iOS-VPP-E-Books zu einer Gruppe.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 329069f0bbda62e0edd6f03b95856c382d4c0983
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150295"
---
# <a name="iosvppebookassignment-resource-type"></a>iosVppEBookAssignment-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Eigenschaften zum Zuweisen eines iOS-VPP-E-Books zu einer Gruppe.


Erbt von [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[iosVppEBookAssignments auflisten](../api/intune-books-iosvppebookassignment-list.md)|[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md)-Objekte.|
|[iosVppEBookAssignment abrufen](../api/intune-books-iosvppebookassignment-get.md)|[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md)|Lesen von Eigenschaften und Beziehungen des [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md)-Objekts.|
|[iosVppEBookAssignment erstellen](../api/intune-books-iosvppebookassignment-create.md)|[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md)|Erstellen eines neuen [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md)-Objekts.|
|[iosVppEBookAssignment löschen](../api/intune-books-iosvppebookassignment-delete.md)|Keine|Löscht ein [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md)-Objekt.|
|[iosVppEBookAssignment aktualisieren](../api/intune-books-iosvppebookassignment-update.md)|[iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md)|Aktualisieren der Eigenschaften eines [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität. Geerbt von [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Zuweisungsziel für das E-Book. Geerbt von [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).|
|installIntent|[installIntent](../resources/intune-shared-installintent.md)|Installationspriorität für das E-Book. Von [ManagedEBookAssignment](../resources/intune-books-managedebookassignment.md)geerbt. Mögliche Werte: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppEBookAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "String"
}
```




