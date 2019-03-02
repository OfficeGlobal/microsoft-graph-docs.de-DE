---
title: Kunden abrufen
description: Ruft ein Customer-Objekt in Dynamics 365 Business Central ab.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0512a493032e738bba41362ecdc40e78de951baf
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365843"
---
# <a name="get-customers"></a><span data-ttu-id="bc24a-103">Kunden abrufen</span><span class="sxs-lookup"><span data-stu-id="bc24a-103">Get customers</span></span>
<span data-ttu-id="bc24a-104">Rufen Sie die Eigenschaften und Beziehungen eines Customer-Objekts für Dynamics 365 Business Central ab.</span><span class="sxs-lookup"><span data-stu-id="bc24a-104">Retrieve the properties and relationships of a customer object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc24a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bc24a-105">Permissions</span></span>
<span data-ttu-id="bc24a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc24a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc24a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bc24a-108">Permission type</span></span> |<span data-ttu-id="bc24a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bc24a-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="bc24a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bc24a-110">Delegated (work or school account)</span></span>|<span data-ttu-id="bc24a-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc24a-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="bc24a-112">Delegiert (persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="bc24a-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="bc24a-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bc24a-113">Not supported.</span></span>|
|<span data-ttu-id="bc24a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bc24a-114">Application</span></span>|<span data-ttu-id="bc24a-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc24a-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc24a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc24a-116">HTTP request</span></span>
```
GET /financials/companies('{id}')/customers('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bc24a-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="bc24a-117">Optional query parameters</span></span>
<span data-ttu-id="bc24a-118">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bc24a-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bc24a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bc24a-119">Request headers</span></span>
|<span data-ttu-id="bc24a-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bc24a-120">Header</span></span>|<span data-ttu-id="bc24a-121">Wert</span><span class="sxs-lookup"><span data-stu-id="bc24a-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="bc24a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc24a-122">Authorization</span></span>  |<span data-ttu-id="bc24a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bc24a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc24a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bc24a-125">Request body</span></span>
<span data-ttu-id="bc24a-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bc24a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc24a-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc24a-127">Response</span></span>
<span data-ttu-id="bc24a-128">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein **Customers** -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bc24a-128">If successful, this method returns a `200 OK` response code and a **customers** object in the response body.</span></span>

<span data-ttu-id="bc24a-129">**Anforderung**</span><span class="sxs-lookup"><span data-stu-id="bc24a-129">**Request**</span></span>

<span data-ttu-id="bc24a-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bc24a-130">Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/customers('{id}')
```

<span data-ttu-id="bc24a-131">**Antwort**</span><span class="sxs-lookup"><span data-stu-id="bc24a-131">**Response**</span></span>

<span data-ttu-id="bc24a-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bc24a-132">Here is an example of the response.</span></span> 

> <span data-ttu-id="bc24a-133">**Hinweis**: das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="bc24a-133">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bc24a-134">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="bc24a-134">All the properties will be returned from an actual call.</span></span>

```json
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
  "currencyId": "currencyId-value",
  "currencyCode": "USD",
  "paymentTermsId": "paymentTermsId-value",
  "shipmentMethodId": "shipmentMethodId-value",
  "paymentMethodId": "paymentMethodId-value",
  "blocked": " ",
  "balance": 0,
  "overdueAmount": 0,
  "totalSalesExcludingTax": 0,
  "lastModifiedDateTime": "2017-03-07T00:35:28.983Z"
}
```

