---
title: ItemCategories abrufen
description: Ruft eine elementkategorie in Dynamics 365 Business Central ab.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 7e339b89f53b0f7c3cd8f5dfc7976ba931bcaffd
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365808"
---
# <a name="get-itemcategories"></a><span data-ttu-id="33f6c-103">ItemCategories abrufen</span><span class="sxs-lookup"><span data-stu-id="33f6c-103">Get itemCategories</span></span>
<span data-ttu-id="33f6c-104">Rufen Sie die Eigenschaften und Beziehungen eines Item Category-Objekts für Dynamics 365 Business Central ab.</span><span class="sxs-lookup"><span data-stu-id="33f6c-104">Retrieve the properties and relationships of an item category object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="33f6c-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="33f6c-105">Permissions</span></span>
<span data-ttu-id="33f6c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33f6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33f6c-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="33f6c-108">Permission type</span></span> |<span data-ttu-id="33f6c-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="33f6c-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="33f6c-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="33f6c-110">Delegated (work or school account)</span></span>|<span data-ttu-id="33f6c-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33f6c-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="33f6c-112">Delegiert (persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="33f6c-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="33f6c-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="33f6c-113">Not supported.</span></span>|
|<span data-ttu-id="33f6c-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="33f6c-114">Application</span></span>|<span data-ttu-id="33f6c-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33f6c-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="33f6c-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="33f6c-116">HTTP request</span></span>

```
GET /financials/companies('{id}')/itemCategories('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="33f6c-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="33f6c-117">Optional query parameters</span></span>
<span data-ttu-id="33f6c-118">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="33f6c-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="33f6c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="33f6c-119">Request headers</span></span>
|<span data-ttu-id="33f6c-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="33f6c-120">Header</span></span>       |<span data-ttu-id="33f6c-121">Wert</span><span class="sxs-lookup"><span data-stu-id="33f6c-121">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="33f6c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="33f6c-122">Authorization</span></span>|<span data-ttu-id="33f6c-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="33f6c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="33f6c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="33f6c-125">Request body</span></span>
<span data-ttu-id="33f6c-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="33f6c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33f6c-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="33f6c-127">Response</span></span>
<span data-ttu-id="33f6c-128">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein **itemCategories** -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="33f6c-128">If successful, this method returns a `200 OK` response code and an **itemCategories** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33f6c-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="33f6c-129">Example</span></span>

<span data-ttu-id="33f6c-130">**Anforderung**</span><span class="sxs-lookup"><span data-stu-id="33f6c-130">**Request**</span></span>

<span data-ttu-id="33f6c-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="33f6c-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/itemCategories('{id}')
```

<span data-ttu-id="33f6c-132">**Antwort**</span><span class="sxs-lookup"><span data-stu-id="33f6c-132">**Response**</span></span>

<span data-ttu-id="33f6c-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="33f6c-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="33f6c-134">**Hinweis**: das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="33f6c-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="33f6c-135">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="33f6c-135">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "CHAIR",
  "displayName": "Office Chair",
  "lastModifiedDateTime": "2017-03-15T02:21:24.047Z"
}
```

