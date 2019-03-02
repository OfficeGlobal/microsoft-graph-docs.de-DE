---
title: CompanyInformation abrufen
description: Ruft ein Unternehmens Informationsobjekt in Dynamics 365 Business Central ab.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: ad49c3d4095283fc42c2e8f2046c646f3558ac18
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365801"
---
# <a name="get-companyinformation"></a><span data-ttu-id="60b86-103">CompanyInformation abrufen</span><span class="sxs-lookup"><span data-stu-id="60b86-103">Get companyInformation</span></span>
<span data-ttu-id="60b86-104">Rufen Sie die Eigenschaften und Beziehungen eines Unternehmens Informationsobjekts für Dynamics 365 Business Central ab.</span><span class="sxs-lookup"><span data-stu-id="60b86-104">Retrieve the properties and relationships of a company information object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="60b86-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="60b86-105">Permissions</span></span>
<span data-ttu-id="60b86-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60b86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60b86-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="60b86-108">Permission type</span></span> |<span data-ttu-id="60b86-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="60b86-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="60b86-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="60b86-110">Delegated (work or school account)</span></span>|<span data-ttu-id="60b86-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60b86-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="60b86-112">Delegiert (persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="60b86-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="60b86-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="60b86-113">Not supported.</span></span>|
|<span data-ttu-id="60b86-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="60b86-114">Application</span></span>|<span data-ttu-id="60b86-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60b86-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="60b86-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="60b86-116">HTTP request</span></span>
```
GET /financials/companies('{id}')/companyInformation('{id}')
```
## <a name="optional-query-parameters"></a><span data-ttu-id="60b86-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="60b86-117">Optional query parameters</span></span>
<span data-ttu-id="60b86-118">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="60b86-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="60b86-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="60b86-119">Request headers</span></span>
|<span data-ttu-id="60b86-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="60b86-120">Header</span></span>|<span data-ttu-id="60b86-121">Wert</span><span class="sxs-lookup"><span data-stu-id="60b86-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="60b86-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="60b86-122">Authorization</span></span>  |<span data-ttu-id="60b86-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="60b86-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60b86-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="60b86-125">Request body</span></span>
<span data-ttu-id="60b86-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="60b86-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60b86-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="60b86-127">Response</span></span>
<span data-ttu-id="60b86-128">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein **companyInformation** -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="60b86-128">If successful, this method returns a `200 OK` response code and a **companyInformation** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60b86-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="60b86-129">Example</span></span>

<span data-ttu-id="60b86-130">**Anforderung**</span><span class="sxs-lookup"><span data-stu-id="60b86-130">**Request**</span></span>

<span data-ttu-id="60b86-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="60b86-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/companyInformation('{id}')
```

<span data-ttu-id="60b86-132">**Antwort**</span><span class="sxs-lookup"><span data-stu-id="60b86-132">**Response**</span></span>

<span data-ttu-id="60b86-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="60b86-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="60b86-134">**Hinweis**: das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="60b86-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="60b86-135">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="60b86-135">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "displayName": "CRONUS USA, Inc.",
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
  "website": "",
  "taxRegistrationNumber": "",
  "currencyCode": "USD",
  "currentFiscalYearStartDate": "2018-01-01",
  "industry": "",
  "picture@odata.mediaReadLink": "https://api.financials.dynamics.com/v1.0/api/beta/companies('{id}')/companyInformation('{id}')/picture",
  "businessProfileId": "",
  "lastModifiedDateTime": "2017-03-16T14:57:19.497Z"
}
```
