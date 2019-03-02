---
title: Ressourcentyp "Companies"
description: Ein Unternehmen in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: f1faca36af25bc8cb3e9019e0dc5b4460991e70d
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365682"
---
# <a name="companies-resource-type"></a>Ressourcentyp "Companies"
Stellt einen Ressourcentyp für Unternehmen in Dynamics 365 Business Central dar. 

## <a name="methods"></a>Methoden

| Methode         | Rückgabetyp  |Beschreibung|
|:---------------|:-------------|:----------|
|[Firmen abrufen](../api/dynamics-companies-get.md)|Unternehmen|Holen Sie sich ein Unternehmen.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft        | Typ |Beschreibung                             |
|:----------------|:-----|:---------------------------------------|
|id               |GUID  |Die eindeutige ID des Unternehmens. Schreibgeschützt.|
|name             |string|Gibt das Unternehmen an.                  |
|displayName      |string|Gibt den Anzeigenamen des Unternehmens an.     |
|systemVersion    |string|Gibt die interne Version des Unternehmens an.|
|businessProfileId|string|Gibt die Geschäftsprofil-ID an, die mit dem Unternehmen verknüpft ist.|


## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung des Unternehmens.

```json
{
  "id": "GUID",
  "name": "string",
  "displayName": "string",
  "systemVersion": "string",
  "businessProfileId": "string"
}

```


