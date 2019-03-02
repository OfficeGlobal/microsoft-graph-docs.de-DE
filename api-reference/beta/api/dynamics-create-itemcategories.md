---
title: ItemCategories erstellen
description: Erstellt ein Element Category-Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 6d3e2918854e169c13971d0c71fc66091874d3ab
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365388"
---
# <a name="create-itemcategories"></a><span data-ttu-id="db7b7-103">ItemCategories erstellen</span><span class="sxs-lookup"><span data-stu-id="db7b7-103">Create itemCategories</span></span>
<span data-ttu-id="db7b7-104">Erstellen Sie ein Element Category-Objekt Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="db7b7-104">Create an item category object Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="db7b7-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="db7b7-105">Permissions</span></span>
<span data-ttu-id="db7b7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db7b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db7b7-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="db7b7-108">Permission type</span></span> |<span data-ttu-id="db7b7-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="db7b7-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="db7b7-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="db7b7-110">Delegated (work or school account)</span></span>|<span data-ttu-id="db7b7-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db7b7-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="db7b7-112">Delegiert (persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="db7b7-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="db7b7-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="db7b7-113">Not supported.</span></span>|
|<span data-ttu-id="db7b7-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="db7b7-114">Application</span></span>|<span data-ttu-id="db7b7-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db7b7-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="db7b7-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="db7b7-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/itemCategories
```

## <a name="optional-query-parameters"></a><span data-ttu-id="db7b7-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="db7b7-117">Optional query parameters</span></span>
<span data-ttu-id="db7b7-118">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="db7b7-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="db7b7-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="db7b7-119">Request headers</span></span>
|<span data-ttu-id="db7b7-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="db7b7-120">Header</span></span>       |<span data-ttu-id="db7b7-121">Wert</span><span class="sxs-lookup"><span data-stu-id="db7b7-121">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="db7b7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="db7b7-122">Authorization</span></span>|<span data-ttu-id="db7b7-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="db7b7-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="db7b7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="db7b7-125">Content-Type</span></span> |<span data-ttu-id="db7b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="db7b7-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="db7b7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="db7b7-127">Request body</span></span>
<span data-ttu-id="db7b7-128">Geben Sie im Anforderungstext eine JSON-Darstellung eines **itemCategories** -Objekts an.</span><span class="sxs-lookup"><span data-stu-id="db7b7-128">In the request body, supply a JSON representation of an **itemCategories** object.</span></span>

## <a name="response"></a><span data-ttu-id="db7b7-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="db7b7-129">Response</span></span>
<span data-ttu-id="db7b7-130">Bei erfolgreicher Ausführung gibt diese Methode ```201 Created``` den Antwortcode und ein **itemCategories** -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="db7b7-130">If successful, this method returns ```201 Created``` response code and an **itemCategories** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db7b7-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="db7b7-131">Example</span></span>

<span data-ttu-id="db7b7-132">**Anforderung**</span><span class="sxs-lookup"><span data-stu-id="db7b7-132">**Request**</span></span>

<span data-ttu-id="db7b7-133">Hier ist ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="db7b7-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/itemCategories
Content-type: application/json

{
  "code": "CHAIR",
  "displayName": "Office Chair"
}
```

<span data-ttu-id="db7b7-134">**Antwort**</span><span class="sxs-lookup"><span data-stu-id="db7b7-134">**Response**</span></span>

<span data-ttu-id="db7b7-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="db7b7-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="db7b7-136">**Hinweis**: das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="db7b7-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="db7b7-137">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="db7b7-137">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "CHAIR",
  "displayName": "Office Chair",
  "lastModifiedDateTime": "2017-03-15T02:21:24.047Z"
}

```




