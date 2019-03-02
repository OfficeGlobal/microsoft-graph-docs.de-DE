---
title: paymentTerms-Ressourcentyp
description: Ein Zahlungsbedingungen-Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4ed1f3791474cf6e29038e75fcd3625e4da300a0
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365640"
---
# <a name="paymentterms-resource-type"></a>paymentTerms-Ressourcentyp
Stellt eine Zahlungsbedingung in Dynamics 365 Business Central dar.

## <a name="methods"></a>Methoden

| Methode                                                      | Rückgabetyp|Beschreibung            |
|:------------------------------------------------------------|:-----------|:----------------------|
|[PaymentTerms abrufen](../api/dynamics-paymentterms-get.md)      |paymentTerms|Rufen Sie ein Zahlungsbedingungen-Objekt ab.   |
|[Post paymentTerms](../api/dynamics-create-paymentterms.md)  |paymentTerms|Erstellen eines Zahlungs Begriffs-Objekts.|
|[Patch-paymentTerms](../api/dynamics-paymentterms-update.md) |paymentTerms|Aktualisieren eines Zahlungs Begriffs-Objekts.|
|[PaymentTerms löschen](../api/dynamics-paymentterms-delete.md)|Keine        |Löschen eines Zahlungs Begriffs-Objekts.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft                     | Typ     |Beschreibung                                                |
|:-----------------------------|:-------|:----------------------------------------------------------|
|id                            |GUID    |Die eindeutige ID des paymentTerms. Nicht bearbeitbar.           |
|code                          |string  |Gibt den Zahlungs Begriffs Code an.                           |
|displayName                   |string  |Gibt den Anzeigenamen für den Zahlungs Ausdruck an.                   |
|dueDateCalculation            |string  |Gibt die Formel an, die verwendet wird, um das Datum zu berechnen, an dem eine Zahlung getätigt werden muss.|
|discountDateCalculation       |string  |Gibt die Formel an, die verwendet wird, um das Datum zu berechnen, an dem eine Zahlung getätigt werden muss, um einen Rabatt zu erhalten.|
|discountPercent               |decimal |Gibt den Rabattprozentsatz an, der für die vorzeitige Zahlung eines Rechnungsbetrags angewendet wird.|
|calculateDiscountOnCreditMemos|Boolescher Wert |Gibt an, ob der Rabatt auf Gutschriften angewendet werden soll. **True** gibt an, dass ein Rabatt gewährt wird, **false** gibt an, dass kein Preisnachlass gewährt wird.|
|lastModifiedDateTime          |DateTime|Die letzte DateTime, die der paymentTerms geändert wurde. Schreibgeschützt.|  


## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung des paymentTerms.


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "dueDateCalculation": "string",
  "discountDateCalculation": "string",
  "discountPercent": "decimal",
  "calculateDiscountOnCreditMemos": "boolean",
  "lastModifiedDateTime": "datetime"
}

```
