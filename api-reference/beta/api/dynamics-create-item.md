---
title: Elemente erstellen
description: Erstellt ein Item-Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 68bb1e1c8fbfa3c7675b5ef6dc39de24ffad2ecd
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365836"
---
# <a name="create-items"></a><span data-ttu-id="6dd27-103">Elemente erstellen</span><span class="sxs-lookup"><span data-stu-id="6dd27-103">Create items</span></span>
<span data-ttu-id="6dd27-104">Erstellen eines Elements in Dynamics 365 Business Central für die Verwendung auf Rechnungen, Anführungszeichen usw.</span><span class="sxs-lookup"><span data-stu-id="6dd27-104">Create an item in Dynamics 365 Business Central for use on invoices, quotes, etc.</span></span>

## <a name="permissions"></a><span data-ttu-id="6dd27-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6dd27-105">Permissions</span></span>
<span data-ttu-id="6dd27-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dd27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dd27-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6dd27-108">Permission type</span></span> |<span data-ttu-id="6dd27-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6dd27-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="6dd27-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6dd27-110">Delegated (work or school account)</span></span>|<span data-ttu-id="6dd27-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dd27-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="6dd27-112">Delegiert (persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="6dd27-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="6dd27-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6dd27-113">Not supported.</span></span>|
|<span data-ttu-id="6dd27-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6dd27-114">Application</span></span>|<span data-ttu-id="6dd27-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dd27-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6dd27-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6dd27-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/items
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6dd27-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6dd27-117">Optional query parameters</span></span>
<span data-ttu-id="6dd27-118">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6dd27-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6dd27-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6dd27-119">Request headers</span></span>
|<span data-ttu-id="6dd27-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6dd27-120">Header</span></span>       |<span data-ttu-id="6dd27-121">Wert</span><span class="sxs-lookup"><span data-stu-id="6dd27-121">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="6dd27-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6dd27-122">Authorization</span></span>|<span data-ttu-id="6dd27-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6dd27-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6dd27-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6dd27-125">Content-Type</span></span> |<span data-ttu-id="6dd27-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6dd27-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="6dd27-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6dd27-127">Request body</span></span>
<span data-ttu-id="6dd27-128">Geben Sie im Anforderungstext eine JSON-Darstellung eines **Items** -Objekts an.</span><span class="sxs-lookup"><span data-stu-id="6dd27-128">In the request body, supply a JSON representation of an **items** object.</span></span>

## <a name="response"></a><span data-ttu-id="6dd27-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="6dd27-129">Response</span></span>
<span data-ttu-id="6dd27-130">Bei erfolgreicher Ausführung gibt diese Methode ```201 Created``` den Antwortcode und ein **Items** -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6dd27-130">If successful, this method returns ```201 Created``` response code and an **items** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6dd27-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6dd27-131">Example</span></span>
<span data-ttu-id="6dd27-132">**Anforderung**</span><span class="sxs-lookup"><span data-stu-id="6dd27-132">**Request**</span></span>

<span data-ttu-id="6dd27-133">Hier ist ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6dd27-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/items
Content-type: application/json

{
  "number": "1896-S",
  "displayName": "ATHENS Desk",
  "type": "Inventory",
  "blocked": false,
  "baseUnitOfMeasureId": "65bdbd3a-39f1-49f4-bf24-598cbac36230",
  "gtin": "",
  "itemCategoryId": "5b0b9c1c-312d-4809-96b2-056690a11057",
  "inventory": 0,
  "unitPrice": 1000.8,
  "priceIncludesTax": false,
  "unitCost": 780.7,
  "taxGroupCode": "FURNITURE"
} 

```

<span data-ttu-id="6dd27-134">**Antwort**</span><span class="sxs-lookup"><span data-stu-id="6dd27-134">**Response**</span></span>

<span data-ttu-id="6dd27-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6dd27-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="6dd27-136">**Hinweis**: das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="6dd27-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6dd27-137">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="6dd27-137">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "number": "1896-S",
  "displayName": "ATHENS Desk",
  "lastModifiedDateTime": "2015-11-09T02:14:32Z"
}
```

