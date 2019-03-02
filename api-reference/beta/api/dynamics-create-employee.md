---
title: Mitarbeiter erstellen
description: Erstellt ein Employee-Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 5432a312c4a1702b47413ee7080da0653a159fef
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365605"
---
# <a name="create-employees"></a><span data-ttu-id="d6536-103">Mitarbeiter erstellen</span><span class="sxs-lookup"><span data-stu-id="d6536-103">Create employees</span></span>
<span data-ttu-id="d6536-104">Erstellen Sie ein Employee-Objekt in Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="d6536-104">Create an employee object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6536-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d6536-105">Permissions</span></span>
<span data-ttu-id="d6536-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6536-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6536-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d6536-108">Permission type</span></span> |<span data-ttu-id="d6536-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d6536-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="d6536-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d6536-110">Delegated (work or school account)</span></span>|<span data-ttu-id="d6536-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6536-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="d6536-112">Delegiert (persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="d6536-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="d6536-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d6536-113">Not supported.</span></span>|
|<span data-ttu-id="d6536-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d6536-114">Application</span></span>|<span data-ttu-id="d6536-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6536-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6536-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d6536-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/employees
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d6536-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d6536-117">Optional query parameters</span></span>
<span data-ttu-id="d6536-118">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d6536-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6536-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d6536-119">Request headers</span></span>
|<span data-ttu-id="d6536-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d6536-120">Header</span></span>        |<span data-ttu-id="d6536-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d6536-121">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="d6536-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6536-122">Authorization</span></span> |<span data-ttu-id="d6536-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d6536-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d6536-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d6536-125">Content-Type</span></span>  |<span data-ttu-id="d6536-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6536-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="d6536-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d6536-127">Request body</span></span>
<span data-ttu-id="d6536-128">Geben Sie im Anforderungstext eine JSON-Darstellung eines **Employees** -Objekts an.</span><span class="sxs-lookup"><span data-stu-id="d6536-128">In the request body, supply a JSON representation of an **employees** object.</span></span>

## <a name="response"></a><span data-ttu-id="d6536-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="d6536-129">Response</span></span>
<span data-ttu-id="d6536-130">Bei erfolgreicher Ausführung gibt diese Methode ```201 Created``` den Antwortcode und \*\*\*\* ein Employees-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d6536-130">If successful, this method returns ```201 Created``` response code and an **employees** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6536-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d6536-131">Example</span></span>

<span data-ttu-id="d6536-132">**Anforderung**</span><span class="sxs-lookup"><span data-stu-id="d6536-132">**Request**</span></span>

<span data-ttu-id="d6536-133">Hier ist ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d6536-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/employees
Content-type: application/json

{
  "id": "id-value",
  "number": "AH",
  "givenName": "Annette",
  "surname": "Hill",
  "jobTitle": "Production Assistant",
  "address": {
    "street": "677 Fifth Avenue",
    "city": "New York",
    "state": "",
    "countryLetterCode": "",
    "postalCode": "10022"
  },
  "phoneNumber": "4465-4899-4643",
  "mobilePhone": "4564-4564-7831",
  "personalEmail": "ah@cronus-demosite.com",
  "employmentDate": "2001-06-01",
  "birthDate": "1973-12-12"  
}

```

<span data-ttu-id="d6536-134">**Antwort**</span><span class="sxs-lookup"><span data-stu-id="d6536-134">**Response**</span></span>

<span data-ttu-id="d6536-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d6536-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="d6536-136">**Hinweis**: das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="d6536-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d6536-137">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="d6536-137">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

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

