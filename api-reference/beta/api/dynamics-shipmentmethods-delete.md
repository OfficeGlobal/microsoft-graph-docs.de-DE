---
title: ShipmentMethods löschen
description: Löscht ein Shipment-Methodenobjekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 25d3d5711fab4511395beb0a90fae7760b1d766a
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365402"
---
# <a name="delete-shipmentmethods"></a>ShipmentMethods löschen
Delete a Shipment Method Object from Dynamics 365 Business Central.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp |Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)|
|:---------------|:------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|Financials.ReadWrite.All |
|Delegiert (persönliches Microsoft-Konto|Nicht unterstützt|
|Anwendung|Financials.ReadWrite.All|

## <a name="http-request"></a>HTTP-Anforderung
```
DELETE /financials/companies('{id}')/shipmentMethods('{id}')
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|------|-----|
|Authorization  |Bearer {token}. Erforderlich. |
|If-Match       |Erforderlich. Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag nicht mit dem aktuellen Tag in der **shipmentMethods**übereinstimmt, wird die **shipmentMethods** nicht aktualisiert. |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, wird der Antwortcode ```204,No Content``` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <a name="example"></a>Beispiel

**Anforderung**

Nachfolgend sehen Sie ein Beispiel der Anforderung.

```json
DELETE https://graph.microsoft.com/beta/financials/companies('{id}')/shipmentMethods('{id}')
```

**Antwort** 

Nachfolgend sehen Sie ein Beispiel der Antwort. 

```json
HTTP/1.1 204 No Content
```
