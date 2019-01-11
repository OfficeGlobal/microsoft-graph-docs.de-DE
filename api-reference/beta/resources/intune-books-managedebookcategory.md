---
title: Ressourcentyp managedEBookCategory
description: Enthält Eigenschaften für eine einzelne Intune eBook Kategorie.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b415554d47c33f06a917c10327dad983db762578
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894187"
---
# <a name="managedebookcategory-resource-type"></a>Ressourcentyp managedEBookCategory

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

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





