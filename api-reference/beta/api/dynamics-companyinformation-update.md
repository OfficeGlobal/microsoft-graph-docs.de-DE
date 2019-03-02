---
title: CompanyInformation aktualisieren
description: Aktualisiert ein Unternehmens Informationsobjekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 82833c7b9d3d329b5dfb566f8e4b9b72d47c49ab
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366620"
---
# <a name="update-companyinformation"></a><span data-ttu-id="7635f-103">CompanyInformation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7635f-103">Update companyInformation</span></span>
<span data-ttu-id="7635f-104">Aktualisieren der Eigenschaften eines Unternehmens Informationsobjekts für Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="7635f-104">Update the properties of a company information object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="7635f-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7635f-105">Permissions</span></span>
<span data-ttu-id="7635f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7635f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7635f-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7635f-108">Permission type</span></span> |<span data-ttu-id="7635f-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7635f-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="7635f-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7635f-110">Delegated (work or school account)</span></span>|<span data-ttu-id="7635f-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7635f-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="7635f-112">Delegiert (persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="7635f-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="7635f-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7635f-113">Not supported.</span></span>|
|<span data-ttu-id="7635f-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7635f-114">Application</span></span>|<span data-ttu-id="7635f-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7635f-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7635f-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7635f-116">HTTP request</span></span>
```
PATCH /financials/companies('{id}')/companyInformation('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7635f-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="7635f-117">Optional query parameters</span></span>
<span data-ttu-id="7635f-118">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7635f-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7635f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7635f-119">Request headers</span></span>
|<span data-ttu-id="7635f-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7635f-120">Header</span></span>        |<span data-ttu-id="7635f-121">Wert</span><span class="sxs-lookup"><span data-stu-id="7635f-121">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="7635f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7635f-122">Authorization</span></span> |<span data-ttu-id="7635f-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7635f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7635f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7635f-125">Content-Type</span></span>  |<span data-ttu-id="7635f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7635f-126">application/json</span></span>         |
|<span data-ttu-id="7635f-127">If-Match</span><span class="sxs-lookup"><span data-stu-id="7635f-127">If-Match</span></span>      |<span data-ttu-id="7635f-128">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7635f-128">Required.</span></span> <span data-ttu-id="7635f-129">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag nicht mit dem aktuellen Tag in der **companyInformation**übereinstimmt, wird die **companyInformation** nicht aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="7635f-129">When this request header is included and the eTag provided does not match the current tag on the **companyInformation**, the **companyInformation** will not be updated.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7635f-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7635f-130">Request body</span></span>
<span data-ttu-id="7635f-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="7635f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="7635f-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="7635f-134">Response</span></span>
<span data-ttu-id="7635f-135">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und ein aktualisiertes **companyInformation** -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7635f-135">If successful, this method returns a `200 OK` response code and an updated an **companyInformation** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7635f-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7635f-136">Example</span></span>

<span data-ttu-id="7635f-137">**Anforderung**</span><span class="sxs-lookup"><span data-stu-id="7635f-137">**Request**</span></span>

<span data-ttu-id="7635f-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7635f-138">Here is an example of the request.</span></span>
```json
PATCH https://graph.microsoft.com/beta/financials/companies('{id}')/companyInformation('{id}')
Content-type: application/json

{
  "displayName": "CRONUS USA, LTD.",
  "website": "www.cronuscorp.net"
}
```

<span data-ttu-id="7635f-139">**Antwort**</span><span class="sxs-lookup"><span data-stu-id="7635f-139">**Response**</span></span>

<span data-ttu-id="7635f-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7635f-140">Here is an example of the response.</span></span> 

> <span data-ttu-id="7635f-141">**Hinweis**: das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="7635f-141">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7635f-142">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="7635f-142">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "displayName": "CRONUS USA, LTD.",
  "address": {
    "street": "7122 South Ashford Street\r\nWestminster",
    "city": "Atlanta",
    "state": "GA",
    "countryLetterCode": "US",
    "postalCode": "31772"
  },
  "phoneNumber": "+1 425 555 0100",
  "faxNumber": "+1 425 555 0101",
  "email": "",
  "website": "www.cronuscorp.net",
  "taxRegistrationNumber": "",
  "currencyCode": "USD",
  "currentFiscalYearStartDate": "2018-01-01",
  "industry": "",
  "picture@odata.mediaReadLink": "https://api.financials.dynamics.com/v1.0/api/beta/companies('{id}')/companyInformation('{id}')/picture",
  "lastModifiedDateTime": "2017-03-16T14:57:19.497Z"
  }
```
