---
title: Aktualisieren von Kreditoren
description: Aktualisiert ein Vendor-Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 8e75860cb3c78c16ccb3ac82bec3a972f11ddf51
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365444"
---
# <a name="update-vendors"></a><span data-ttu-id="86f32-103">Aktualisieren von Kreditoren</span><span class="sxs-lookup"><span data-stu-id="86f32-103">Update vendors</span></span>
<span data-ttu-id="86f32-104">Aktualisieren der Eigenschaften eines Vendor-Objekts für Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="86f32-104">Update the properties of a vendor object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="86f32-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="86f32-105">Permissions</span></span>
<span data-ttu-id="86f32-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86f32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86f32-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="86f32-108">Permission type</span></span> |<span data-ttu-id="86f32-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="86f32-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="86f32-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="86f32-110">Delegated (work or school account)</span></span>|<span data-ttu-id="86f32-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86f32-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="86f32-112">Delegiert (persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="86f32-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="86f32-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="86f32-113">Not supported.</span></span>|
|<span data-ttu-id="86f32-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="86f32-114">Application</span></span>|<span data-ttu-id="86f32-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86f32-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="86f32-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="86f32-116">HTTP request</span></span>
```
PATCH /financials/companies('{id}')/vendors('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="86f32-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="86f32-117">Optional query parameters</span></span>
<span data-ttu-id="86f32-118">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="86f32-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="86f32-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="86f32-119">Request headers</span></span>
|<span data-ttu-id="86f32-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="86f32-120">Header</span></span>|<span data-ttu-id="86f32-121">Wert</span><span class="sxs-lookup"><span data-stu-id="86f32-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="86f32-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="86f32-122">Authorization</span></span> |<span data-ttu-id="86f32-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="86f32-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="86f32-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="86f32-125">Content-Type</span></span>  |<span data-ttu-id="86f32-126">application/json</span><span class="sxs-lookup"><span data-stu-id="86f32-126">application/json</span></span>|
|<span data-ttu-id="86f32-127">If-Match</span><span class="sxs-lookup"><span data-stu-id="86f32-127">If-Match</span></span>      |<span data-ttu-id="86f32-128">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="86f32-128">Required.</span></span> <span data-ttu-id="86f32-129">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag nicht mit dem aktuellen Tag der **Anbieter**übereinstimmt, werden die **Anbieter** nicht aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="86f32-129">When this request header is included and the eTag provided does not match the current tag on the **vendors**, the **vendors** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="86f32-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="86f32-130">Request body</span></span>
<span data-ttu-id="86f32-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="86f32-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="86f32-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="86f32-134">Response</span></span>
<span data-ttu-id="86f32-135">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes **vendors** -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="86f32-135">If successful, this method returns a `200 OK` response code and an updated **vendors** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86f32-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="86f32-136">Example</span></span>

<span data-ttu-id="86f32-137">**Anforderung**</span><span class="sxs-lookup"><span data-stu-id="86f32-137">**Request**</span></span>

<span data-ttu-id="86f32-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="86f32-138">Here is an example of the request.</span></span>
```json
PATCH https://graph.microsoft.com/beta/financials/companies('{id}')/vendors('{id}')
Content-type: application/json

{
  "displayName": "Wide World Importers Inc.",
  "blocked": "Payment"
}
```

<span data-ttu-id="86f32-139">**Antwort**</span><span class="sxs-lookup"><span data-stu-id="86f32-139">**Response**</span></span>

<span data-ttu-id="86f32-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="86f32-140">Here is an example of the response.</span></span> 

> <span data-ttu-id="86f32-141">**Hinweis**: das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="86f32-141">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="86f32-142">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="86f32-142">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "number": "40000",
  "displayName": "Wide World Importers Inc.",
  "address": {
    "street": "51 Radcroft Road",
    "city": "Atlanta",
    "state": "GA",
    "countryLetterCode": "US",
    "postalCode": "31772"
  },
  "phoneNumber": "",
  "email": "toby.rhode@cronuscorp.net",
  "website": "",
  "taxRegistrationNumber": "",
  "currencyCode": "USD",
  "irs1099Code": "",
  "taxLiable": true,
  "blocked": "Payment",
  "balance": 0,
  "lastModifiedDateTime": "2017-03-07T00:35:29.667Z"
}
```


