---
title: Ressourcentyp managedEBookCategory
description: Enthält Eigenschaften für eine einzelne Intune eBook Kategorie.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7f4136fbfb93db6e7e9dee4a81dcc44a613a7226
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915956"
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





