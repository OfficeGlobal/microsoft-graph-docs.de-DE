---
title: shipmentMethods-Ressourcentyp
description: Eine Sendungs Methode in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 2f7ef9611fc85c13ac24c79b292e06a6bdc5d587
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365500"
---
# <a name="shipmentmethods-resource-type"></a>shipmentMethods-Ressourcentyp
Stellt eine Versandmethode in Dynamics 365 Business Central dar, beispielsweise UPS, FedEx und DHL.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[ShipmentMethods abrufen](../api/dynamics-shipmentmethods-get.md)|shipmentMethods|Ruft eine Sendungs Methode ab.|
|[Post shipmentMethods](../api/dynamics-create-shipmentmethods.md)|shipmentMethods|Erstellt eine Transportmethode.|
|[Patch-shipmentMethods](../api/dynamics-shipmentmethods-update.md)|shipmentMethods|Aktualisiert eine Transportmethode.|
|[ShipmentMethods löschen](../api/dynamics-shipmentmethods-delete.md)|Keine|Löscht eine Transportmethode.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|GUID|Die eindeutige ID des shipmentMethod. Nicht bearbeitbar.|
|code|string|Gibt den Code der Transportmethode an.|
|displayName|string|Gibt den Anzeigenamen der Sendungs Methode an.|
|lastModifiedDateTime|DateTime|Die letzte DateTime, die die Sendungs Methode geändert wurde. Schreibgeschützt.|  


## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung des shipmentMethod.

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```


