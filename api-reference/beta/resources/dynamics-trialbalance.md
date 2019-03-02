---
title: trialBalance-Ressourcentyp
description: Ein Test-Balance-Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 1a7e906e50ddf39e4c9e2d3d9dde11226c7ec662
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365325"
---
# <a name="trialbalance-resource-type"></a>trialBalance-Ressourcentyp
Stellt einen Test Saldo in Dynamics 365 Business Central dar.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[TrialBalance abrufen](../api/dynamics-trialbalance-get.md)|trialBalance|Ruft ein Test Balance-Objekt ab.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|number|string|Die sachKontonummer für das trialBalance-Element|
|accountId|GUID|Der eindeutige Bezeichner für das Sachkonto des Record-Elements.|
|accountType|string|Der Kontotyp des Sachkontos des Datensatzes.|
|Anzeige|string|Der sachKontoname für das trialBalance-Element.|
|totalDebit|string|Stellt den gesamten Sollbetrag im sachKonto dar.|
|totalCredit|string|Stellt den gesamten Guthabenbetrag im sachKonto dar.|
|balanceAtDateDebit|string|Stellt einen positiven Saldo in einem sachKonto dar.|
|balanceAtDateCredit|string|Stellt einen negativen Saldo in einem sachKonto dar.|
|dateFilter|date|Der Datumsfilter, der zum Berechnen der trialBalance-Elemente verwendet wird.|


## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.


```json
{
    "number": "string",
    "accountId": "GUID",
    "accountType": "string",
    "display": "string",
    "totalDebit": "string",
    "totalCredit": "string",
    "balanceAtDateDebit": "string",
    "balanceAtDateCredit": "string",
    "dateFilter": "date"
}

```

