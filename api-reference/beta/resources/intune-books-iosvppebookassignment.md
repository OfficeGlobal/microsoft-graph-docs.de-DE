---
title: iosVppEBookAssignment-Ressourcentyp
description: Enthält Eigenschaften zum Zuweisen eines iOS-VPP-E-Books zu einer Gruppe.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 49ddbf75f4e073f636857c4ba9c9fa7910c847f1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399591"
---
# <a name="iosvppebookassignment-resource-type"></a>iosVppEBookAssignment-Ressourcentyp

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

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
|installIntent|[installIntent](../resources/intune-shared-installintent.md)|Installationspriorität für das E-Book. Geerbt von [ManagedEBookAssignment](../resources/intune-books-managedebookassignment.md). Mögliche Werte: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|

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




