---
title: Ressourcentyp managedEBookCategory
description: Enthält Eigenschaften für eine einzelne Intune eBook Kategorie.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: df057c3aa05d181365397d150aeae93754b63dad
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415334"
---
# <a name="managedebookcategory-resource-type"></a>Ressourcentyp managedEBookCategory

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Enthält Eigenschaften für eine einzelne Intune eBook Kategorie.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste managedEBookCategories](../api/intune-books-managedebookcategory-list.md)|[ManagedEBookCategory](../resources/intune-books-managedebookcategory.md) -Auflistung|Listeneigenschaften und Beziehungen der [ManagedEBookCategory](../resources/intune-books-managedebookcategory.md) -Objekte.|
|[Abrufen von managedEBookCategory](../api/intune-books-managedebookcategory-get.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md)|Lesen Sie Eigenschaften und Beziehungen des [ManagedEBookCategory](../resources/intune-books-managedebookcategory.md) -Objekts.|
|[Erstellen von managedEBookCategory](../api/intune-books-managedebookcategory-create.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md)|Erstellen eines neuen [ManagedEBookCategory](../resources/intune-books-managedebookcategory.md) -Objekts.|
|[ManagedEBookCategory löschen](../api/intune-books-managedebookcategory-delete.md)|Keine|Löscht eine [ManagedEBookCategory](../resources/intune-books-managedebookcategory.md).|
|[ManagedEBookCategory aktualisieren](../api/intune-books-managedebookcategory-update.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md)|Aktualisieren Sie die Eigenschaften eines [ManagedEBookCategory](../resources/intune-books-managedebookcategory.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|displayName|Zeichenfolge|Der Name der Kategorie eBook.|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der ManagedEBookCategory.|

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




