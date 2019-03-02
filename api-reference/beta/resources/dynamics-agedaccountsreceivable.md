---
title: agedAccountsReceivable-Ressourcentyp
description: Ein gealterte Forderungen Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: ce5d010c08f956468398082821040e30b4ef2ace
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365577"
---
# <a name="agedaccountsreceivable-resource-type"></a>agedAccountsReceivable-Ressourcentyp
Stellt ein agedAccountsReceivable-Objekt in Dynamics 365 Business Central dar, das die Alterung eines Kundenkontos anzeigt.

## <a name="methods"></a>Methoden

| Methode         | Rückgabetyp  |Beschreibung|
|:---------------|:-------------|:----------|
|[AgedAccountsReceivable abrufen](../api/dynamics-agedaccountsreceivable-get.md)|agedAccountsReceivable|AgedAccountsReceivable-Objekt abrufen|

## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung                                  |
|:---------------|:--------|:--------------------------------------------|
|customerId      |GUID     |Die eindeutige ID des Kunden.                   |
|customerNumber  |string   |Gibt die Nummer des Kunden an.                 |
|name            |string   |Gibt den Namen des Kunden an.                   |
|currencyCode    |string   |Gibt die Währung an.                      |
|balanceDue      |numerischen  |Gibt den Gesamtsaldo des Kunden an.      |
|currentAmount   |numerischen  |Gibt den Saldo für die aktuelle Alterungsperiode an.|
|period1Amount   |numerischen  |Gibt den Saldo im ersten Alterungszeitraum an. |
|period2Amount   |numerischen  |Gibt den Saldo im zweiten Alterungszeitraum an.|
|period3Amount   |numerischen  |Gibt den Saldo im dritten Alterungszeitraum an. |
|agedAsOfDate    |date     |Gibt den Zeitraum an, der zum Berechnen von Alterungs Perioden verwendet wird.|
|periodLengthFilter|string |Gibt die Länge der Punkte an. Zulässige Zeiteinheiten sind: D, WD, W, M, Q und Y. C, was bedeutet, dass die aktuelle Zeiteinheit auf dem Datum basiert, als Präfix für die Zeiteinheit angegeben werden kann.|


## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.


```json
{
    "customerId": "GUID",
    "customerNumber": "string",
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


