---
title: customerPayments-Ressourcentyp
description: Ein Kunden Zahlungs Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 9063a9066c51956596e4f0aa918a2e7a53bf2ab9
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365612"
---
# <a name="customerpayments-resource-type"></a>customerPayments-Ressourcentyp
Stellt eine Kundenzahlung in Dynamics 365 Business Central dar. Eine Debitorenzahlung wird als Zeile in einer Debitoren Zahlungserfassung eingegeben.

## <a name="methods"></a>Methoden

| Methode         | Rückgabetyp  |Beschreibung|
|:---------------|:-------------|:----------|
|[CustomerPayments abrufen](../api/dynamics-customerpayment-get.md)|customerPayments|Ruft eine Kundenzahlung ab.|
|[Post customerPayments](../api/dynamics-create-customerpayment.md)|customerPayments|Erstellt eine Debitorenzahlung.|
|[Patch-customerPayments](../api/dynamics-customerpayment-update.md)|customerPayments|Aktualisiert eine Kundenzahlung.|
|[CustomerPayments löschen](../api/dynamics-customerpayment-delete.md)|Keine|Löscht eine Debitorenzahlung.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ    |Beschreibung|
|:-------------|:--------|:----------|
|id|GUID|Die eindeutige ID der Debitorenzahlung. Nicht bearbeitbar.|
|journalDisplayName|string|Das Debitoren-Zahlungs Blatt, in dem der Zahlungsdatensatz eine Zeile ist.|
|lineNumber|integer|Die Anzahl der Debitorenzahlung.|
|customerId|GUID|Die eindeutige ID des Debitors, mit dem die Zahlung verbunden ist.|
|customerNumber|Zeichenfolge, maximale Größe 20|Die Nummer des Debitors, mit dem die Zahlung verbunden ist.|
|contactId|Zeichenfolge, maximale Größe 250|Die Exchange-Kontakt-ID für den angegebenen Kunden. Wenn keine Kunden-ID angegeben wird, verwenden wir die Kontakt-ID, um Sie zu finden.|
|postingDate|date|Das Datum, an dem die Debitorenzahlung gebucht wird.|
|documentNumber|Zeichenfolge, maximale Größe 20|Gibt eine Dokumentnummer für die Debitorenzahlung an.|
|externalDocumentNumber|Zeichenfolge, maximale Größe 20|Gibt eine externe Belegnummer für die Debitorenzahlung an.|
|Menge|decimal|Gibt den Gesamtbetrag (einschließlich Mehrwertsteuer) an, aus dem die Debitorenzahlung besteht.|
|appliesToInvoiceId|GUID|Die eindeutige ID der Rechnung, mit der die Zahlung verbunden ist.|
|appliesToInvoiceNumber|Zeichenfolge, maximale Größe 20|Die Nummer der Rechnung, mit der die Zahlung verbunden ist.|
|description|Zeichenfolge, maximale Größe 50|Die Beschreibung der Debitorenzahlung, die vom Benutzer bereitgestellt oder selbst erstellt wurde.|
|Kommentar|Zeichenfolge, maximale Größe 250|Ein benutzerdefinierter Kommentar zur Debitorenzahlung.|
|lastModifiedDateTime|DateTime|Die letzte DateTime, für die die Debitorenzahlung geändert wurde. Schreibgeschützt.|


## <a name="relationships"></a>Beziehungen
Bei einer Debitorenzahlung handelt es sich um eine Unterseite einer Debitoren Zahlungserfassung. Er kann nicht direkt zugegriffen werden.

Eine Debitorenzahlung kann eine "übergeordnete Entität" der Dimensionszeilen sein.

Ein Kunde (customerId) muss in der Customers-Tabelle vorhanden sein.

In der Tabelle "Verkaufsrechnungen" muss eine Rechnung (appliesToInvoiceId) vorhanden sein.


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

```json
{
    "id": "GUID",
    "journalDisplayName": "string",
    "lineNumber": "integer",
    "customerId": "GUID",
    "customerNumber": "string",
    "contactId": "string",
    "postingDate": "date",
    "documentNumber": "string",
    "externalDocumentNumber": "string",
    "amount": "decimal",
    "appliesToInvoiceId": "GUID",
    "appliesToInvoiceNumber": "string",
    "description": "string",
    "comment": "string",
    "lastModifiedDateTime": "datetime"
}
```

