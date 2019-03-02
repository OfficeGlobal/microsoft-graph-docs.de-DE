---
title: Ressourcentyp "vendors"
description: Ein Vendor-Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 1cec20dee4a124bb704d60ceb8229ea820aa55b0
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365661"
---
# <a name="vendors-resource-type"></a>Ressourcentyp "vendors"
Stellt einen Anbieter in Dynamics 365 Business Central dar.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Kreditoren abrufen](../api/dynamics-vendor-get.md)|Anbieter|Ruft ein Vendor-Objekt ab.|
|[Post-Kreditoren](../api/dynamics-create-vendor.md)|Anbieter|Erstellt ein Vendor-Objekt.|
|[Patch-Anbieter](../api/dynamics-vendor-update.md)|Anbieter|Aktualisiert ein Vendor-Objekt.|
|[Kreditor löschen](../api/dynamics-vendor-delete.md)|Keine|Löscht ein Vendor-Objekt.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|GUID|Die eindeutige ID des Kreditors. Nicht bearbeitbar.|
|number|string|Die Kreditornummer.|
|displayName|string|Der Anzeigename des Anbieters.|
|address|[Navigations. PostalAddress](../resources/dynamics-complextypes.md)|Die Adresse des Kreditors.|
|PhoneNumber|string|Die Telefonnummer des Kreditors.|
|email|string|Die e-Mail-Adresse des Anbieters.|
|Website|string|Die Websiteadresse des Anbieters.|
|taxRegistrationNumber|string|Die Steuernummer des Kreditors.|
|currencyId|GUID|Die Standard-Währungscode-ID für den Kreditor.|
|currencyCode|string|Der Standardwährungscode für den Kreditor.|
|irs1099Code|string|Gibt einen 1099-Code für den Kreditor an. Nur uns.|
|paymentTermsId|GUID|Die Standard-Zahlungs Bedingungs-ID für den Kreditor.|
|paymentMethodId|GUID|Die Standard-Zahlungsmethoden-ID für den Kreditor.|
|taxLiable|Boolescher Wert|Gibt an, ob der Verkäufer steuerpflichtig ist.|
|gesperrt|string|Gibt an, welche Transaktionen mit dem Kreditor, der nicht gebucht werden kann. Akzeptierte Werte sind leer, Zahlung oder alle|
|Ausgleich|decimal|Der Saldo des Kreditors. Schreibgeschützt.|
|lastModifiedDateTime|DateTime|Die letzte DateTime, die der Kreditor geändert wurde. Schreibgeschützt.|  


## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung des Anbieters.

```json
{
  "id": "GUID",
  "number": "string",
  "displayName": "string",
  "address": "NAV.PostalAddress",
  "phoneNumber": "string",
  "email": "string",
  "website": "string",
  "taxRegistrationNumber": "string",
  "currencyId": "GUID",
  "currencyCode": "string",
  "irs1099Code": "string",
  "paymentTermsId": "GUID",
  "paymentMethodId": "GUID",
  "taxLiable": "boolean",
  "blocked": "string",
  "balance": "decimal",
  "lastModifiedDateTime": "datetime"
}

```

