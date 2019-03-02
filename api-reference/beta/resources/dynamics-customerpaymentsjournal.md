---
title: customerPaymentJournals-Ressourcentyp
description: Ein Kunden Zahlungsjournal in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: a8b01124db732866e1a7b971af57d7e0a2b692e1
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365738"
---
# <a name="customerpaymentsjournals-resource-type"></a>customerPaymentsJournals-Ressourcentyp
Stellt ein Debitoren Zahlungsjournal in Dynamics 365 Business Central dar.

## <a name="methods"></a>Methoden

| Methode               | Rückgabetyp             |Beschreibung                      |
|:---------------------|:------------------------|:--------------------------------|
|[CustomerPaymentJournals abrufen](../api/dynamics-customerpaymentsjournal-get.md)      |customerPaymentJournals|Ruft ein Debitoren Zahlungsjournal ab.   |
|[Post customerPaymentJournals](../api/dynamics-create-customerpaymentsjournal.md)  |customerPaymentJournals|Erstellt ein Debitoren Zahlungsjournal.|
|[Patch-customerPaymentJournals](../api/dynamics-customerpaymentsjournal-update.md) |customerPaymentJournals|Aktualisiert ein Debitoren Zahlungsjournal.|
|[CustomerPaymentJournals löschen](../api/dynamics-customerpaymentsjournal-delete.md)|Keine                     |Löscht ein Debitoren-Zahlungs Blatt.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft           | Typ                  |Beschreibung                                                             |
|:-------------------|:----------------------|:-----------------------------------------------------------------------|
|id                  |GUID                   |Die eindeutige ID des Debitoren-Zahlungs Blatts. Nicht bearbeitbar.           |
|code                |Zeichenfolge, maximale Größe 10| Der Code des Debitoren-Zahlungs Blatts.                             |
|displayName         |Zeichenfolge, maximale Größe 50| Der Anzeigename des Debitoren-Zahlungs Blatts.                     |
|lastModifiedDateTime|DateTime               |Die letzte Uhrzeit, zu der das Debitoren Zahlungsjournal geändert wurde. Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.


```json
{
  "id": "GUID",
  "code": "String",
  "displayName": "String",
  "lastModifiedDateTime": "datetime"
}
```

