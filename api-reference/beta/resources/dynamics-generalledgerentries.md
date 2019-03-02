---
title: generalLedgerEntries-Ressourcentyp
description: Ein Hauptbuch-Eintrag in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0a5701451bf96773428b12b6bb715320e2ba81b5
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365759"
---
# <a name="generalledgerentries-resource-type"></a>generalLedgerEntries-Ressourcentyp
Stellt ein generalLedgerEntry-Objekt in Dynamics 365 Business Central dar.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:-------------|:-------------|:----------|
|[GeneralLedgerEntries abrufen](../api/dynamics-generalledgerentries-get.md)|generalLedgerEntries|Ein G/L-Eintrags Objekt abrufen.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft           | Typ                  |Beschreibung                                  |
|:-------------------|:----------------------|:--------------------------------------------|
|id                  |numerischen                |Die eindeutige ID des G/L-Eintrags.              |
|postingDate         |date                   |Gibt das Buchungsdatum des Fibu-Eintrags an. |
|documentNumber      |Zeichenfolge, maximale Größe 20|Gibt die Dokumentnummer des G/L-Eintrags an.|
|documentType        |string                 |Gibt den Dokumenttyp des G/L-Eintrags an.|
|accountId           |GUID                   |Gibt die Konto-Nr. des G/L-Eintrags an.    |
|accountNumber       |Zeichenfolge, maximale Größe 20|Gibt die accountNumber des G/L-Eintrags an.|
|description         |Zeichenfolge, maximale Größe 50|Gibt die Beschreibung des G/L-Eintrags an.  |
|debitAmount         |numerischen                |Gibt die debitAmount des G/L-Eintrags an.  |
|creditAmount        |numerischen                |Gibt die creditAmount des G/L-Eintrags an. |
|lastModifiedDateTime|DateTime               |Die letzte DateTime, die der G/L-Eintrag geändert wurde.|


## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.


```json
{
  "id": "int",
  "postingDate": "Date",
  "documentNumber": "string",
  "documentType": "string",
  "accountId": "GUID",
  "accountNumber": "string",
  "description": "string",
  "debitAmount": "decimal",
  "creditAmount": "decimal",
  "lastModifiedDateTime": "datetime"
}

```

