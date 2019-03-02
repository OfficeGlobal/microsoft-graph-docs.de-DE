---
title: taxGroups-Ressourcentyp
description: Ein Steuergruppen Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: bdfbec8f5373637924262388dab0e9c74c363af9
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366690"
---
# <a name="taxgroups-resource-type"></a>taxGroups-Ressourcentyp
Stellt einen taxGroups-Ressourcentyp in Dynamics 365 Business Central dar.

## <a name="methods"></a>Methoden
| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[TaxGroups abrufen](../api/dynamics-taxgroups-get.md)|taxGroups|Ruft ein Steuergruppen Objekt ab.|
|[Post taxGroups](../api/dynamics-create-taxgroups.md)|taxGroups|Erstellt ein Steuergruppen Objekt.|
|[Patch-taxGroups](../api/dynamics-taxgroups-update.md)|taxGroups|Aktualisiert ein Steuergruppen Objekt.|
|[TaxGroups löschen](../api/dynamics-taxgroups-delete.md)|Keine|Löscht ein Steuergruppen Objekt.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|GUID|Die eindeutige ID des taxGroup. Schreibgeschützt.|
|code|string|Gibt die Steuergruppe an.|
|displayName|string|Gibt den Anzeigenamen der Steuergruppe an.|
|taxType|string|Gibt den Steuertyp für die Gruppe an.|
|lastModifiedDateTime|DateTime|Die letzte DateTime, die die Steuergruppe geändert wurde. Schreibgeschützt.|  


## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung des taxGroup.

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "taxType": "string",
  "lastModifiedDateTime": "datetime"
}

```


