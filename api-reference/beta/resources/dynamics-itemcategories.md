---
title: itemCategories-Ressourcentyp
description: Eine elementkategorie in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: e18319683f6dbceddccc9cf83e48cd3ef89f895d
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365745"
---
# <a name="itemcategories-resource-type"></a>itemCategories-Ressourcentyp
Stellt eine Kategorie für eine Reihe von Elementen in Dynamics 365 Business Central dar.

## <a name="methods"></a>Methoden

| Methode                                                          | Rückgabetyp  |Beschreibung             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[ItemCategories abrufen](../api/dynamics-itemcategories-get.md)      |itemCategories|Rufen Sie eine elementkategorie ab.   |
|[Post itemCategories](../api/dynamics-create-itemcategories.md)  |itemCategories|Erstellen Sie eine elementkategorie.|
|[Patch-itemCategories](../api/dynamics-itemcategories-update.md) |itemCategories|Aktualisieren Sie eine elementkategorie.|
|[ItemCategories löschen](../api/dynamics-itemcategories-delete.md)|Keine          |Löscht eine elementkategorie.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft           | Typ   |Beschreibung                                     |
|:-------------------|:-------|:-----------------------------------------------|
|id                  |GUID    |Die eindeutige ID des itemCategory. Nicht bearbeitbar.|
|code                |string  |Der itemCategory-Code.                          |
|displayName         |string  |Der Anzeigename des itemCategories.                |
|lastModifiedDateTime|DateTime|Die letzte DateTime, die der itemCategory geändert wurde. Schreibgeschützt.|  


## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung des itemCategories.

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}
```

