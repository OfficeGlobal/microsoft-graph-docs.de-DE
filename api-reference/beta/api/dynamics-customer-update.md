---
title: Kunden aktualisieren
description: Aktualisiert ein Kundenobjekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0d3c69d3e8ef7951fceefba875dbab2d9949db59
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365675"
---
# <a name="update-customers"></a><span data-ttu-id="1f43d-103">Kunden aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1f43d-103">Update customers</span></span>
<span data-ttu-id="1f43d-104">Aktualisieren der Eigenschaften eines Customer-Objekts für Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="1f43d-104">Update the properties of a customer object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f43d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1f43d-105">Permissions</span></span>
<span data-ttu-id="1f43d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f43d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f43d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1f43d-108">Permission type</span></span> |<span data-ttu-id="1f43d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1f43d-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="1f43d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1f43d-110">Delegated (work or school account)</span></span>|<span data-ttu-id="1f43d-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f43d-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="1f43d-112">Delegiert (persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="1f43d-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="1f43d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1f43d-113">Not supported.</span></span>|
|<span data-ttu-id="1f43d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1f43d-114">Application</span></span>|<span data-ttu-id="1f43d-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f43d-115">Financials.ReadWrite.All</span></span>|
## <a name="http-request"></a><span data-ttu-id="1f43d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f43d-116">HTTP request</span></span>

```
PATCH /financials/companies('{id}')/customers('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1f43d-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1f43d-117">Optional query parameters</span></span>
<span data-ttu-id="1f43d-118">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1f43d-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1f43d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1f43d-119">Request headers</span></span>
|<span data-ttu-id="1f43d-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1f43d-120">Header</span></span>         |<span data-ttu-id="1f43d-121">Wert</span><span class="sxs-lookup"><span data-stu-id="1f43d-121">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="1f43d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f43d-122">Authorization</span></span>  |<span data-ttu-id="1f43d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1f43d-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="1f43d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1f43d-125">Content-Type</span></span>   |<span data-ttu-id="1f43d-126">Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="1f43d-126">application/json.</span></span>         |
|<span data-ttu-id="1f43d-127">If-Match</span><span class="sxs-lookup"><span data-stu-id="1f43d-127">If-Match</span></span>       |<span data-ttu-id="1f43d-128">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1f43d-128">Required.</span></span> <span data-ttu-id="1f43d-129">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag nicht mit dem aktuellen Tag für die **Kunden**übereinstimmt, werden die **Kunden** nicht aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="1f43d-129">When this request header is included and the eTag provided does not match the current tag on the **customers**, the **customers** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f43d-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1f43d-130">Request body</span></span>
<span data-ttu-id="1f43d-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="1f43d-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="1f43d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f43d-134">Response</span></span>
<span data-ttu-id="1f43d-135">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes **Customers** -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1f43d-135">If successful, this method returns a `200 OK` response code and an updated **customers** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f43d-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1f43d-136">Example</span></span>

<span data-ttu-id="1f43d-137">**Anforderung**</span><span class="sxs-lookup"><span data-stu-id="1f43d-137">**Request**</span></span>

<span data-ttu-id="1f43d-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1f43d-138">Here is an example of the request.</span></span>

```json
PATCH https://graph.microsoft.com/beta/financials/companies('{id}')/customers('{id}')
Content-type: application/json

{
  "displayName": "Coho Winery Inc.",
  "phoneNumber": "(555) 555-1234"
}
```

<span data-ttu-id="1f43d-139">**Antwort**</span><span class="sxs-lookup"><span data-stu-id="1f43d-139">**Response**</span></span>

<span data-ttu-id="1f43d-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1f43d-140">Here is an example of the response.</span></span> 

> <span data-ttu-id="1f43d-141">**Hinweis**: das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="1f43d-141">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1f43d-142">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="1f43d-142">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "number": "10000",
  "displayName": "Coho Winery Inc.",
  "type": "Company",
  "address": {
    "street": "192 Market Square",
    "city": "Atlanta",
    "state": "GA",
    "countryLetterCode": "US",
    "postalCode": "31772"
  },
  "phoneNumber": "(555) 555-1234"
  "email": "jim.glynn@cronuscorp.net",
  "website": "",
  "taxLiable": true,
  "taxAreaId": "taxAreaId-value",
  "taxAreaDisplayName": "tax area",
  "taxRegistrationNumber": "28012001T",
  "currencyId": "currencyId-value",
  "currencyCode": "USD",
  "paymentTermsId": "paymentTermsId-value",
  "shipmentMethodId": "shipmentMethodId-value",
  "paymentMethodId": "paymentMethod-value",
  "blocked": " ",
  "balance": 0,
  "overdueAmount": 0
  "totalSalesExcludingTax": 0,
  "lastModifiedDateTime": "2017-03-07T00:35:28.983Z"
}
```


