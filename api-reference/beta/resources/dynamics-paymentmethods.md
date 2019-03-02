---
title: paymentMethods-Ressourcentyp
description: Ein Zahlungsmethoden Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 1e4cd044d4b552a9239b742efb302633524ce22b
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366648"
---
# <a name="paymentmethods-resource-type"></a>paymentMethods-Ressourcentyp
Stellt eine Zahlungsmethode in Dynamics 365 Business Central dar, beispielsweise PayPal, Kreditkarte und Bankkonto.

## <a name="methods"></a>Methoden

| Methode                                                          | Rückgabetyp  |Beschreibung             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[PaymentMethods abrufen](../api/dynamics-paymentmethods-get.md)      |paymentMethods|Ruft ein Zahlungsmethoden Objekt ab.   |
|[Post paymentMethods](../api/dynamics-create-paymentmethods.md)  |paymentMethods|Erstellt ein Zahlungsmethoden Objekt.|
|[Patch-paymentMethods](../api/dynamics-paymentmethods-update.md) |paymentMethods|Aktualisiert ein Zahlungsmethoden Objekt.|
|[PaymentMethods löschen](../api/dynamics-paymentmethods-delete.md)|Keine          |Löscht ein Zahlungsmethoden Objekt.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft           | Typ   |Beschreibung                                                  |
|:-------------------|:-------|:------------------------------------------------------------|
|id                  |GUID    |Die eindeutige ID des paymentMethods. Nicht bearbeitbar.           |
|code                |string  |Gibt den Zahlungsmethoden Code an.                           |
|displayName         |string  |Gibt den Anzeigenamen der Zahlungsmethode an.                   |
|lastModifiedDateTime|DateTime|Die letzte DateTime, die die Zahlungsmethode geändert wurde. Schreibgeschützt.|  


## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung des paymentMethods.


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```
