---
title: Ressourcentyp "Customers"
description: Stellt einen Kunden in Dynamics 365 Business Central dar.
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: e4daa28018001fb6cb6e4866bedf8e256a72abef
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365934"
---
# <a name="customers-resource-type"></a>Ressourcentyp "Customers"
Stellt einen Kunden in Dynamics 365 Business Central dar.

## <a name="methods"></a>Methoden

| Methode                                              |Rückgabetyp| Beschreibung      |
|:----------------------------------------------------|:----------|:-----------------|
|[Kunden abrufen](../api/dynamics-customer-get.md)      |Kunden   |Ruft einen Kunden ab.   |
|[Kunden erstellen](../api/dynamics-create-customer.md)|Kunden   |Erstellt einen Kunden.|
|[Kunden aktualisieren](../api/dynamics-customer-update.md)|Kunden   |Aktualisiert einen Kunden.|
|[Kunden löschen](../api/dynamics-customer-delete.md)|Keine        |Löscht einen Kunden.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft    | Typ     |Beschreibung|
|:------------|:---------|:----------|
|id           |GUID      |Die eindeutige ID des Elements. Nicht bearbeitbar.|
|number       |string    |Die Kundennummer.|
|displayName  |string    |Gibt den Namen des Kunden an. Dieser Name wird in allen Verkaufsdokumenten des Kunden angezeigt.|
|type         |string    |Gibt den Kundentyp an, kann "Company" oder "Person" sein.|
|address      |[Navigations. PostalAddress](../resources/dynamics-complextypes.md)|Gibt die Adresse des Kunden an. Diese Adresse wird in allen Verkaufsdokumenten des Kunden angezeigt.|
|PhoneNumber  |string    |Gibt die Telefonnummer des Kunden an.|
|email        |string    |Gibt die e-Mail-Adresse des Kunden an.|
|Website      |string    |Gibt die Adresse der Startseite des Kunden an.|
|taxLiable    |Boolescher Wert   |Gibt an, ob der Kunde oder Lieferant für die Mehrwertsteuer haftet. Wird auf **true** festgelegt, wenn der Kunde steuerpflichtig ist.|
|taxAreaId    |GUID      |Gibt an, zu welchem Steuerbereich der Kunde gehört.|
|taxAreaDisplayName|string|Der Anzeigename des Steuerbereichs, zu dem der Kunde gehört, angegeben.|
|taxRegistrationNumber|Zeichenfolge, maximale Größe 20|Die Steuernummer des Kunden wurde angegeben.|
|currencyId   |GUID      |Gibt an, welche Währung der Kunde verwendet.|
|currencyCode |numerischen   |Der Standardwährungscode für den Kunden.|
|paymentTermsId|GUID     |Gibt an, welche Zahlungsfrist der Kunde verwendet.|
|paymentMethodId|GUID    |Gibt an, welche Zahlungsmethode der Kunde verwendet.|
|shipmentMethodId|GUID   |Gibt an, welche Transportmethode der Kunde verwendet.|
|gesperrt      |string    |Gibt an, dass Transaktionen mit dem Kunden nicht gebucht werden können. Auf **alle**festlegen, wenn der Kunde blockiert ist, auf leer gesetzt, wenn nicht blockiert.|
|Ausgleich      |numerischen   |Gibt den Zahlungsbetrag an, den der Kunde für abgeschlossene Verkäufe schuldet. Dieser Wert wird auch als Saldo des Kunden bezeichnet. Schreibgeschützt.|
|overdueAmount|numerischen   |Gibt den fälligen Betrag des Debitors an.|
|totalSalesExcludingTax|numerischen|Gibt den Gesamtumsatz ohne Steuern des Kunden an.|
|lastModifiedDateTime|DateTime|Die letzte DateTime, für die der Kunde geändert wurde. Schreibgeschützt.|  


## <a name="relationships"></a>Beziehungen
In der Tabelle Währungen muss eine Währung (currencyCode) vorhanden sein.

In der Tabelle mit den Zahlungsbedingungen muss ein Zahlungs Ausdruck (paymentTerms) vorhanden sein.

Eine Transportmethode (shipmentMethod) muss in der Tabelle "Transportmethode" vorhanden sein.

In der Tabelle "Zahlungsmethode" muss eine Zahlungsmethode (paymentMethod) vorhanden sein.

In der Tabelle Steuerbereich muss ein Steuerbereich (taxArea) vorhanden sein.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.


```json
{
    "id": "GUID",
    "number": "string",
    "displayName": "string",
    "type": "string",
    "address": NAV.PostalAddress,
    "phoneNumber": "string",
    "email": "string",
    "website": "string",
    "taxLiable": "boolean",
    "taxAreaId": "GUID",
    "taxAreaDisplayName": "string",
    "taxRegistrationNumber": "string",
    "currencyCode": "string",
    "paymentTermsId": "GUID",
    "shipmentMethodId": "GUID",
    "paymentMethodId":  "GUID",
    "blocked": "string",
    "balance": "decimal",
    "overdueAmount": "numeric",
    "totalSalesExcludingTax": "numeric",
    "lastModifiedDateTime": "datetime"
}


```

