---
title: Kreditoren erstellen
description: Erstellt ein Vendor-Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 90c2c8a25602ac2a2c4197c916b9ce14e03b8e6d
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365353"
---
# <a name="create-vendors"></a><span data-ttu-id="9926f-103">Kreditoren erstellen</span><span class="sxs-lookup"><span data-stu-id="9926f-103">Create vendors</span></span>
<span data-ttu-id="9926f-104">Erstellen Sie ein Vendor-Objekt in Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="9926f-104">Create a vendor object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="9926f-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9926f-105">Permissions</span></span>
<span data-ttu-id="9926f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9926f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9926f-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9926f-108">Permission type</span></span> |<span data-ttu-id="9926f-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9926f-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="9926f-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9926f-110">Delegated (work or school account)</span></span>|<span data-ttu-id="9926f-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9926f-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="9926f-112">Delegiert (persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="9926f-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="9926f-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9926f-113">Not supported.</span></span>|
|<span data-ttu-id="9926f-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9926f-114">Application</span></span>|<span data-ttu-id="9926f-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9926f-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9926f-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9926f-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/vendors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9926f-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9926f-117">Optional query parameters</span></span>
<span data-ttu-id="9926f-118">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9926f-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9926f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9926f-119">Request headers</span></span>
|<span data-ttu-id="9926f-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9926f-120">Header</span></span>|<span data-ttu-id="9926f-121">Wert</span><span class="sxs-lookup"><span data-stu-id="9926f-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="9926f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9926f-122">Authorization</span></span>  |<span data-ttu-id="9926f-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9926f-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="9926f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9926f-125">Content-Type</span></span>  |<span data-ttu-id="9926f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9926f-126">application/json</span></span>   |

## <a name="request-body"></a><span data-ttu-id="9926f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9926f-127">Request body</span></span>
<span data-ttu-id="9926f-128">Geben Sie im Anforderungstext eine JSON-Darstellung eines **vendors** -Objekts an.</span><span class="sxs-lookup"><span data-stu-id="9926f-128">In the request body, supply a JSON representation of a **vendors** object.</span></span>

## <a name="response"></a><span data-ttu-id="9926f-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="9926f-129">Response</span></span>
<span data-ttu-id="9926f-130">Bei erfolgreicher Ausführung gibt diese Methode ```201 Created``` den Antwortcode und \*\*\*\* ein vendors-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9926f-130">If successful, this method returns ```201 Created``` response code and a **vendors** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9926f-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9926f-131">Example</span></span>

<span data-ttu-id="9926f-132">**Anforderung**</span><span class="sxs-lookup"><span data-stu-id="9926f-132">**Request**</span></span>

<span data-ttu-id="9926f-133">Hier ist ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9926f-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/vendors
Content-type: application/json

{
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
  "currencyCode": "USD",
  "irs1099Code": "",
  "taxLiable": true,
  "blocked": " "
}
```

<span data-ttu-id="9926f-134">**Antwort**</span><span class="sxs-lookup"><span data-stu-id="9926f-134">**Response**</span></span>

<span data-ttu-id="9926f-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9926f-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="9926f-136">**Hinweis**: das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="9926f-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9926f-137">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="9926f-137">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "number": "40000",
  "displayName": "Wide World Importers",
  "lastModifiedDateTime": "2015-11-09T02:14:32Z"
}

```

