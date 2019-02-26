---
title: managedEBookCategory-Ressourcentyp
description: Enthält Eigenschaften für eine einzelne InTune-eBook-Kategorie.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cb96477944edad4e2ca85020aa273e6718f8cdc2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152452"
---
# <a name="managedebookcategory-resource-type"></a>managedEBookCategory-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Eigenschaften für eine einzelne InTune-eBook-Kategorie.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Mobileappconfigurations aufListen](../api/intune-books-managedebookcategory-list.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [managedEBookCategory](../resources/intune-books-managedebookcategory.md) -Objekte.|
|[ManagedEBookCategory abrufen](../api/intune-books-managedebookcategory-get.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md)|Lesen von Eigenschaften und Beziehungen des [managedEBookCategory](../resources/intune-books-managedebookcategory.md) -Objekts.|
|[ManagedEBookCategory erstellen](../api/intune-books-managedebookcategory-create.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md)|Erstellen eines neuen [managedEBookCategory](../resources/intune-books-managedebookcategory.md) -Objekts.|
|[ManagedEBookCategory löschen](../api/intune-books-managedebookcategory-delete.md)|Keine|Löscht eine [managedEBookCategory](../resources/intune-books-managedebookcategory.md).|
|[ManagedEBookCategory aktualisieren](../api/intune-books-managedebookcategory-update.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md)|Aktualisieren der Eigenschaften eines [managedEBookCategory](../resources/intune-books-managedebookcategory.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|displayName|Zeichenfolge|Der Name der eBook-Kategorie.|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des ManagedEBookCategory.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBookCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```




