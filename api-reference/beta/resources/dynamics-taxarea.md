---
title: taxAreas-Ressourcentyp
description: Ein Steuerbereich.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: aeda0ca136c178355a8a8f9589eb7410399ef62a
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365451"
---
# <a name="taxareas-resource-type"></a>taxAreas-Ressourcentyp
Stellt einen Ressourcentyp für Steuerbereiche in Dynamics 365 Business Central dar.

## <a name="methods"></a>Methoden
| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[TaxAreas abrufen](../api/dynamics-taxarea-get.md)|taxAreas|Ruft ein Steuerbereichs Objekt ab.|
|[Post taxAreas](../api/dynamics-create-taxarea.md)|taxAreas|Erstellt ein Steuerbereich-Objekt.|
|[Patch-taxAreas](../api/dynamics-taxarea-update.md)|taxAreas|Aktualisiert ein Steuerbereichs Objekt.|
|[TaxAreas löschen](../api/dynamics-taxarea-delete.md)|Keine|Löscht ein Steuerbereichs Objekt.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|GUID|Die eindeutige ID des Steuerbereichs. Nicht bearbeitbar.|
|code|Zeichenfolge, maximale Größe 20| Der Code des Steuerbereichs.|
|displayName|Zeichenfolge, maximale Größe 50| Der Anzeigename des Steuerbereichs.|
|taxType|string|Der Steuertyp des Steuerbereichs.|
|lastModifiedDateTime|DateTime|Der letzte DateTime-Steuerbereich wurde geändert. Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.


```json
{
  "id": "GUID",
  "code": "String",
  "displayName": "String",
  "taxType": "String",
  "lastModifiedDateTime": "datetime"
}
```


