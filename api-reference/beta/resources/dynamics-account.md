---
title: Ressourcentyp "Accounts"
description: Ein Account-Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4252c20e9d11f67a6de40871b1649a165cbd787c
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365458"
---
# <a name="accounts-resource-type"></a>Ressourcentyp "Accounts"
Stellt ein Account-Objekt in Dynamics 365 Business Central dar.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Konten abrufen](../api/dynamics-account-get.md)|Konten|Get Accounts-Objekt.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|GUID|Die eindeutige ID des Kontos.|
|number|Zeichenfolge, maximale Größe 20|Gibt die Nummer des Sachkontos an.|
|displayName|Zeichenfolge, maximale Größe 50|Gibt den Namen des Sachkontos an.|
|category|Zeichenfolge, maximale Größe 20|Gibt die Kategorie des Sachkontos an.|
|subCategory|Zeichenfolge, maximale Größe 80|Gibt die Unterkategorie der Kontokategorie des Sachkontos an.|
|gesperrt|Boolescher Wert|Gibt an, dass Posten nicht in das Sachkonto gebucht werden können. **True** gibt an, dass das Konto gesperrt ist und das Veröffentlichen nicht zulässig ist.|
|lastModifiedDateTime|DateTime|Die letzte Uhrzeit, zu der das Konto geändert wurde.|


## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.


```json
{
  "id": "GUID",
  "number": "string",
  "displayName": "string",
  "category": "string",
  "subCategory": "string",
  "blocked": "boolean",
  "lastModifiedDateTime": "datetime"
}

```
