---
title: Ressourcentyp "Währungen"
description: Ein Currency-Objekt in Dynamics 365 Business Central
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: c0d15b8d20e99537cb2f567a9f8fe12b45dbd389
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366627"
---
# <a name="currencies-resource-type"></a>Ressourcentyp "Währungen"
Stellt eine Währung dar, die in Dynamics 365 Business Central verwendet wird.

## <a name="methods"></a>Methoden
| Methode                                                  |Rückgabetyp|Beschreibung       |
|:--------------------------------------------------------|:----------|:-----------------|
|[Währungen abrufen](../api/dynamics-currencies-get.md)      |Währungen |Holen Sie sich eine Währung.   |
|[Post Währungen](../api/dynamics-create-currencies.md)  |Währungen |Erstellen Sie eine Währung.|
|[Patch-Währungen](../api/dynamics-currencies-update.md) |Währungen |Aktualisieren einer Währung.|
|[Währungen löschen](../api/dynamics-currencies-delete.md)|Keine       |Eine Währung löschen.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft              | Typ   |Beschreibung                                                   |
|:----------------------|:-------|:-------------------------------------------------------------|
|id                     |GUID    |Die eindeutige ID der Währung. Nicht bearbeitbar.                  |
|code                   |string  |Gibt den Währungscode an.                                  |
|displayName            |string  |Gibt den Anzeigenamen der Währung an.                          |
|Symbol                 |string  |Gibt das Symbol für diese Währung an, das in Schecks angezeigt wird.|
|amountDecimalPlaces    |string  |Gibt die Anzahl der Dezimalstellen an, die vom System für Beträge für diese Währung angezeigt werden.|
|amountRoundingPrecision|decimal |Gibt die Größe des Intervalls an, das beim Runden von Beträgen für diese Währung verwendet werden soll.|
|lastModifiedDateTime   |DateTime|Die letzte Uhrzeit, zu der die Währung geändert wurde. Schreibgeschützt.       |  


## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Währungen.


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "symbol": "string",
  "amountDecimalPlaces": "string",
  "amountRoundingPrecision": "decimal",
  "lastModifiedDateTime": "datetime"
}

```

