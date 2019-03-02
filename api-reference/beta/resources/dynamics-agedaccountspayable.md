---
title: agedAccountsPayable-Ressourcentyp
description: Ein gealterte Kreditoren Objekte in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 679c24b7ef32ef59b34a5885ea745d8c244376b2
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365906"
---
# <a name="agedaccountspayable-resource-type"></a>agedAccountsPayable-Ressourcentyp
Stellt ein agedAccountsPayable-Objekt in Dynamics 365 Business Central dar, das die Alterung eines Kreditorenkontos anzeigt.

## <a name="methods"></a>Methoden

| Methode         | Rückgabetyp  |Beschreibung|
|:---------------|:-------------|:----------|
|[AgedAccountsPayable abrufen](../api/dynamics-agedaccountspayable-get.md)|agedAccountsPayable|AgedAccountsPayable-Objekt abrufen|

## <a name="properties"></a>Eigenschaften
| Eigenschaft      | Typ     |Beschreibung                                 |
|:--------------|:---------|:-------------------------------------------|
|vendorId       |GUID      |Die eindeutige ID des Anbieters.                    |
|vendorNumber   |string    |Gibt die Nummer des Kreditors an.                  |
|name           |string    |Gibt den Namen des Anbieters an.                    |
|currencyCode   |string    |Gibt die Währung an.                     |
|balanceDue     |numerischen   |Gibt den Gesamtsaldo des Kreditors an.|
|currentAmount  |numerischen   |Gibt den Saldo vor dem ersten Fälligkeits Zeitraum an.|
|period1Amount  |numerischen   |Gibt den Saldo im ersten Alterungszeitraum an.|
|period2Amount  |numerischen   |Gibt den Saldo im zweiten Alterungszeitraum an.|
|period3Amount  |numerischen   |Gibt den Saldo im dritten Alterungszeitraum an.|
|agedAsOfDate   |date|Gibt den Zeitraum an, der zum Berechnen von Alterungs Perioden verwendet wird.|
|periodLengthFilter|string |Gibt die Länge der Punkte an. Zulässige Werte für die Zeiteinheiten sind: D, WD, W, M, Q oder Y. C, was bedeutet, dass die aktuelle Zeiteinheit auf dem Datum basiert, als Präfix für die Zeiteinheit angegeben werden kann.|


## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.


```json
{
    "vendorId": "GUID",
    "vendorNumber": "string",
    "name": "string",
    "currencyCode": "string",
    "balanceDue": "decimal",
    "currentAmount": "decimal",
    "period1Amount": "decimal",
    "period2Amount": "decimal",
    "period3Amount": "decimal",
    "agedAsOfDate": "date",
    "periodLengthFilter": "string"
}

```
