---
title: Ressourcentyp "Items"
description: Ein Item-Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 42ec7720e2e858f319beab8576fbe57542dd470c
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365962"
---
# <a name="items-resource-type"></a>Ressourcentyp "Items"
Stellt ein Element in Dynamics 365 Business Central dar.

## <a name="methods"></a>Methoden

| Methode                                      |Rückgabetyp|Beschreibung |
|:--------------------------------------------|:----------|:-----------|
|[Elemente abrufen](../api/dynamics-item-get.md)      |Elemente     |Ruft ein Item-Objekt ab.   |
|[Bereitstellungselemente](../api/dynamics-create-item.md)  |Elemente     |Erstellt ein Item-Objekt.|
|[Patchelement](../api/dynamics-item-update.md)  |Elemente     |Aktualisiert ein Item-Objekt.|
|[Löschen von Elementen](../api/dynamics-item-delete.md)|Keine      |Löscht ein Item-Objekt.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft           | Typ |Beschreibung                                          |
|:-------------------|:-------|:----------------------------------------------------|
|id                  |GUID    |Die eindeutige ID des Elements. Nicht bearbeitbar.             |
|number              |string  |Die Artikelnummer.                                     |
|displayName         |string  |Gibt eine Beschreibung des Elements an.                 |
|type                |numerischen |Der inventurtyp für das Element. 1 = Inventarelement, 2 = Service Element. Dies ist eine erforderliche Eigenschaft.|
|gesperrt             |Boolescher Wert |Gibt an, dass Transaktionen mit dem Element nicht gebucht werden können, da sich das Element in der Quarantäne befindet. Wird auf **true**festgelegt, wenn item blockiert ist.|
|baseUnitOfMeasureId |GUID    |Gibt die ID der Maßeinheit an.             |
|baseUnitOfMeasure   |[Navigations. UnitOfMeasure](../resources/dynamics-complextypes.md)|Gibt die Einheit an, in der das Element im Bestand aufbewahrt wird.|
|GTIN                |numerischen |Dies ist die Nummer des globalen Handels Artikels.                |
|itemCategoryId      |GUID |Gibt die Kategorie an, zu der das Element gehört. Elementkategorien enthalten auch alle zugewiesenen Element Attribute.|
|inventory           |decimal |Gibt an, wie viele Einheiten, wie Teile, Kisten oder Dosen, des Elements im Inventar sind. Schreibgeschützt.|
|unitPrice           |decimal |Gibt den Preis für eine Einheit des Elements in der angegebenen Währung an.|
|priceIncludesTax    |Boolescher Wert |Gibt an, dass der Einzelpreis Steuern enthält. Auf **true**festgelegt, wenn Einzelpreis Steuer enthält.|
|unitCost            |decimal |Gibt die Kosten pro Einheit des Elements an.             |
|taxGroupId          |GUID    |Gibt die ID der Steuergruppe für das Element an.      |
|taxGroupCode        |numerischen |Eine Steuergruppe stellt eine Gruppe von Inventar Elementen oder Ressourcen dar, die identischen Steuerbedingungen unterliegen.|
|lastModifiedDateTime|DateTime|Die letzte DateTime, die das Element geändert wurde. Schreibgeschützt.  |  


## <a name="relationships"></a>Beziehungen
In der Tabelle "Steuergruppe" muss eine Steuergruppe (taxGroupCode) vorhanden sein.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.


```json
{
      "id": "GUID",
      "number": "string",
      "displayName": "string",
      "type": "string",
      "blocked": "boolean",
      "baseUnitOfMeasureId": "GUID",
      "baseUnitOfMeasure": "NAV.UnitOfMeasure",
      "gtin": "numeric",
      "itemCategoryId": "GUID",
      "inventory": "decimal",
      "unitPrice": "decimal",
      "priceIncludesTax": "boolean",
      "unitCost": "decimal",
      "taxGroupId": "GUID",
      "taxGroupCode": "string",
      "lastModifiedDateTime": "datetime"
}

```


