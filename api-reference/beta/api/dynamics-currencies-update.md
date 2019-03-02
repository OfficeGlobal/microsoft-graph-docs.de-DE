---
title: Währungen aktualisieren
description: Aktualisiert ein Currency-Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: e243325d4a7e7536c1e079385f695ef2cc7359c7
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365647"
---
# <a name="update-currencies"></a>Währungen aktualisieren
Aktualisieren der Eigenschaften eines Currency-Objekts für Dynamics 365 Business Central.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp |Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)|
|:---------------|:------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|Financials.ReadWrite.All |
|Delegiert (persönliches Microsoft-Konto|Nicht unterstützt|
|Anwendung|Financials.ReadWrite.All|

## <a name="http-request"></a>HTTP-Anforderung
```
PATCH /financials/companies('{id}')/currencies('{id}')
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile       |Wert                    |
|-------------|-------------------------|
|Authorization|Bearer {token}. Erforderlich.|
|Content-Type |application/json         |
|If-Match     |Erforderlich. Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag nicht mit dem aktuellen Tag in den **Währungen**übereinstimmt, werden die **Währungen** nicht aktualisiert. |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.

## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes **Währungen** -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

**Anforderung**

Nachfolgend sehen Sie ein Beispiel der Anforderung.
```json
PATCH https://graph.microsoft.com/beta/financials/companies('{id}')/currencies('{id}')
Content-type: application/json

{
    "displayName": "United States Dollar"
}
```

**Antwort**

Nachfolgend sehen Sie ein Beispiel der Antwort. 

> **Hinweis**: das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "code": "US",
  "displayName": "United States Dollar",
  "symbol": "$",
  "amountDecimalPlaces": "2:2",
  "amountRoundingPrecision": 0.01,
  "lastModifiedDateTime": "2017-03-22T21:12:18.793Z"
}
```
