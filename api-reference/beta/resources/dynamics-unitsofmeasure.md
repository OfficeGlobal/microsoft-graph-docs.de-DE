---
title: unitsOfMeasure-Ressourcentyp
description: Ein Maßeinheits Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 870e188939646594b62e6eebf3e234eb0211f140
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365752"
---
# <a name="unitsofmeasure-resource-type"></a>unitsOfMeasure-Ressourcentyp
Stellt eine Maßeinheit dar, bei der es sich um einen Standardwert für die Messung einer Menge in Dynamics 365 Business Central handelt.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[UnitsOfMeasure abrufen](../api/dynamics-unitsofmeasure-get.md)|unitsOfMeasure|Ruft ein Maßeinheits Objekt ab.|
|[Post unitsOfMeasure](../api/dynamics-create-unitsofmeasure.md)|unitsOfMeasure|Erstellt ein Maßeinheits Objekt.|
|[Patch-unitsOfMeasure](../api/dynamics-unitsofmeasure-update.md)|unitsOfMeasure|Aktualisiert ein Maßeinheits Objekt.|
|[UnitsOfMeasure löschen](../api/dynamics-unitsofmeasure-delete.md)|Keine|Löscht ein Maßeinheits Objekt.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|GUID|Die eindeutige ID des unitsOfMeasure. Nicht bearbeitbar.|
|code|string|Gibt den Code für die Maßeinheit an.|
|displayName|string|Gibt den Anzeigenamen des Maßeinheiten an.|
|internationalStandardCode|string|Gibt den Code für die Maßeinheit an, der gemäß dem UNECE-Rec20-Standard in Verbindung mit dem elektronischen Senden von Verkaufsdokumenten ausgedrückt wird.|
|lastModifiedDateTime|DateTime|Die letzte DateTime, die die Maßeinheit geändert wurde. Schreibgeschützt.|  


## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der **unitsOfMeasure** -Ressource.

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "internationalStandardCode": "string",
  "lastModifiedDateTime": "datetime"
}

```
