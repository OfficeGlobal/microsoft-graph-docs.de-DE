---
title: Mitarbeiter abrufen
description: Ruft ein Employee-Objekt in Dynamics 365 Business Central ab.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 9adab4c18d2c380f949d3fd7894aae4a8de7c0da
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365584"
---
# <a name="get-employees"></a><span data-ttu-id="6f409-103">Mitarbeiter abrufen</span><span class="sxs-lookup"><span data-stu-id="6f409-103">Get employees</span></span>
<span data-ttu-id="6f409-104">Rufen Sie die Eigenschaften und Beziehungen eines Employee-Objekts für Dynamics 365 Business Central ab.</span><span class="sxs-lookup"><span data-stu-id="6f409-104">Retrieve the properties and relationships of an employee object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f409-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6f409-105">Permissions</span></span>
<span data-ttu-id="6f409-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f409-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f409-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6f409-108">Permission type</span></span> |<span data-ttu-id="6f409-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6f409-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="6f409-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6f409-110">Delegated (work or school account)</span></span>|<span data-ttu-id="6f409-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f409-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="6f409-112">Delegiert (persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="6f409-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="6f409-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6f409-113">Not supported.</span></span>|
|<span data-ttu-id="6f409-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6f409-114">Application</span></span>|<span data-ttu-id="6f409-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f409-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f409-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f409-116">HTTP request</span></span>
```
GET /financials/companies('{id}')/employees('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6f409-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6f409-117">Optional query parameters</span></span>
<span data-ttu-id="6f409-118">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6f409-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6f409-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6f409-119">Request headers</span></span>
|<span data-ttu-id="6f409-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6f409-120">Header</span></span>       |<span data-ttu-id="6f409-121">Wert</span><span class="sxs-lookup"><span data-stu-id="6f409-121">Value</span></span>                     |
|-------------|--------------------------|
|<span data-ttu-id="6f409-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f409-122">Authorization</span></span>|<span data-ttu-id="6f409-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6f409-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f409-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6f409-125">Request body</span></span>
<span data-ttu-id="6f409-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6f409-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f409-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f409-127">Response</span></span>
<span data-ttu-id="6f409-128">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein **Employees** -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6f409-128">If successful, this method returns a `200 OK` response code and an **employees** object in the response body.</span></span>

<span data-ttu-id="6f409-129">**Anforderung**</span><span class="sxs-lookup"><span data-stu-id="6f409-129">**Request**</span></span>

<span data-ttu-id="6f409-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6f409-130">Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/employees('{id}')
```

<span data-ttu-id="6f409-131">**Antwort**</span><span class="sxs-lookup"><span data-stu-id="6f409-131">**Response**</span></span>

<span data-ttu-id="6f409-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6f409-132">Here is an example of the response.</span></span> 

> <span data-ttu-id="6f409-133">**Hinweis**: das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="6f409-133">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6f409-134">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="6f409-134">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "number": "AH",
  "displayName": "Annette Hill",
  "givenName": "Annette",
  "middleName": "",
  "surname": "Hill",
  "jobTitle": "Secretary",
  "address": {
    "street": "677 Fifth Avenue",
    "city": "New York",
    "state": "",
    "countryLetterCode": "",
    "postalCode": "10022"
  },
  "phoneNumber": "4465-4899-4643",
  "mobilePhone": "4564-4564-7831",
  "email": "",
  "personalEmail": "ah@cronus-demosite.com",
  "employmentDate": "2001-06-01",
  "terminationDate": "0001-01-01",
  "status": "Active",
  "birthDate": "1973-12-12",
  "picture@odata.mediaReadLink": "https://api.financials.dynamics.com/v1.0/api/beta/companies('{id}')/employees('{id}')/picture",
  "lastModifiedDateTime": "2017-03-16T14:57:19.497Z"  
}
```


