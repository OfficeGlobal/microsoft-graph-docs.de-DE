---
title: countriesRegions-Ressourcentyp
description: Ein Objekt "Länder/Regionen" in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: b6f50ba3046a402f2b8729529675653286808459
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365486"
---
# <a name="countriesregions-resource-type"></a>countriesRegions-Ressourcentyp
Stellt ein countriesRegions-Objekt in Dynamics 365 Business Central dar, das Teil einer Adresse ist.

## <a name="methods"></a>Methoden

| Methode                                                              | Rückgabetyp    |Beschreibung                |
|:--------------------------------------------------------------------|:---------------|:--------------------------|
|[CountriesRegions abrufen](../api/dynamics-countriesregions-get.md)      |countriesRegions|Holen Sie sich eine Länder/Regionen.   |
|[Post countriesRegions](../api/dynamics-create-countriesregions.md)  |countriesRegions|Erstellen Sie eine Länder/Regionen.|
|[Patch-countriesRegions](../api/dynamics-countriesregions-update.md) |countriesRegions|Aktualisieren Sie eine Länder/Regionen.|
|[CountriesRegions löschen](../api/dynamics-countriesregions-delete.md)|Keine            |Löschen Sie eine Länder/Regionen.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ       |Beschreibung                                                  |
|:---------------|:-----------|:------------------------------------------------------------|
|id              |GUID        |Die eindeutige ID des Landes/der Region. Nicht bearbeitbar.           |
|code            |string      |Gibt den Code des Landes/der Region an.                    |
|displayName     |string      |Gibt den Anzeigenamen des Landes/der Region an.            |
|Sind hinterlegt   |string      |Gibt das Format der Adresse an, die auf externen Dokumenten angezeigt wird. Sie verknüpfen ein Adressformat mit einem Land/Regionscode, sodass externe Dokumente, die auf Karten oder Dokumenten mit diesem Land/Regionscode basieren, das angegebene Adressformat verwenden.|
|lastModifiedDateTime|DateTime|Die letzte Uhrzeit, zu der das Land/die Region geändert wurde. Schreibgeschützt.|  


## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung des countriesRegions.


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "addressFormat": "string",
  "lastModifiedDateTime": "datetime"
}

```


