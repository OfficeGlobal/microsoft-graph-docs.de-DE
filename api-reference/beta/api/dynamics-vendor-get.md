---
title: Kreditoren abrufen
description: Ruft ein Vendor-Objekt in Dynamics 365 Business Central ab.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: ffd7476ca8412af4858df17d9c415431eaa301dc
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365416"
---
# <a name="get-vendors"></a><span data-ttu-id="233c3-103">Kreditoren abrufen</span><span class="sxs-lookup"><span data-stu-id="233c3-103">Get vendors</span></span>
<span data-ttu-id="233c3-104">Rufen Sie die Eigenschaften und Beziehungen eines Vendor-Objekts für Dynamics 365 Business Central ab.</span><span class="sxs-lookup"><span data-stu-id="233c3-104">Retrieve the properties and relationships of a vendor object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="233c3-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="233c3-105">Permissions</span></span>
<span data-ttu-id="233c3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="233c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="233c3-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="233c3-108">Permission type</span></span> |<span data-ttu-id="233c3-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="233c3-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="233c3-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="233c3-110">Delegated (work or school account)</span></span>|<span data-ttu-id="233c3-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="233c3-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="233c3-112">Delegiert (persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="233c3-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="233c3-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="233c3-113">Not supported.</span></span>|
|<span data-ttu-id="233c3-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="233c3-114">Application</span></span>|<span data-ttu-id="233c3-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="233c3-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="233c3-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="233c3-116">HTTP request</span></span>

```
GET /financials/companies('{id}')/vendors('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="233c3-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="233c3-117">Optional query parameters</span></span>
<span data-ttu-id="233c3-118">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="233c3-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="233c3-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="233c3-119">Request headers</span></span>
|<span data-ttu-id="233c3-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="233c3-120">Header</span></span>|<span data-ttu-id="233c3-121">Wert</span><span class="sxs-lookup"><span data-stu-id="233c3-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="233c3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="233c3-122">Authorization</span></span>  |<span data-ttu-id="233c3-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="233c3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="233c3-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="233c3-125">Request body</span></span>
<span data-ttu-id="233c3-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="233c3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="233c3-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="233c3-127">Response</span></span>
<span data-ttu-id="233c3-128">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein **vendors** -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="233c3-128">If successful, this method returns a `200 OK` response code and a **vendors** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="233c3-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="233c3-129">Example</span></span>

<span data-ttu-id="233c3-130">**Anforderung**</span><span class="sxs-lookup"><span data-stu-id="233c3-130">**Request**</span></span>

<span data-ttu-id="233c3-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="233c3-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/vendors('{id}')
```

<span data-ttu-id="233c3-132">**Antwort**</span><span class="sxs-lookup"><span data-stu-id="233c3-132">**Response**</span></span>

<span data-ttu-id="233c3-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="233c3-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="233c3-134">**Hinweis**: das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="233c3-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="233c3-135">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="233c3-135">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "number": "40000",
  "displayName": "Wide World Importers",
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
  "currencyId": "id-value",
  "currencyCode": "USD",
  "irs1099Code": "",
  "paymentTermsId": "id-value",
  "paymentMethodId": "id-value",
  "taxLiable": true,
  "blocked": " ",
  "balance": 0,
  "lastModifiedDateTime": "2017-03-07T00:35:29.667Z"
}
```


