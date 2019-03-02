---
title: Kunden erstellen
description: Erstellt ein Customer-Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 7bf9a6ec0085deb1557a1d65560974d1498e444c
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365822"
---
# <a name="create-customers"></a><span data-ttu-id="5dd84-103">Kunden erstellen</span><span class="sxs-lookup"><span data-stu-id="5dd84-103">Create customers</span></span>
<span data-ttu-id="5dd84-104">Erstellen Sie ein Kundenobjekt in Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="5dd84-104">Create a customer object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="5dd84-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5dd84-105">Permissions</span></span>
<span data-ttu-id="5dd84-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5dd84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5dd84-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5dd84-108">Permission type</span></span> |<span data-ttu-id="5dd84-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5dd84-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="5dd84-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5dd84-110">Delegated (work or school account)</span></span>|<span data-ttu-id="5dd84-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dd84-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="5dd84-112">Delegiert (persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="5dd84-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="5dd84-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5dd84-113">Not supported.</span></span>|
|<span data-ttu-id="5dd84-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5dd84-114">Application</span></span>|<span data-ttu-id="5dd84-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dd84-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5dd84-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5dd84-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/customers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5dd84-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5dd84-117">Optional query parameters</span></span>
<span data-ttu-id="5dd84-118">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5dd84-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5dd84-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5dd84-119">Request headers</span></span>
|<span data-ttu-id="5dd84-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5dd84-120">Header</span></span>         |<span data-ttu-id="5dd84-121">Wert</span><span class="sxs-lookup"><span data-stu-id="5dd84-121">Value</span></span>                    |
|---------------|-------------------------|
|<span data-ttu-id="5dd84-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5dd84-122">Authorization</span></span>  |<span data-ttu-id="5dd84-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5dd84-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5dd84-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5dd84-125">Content-Type</span></span>   |<span data-ttu-id="5dd84-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5dd84-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="5dd84-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5dd84-127">Request body</span></span>
<span data-ttu-id="5dd84-128">Geben Sie im Anforderungstext eine JSON-Darstellung \*\*\*\* des Customers-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="5dd84-128">In the request body, supply a JSON representation of **customers** object.</span></span>

## <a name="response"></a><span data-ttu-id="5dd84-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="5dd84-129">Response</span></span>
<span data-ttu-id="5dd84-130">Bei erfolgreicher Ausführung gibt diese Methode ```201 Created``` den Antwortcode und \*\*\*\* ein Customers-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5dd84-130">If successful, this method returns ```201 Created``` response code and a **customers** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5dd84-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5dd84-131">Example</span></span>

<span data-ttu-id="5dd84-132">**Anforderung**</span><span class="sxs-lookup"><span data-stu-id="5dd84-132">**Request**</span></span>

<span data-ttu-id="5dd84-133">Hier ist ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5dd84-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/customers
Content-type: application/json

{
  "number": "10000",
  "displayName": "Coho Winery",
  "type": "Company",
  "address": {
    "street": "192 Market Square",
    "city": "Atlanta",
    "state": "GA",
    "countryLetterCode": "US",
    "postalCode": "31772"
  },
  "phoneNumber": "",
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
  "paymentMethodId": "paymentMethodId-value",
  "blocked": " ",
  "overdueAmount": 0,
  "totalSalesExcludingTax": 0,
}

```

<span data-ttu-id="5dd84-134">**Antwort**</span><span class="sxs-lookup"><span data-stu-id="5dd84-134">**Response**</span></span>

<span data-ttu-id="5dd84-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5dd84-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="5dd84-136">**Hinweis**: das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="5dd84-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5dd84-137">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="5dd84-137">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "number": "10000",
  "displayName": "Coho Winery",
  "type": "Company",
  "address": {
    "street": "192 Market Square",
    "city": "Atlanta",
    "state": "GA",
    "countryLetterCode": "US",
    "postalCode": "31772"
  },
  "phoneNumber": "",
  "email": "jim.glynn@cronuscorp.net",
  "website": "",
  "taxLiable": true,
  "taxAreaId": "taxAreaId-value",
  "taxAreaDisplayName": "tax area",
  "taxRegistrationNumber": "28012001T",
  "currencyCode": "USD",
  "blocked": " ",
  "balance": 0,
  "overdueAmount": 0,
  "totalSalesExcludingTax": 0,
  "lastModifiedDateTime": "2017-03-07T00:35:28.983Z"
}

```

