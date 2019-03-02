---
title: TaxAreas aktualisieren
description: Aktualisiert ein Steuerbereich-Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 42a53f03e71ca5fe41293db0dc5459990f4560e6
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366753"
---
# <a name="update-taxareas"></a><span data-ttu-id="437d6-103">TaxAreas aktualisieren</span><span class="sxs-lookup"><span data-stu-id="437d6-103">Update taxAreas</span></span>
<span data-ttu-id="437d6-104">Aktualisieren der Eigenschaften eines Steuerbereichs Objekts für Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="437d6-104">Update the properties of a tax area object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="437d6-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="437d6-105">Permissions</span></span>
<span data-ttu-id="437d6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="437d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="437d6-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="437d6-108">Permission type</span></span> |<span data-ttu-id="437d6-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="437d6-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="437d6-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="437d6-110">Delegated (work or school account)</span></span>|<span data-ttu-id="437d6-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="437d6-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="437d6-112">Delegiert (persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="437d6-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="437d6-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="437d6-113">Not supported.</span></span>|
|<span data-ttu-id="437d6-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="437d6-114">Application</span></span>|<span data-ttu-id="437d6-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="437d6-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="437d6-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="437d6-116">HTTP request</span></span>

```
PATCH /financials/companies('{id}')/taxAreas('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="437d6-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="437d6-117">Optional query parameters</span></span>
<span data-ttu-id="437d6-118">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="437d6-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="437d6-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="437d6-119">Request headers</span></span>
|<span data-ttu-id="437d6-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="437d6-120">Header</span></span>|<span data-ttu-id="437d6-121">Wert</span><span class="sxs-lookup"><span data-stu-id="437d6-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="437d6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="437d6-122">Authorization</span></span> |<span data-ttu-id="437d6-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="437d6-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="437d6-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="437d6-125">Content-Type</span></span>  |<span data-ttu-id="437d6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="437d6-126">application/json</span></span>|
|<span data-ttu-id="437d6-127">If-Match</span><span class="sxs-lookup"><span data-stu-id="437d6-127">If-Match</span></span>      |<span data-ttu-id="437d6-128">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="437d6-128">Required.</span></span> <span data-ttu-id="437d6-129">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag nicht mit dem aktuellen Tag in der **taxAreas**übereinstimmt, wird die **taxAreas** nicht aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="437d6-129">When this request header is included and the eTag provided does not match the current tag on the **taxAreas**, the **taxAreas** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="437d6-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="437d6-130">Request body</span></span>
<span data-ttu-id="437d6-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="437d6-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="437d6-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="437d6-134">Response</span></span>
<span data-ttu-id="437d6-135">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes **taxAreas** -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="437d6-135">If successful, this method returns a `200 OK` response code and an updated **taxAreas** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="437d6-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="437d6-136">Example</span></span>

<span data-ttu-id="437d6-137">**Anforderung**</span><span class="sxs-lookup"><span data-stu-id="437d6-137">**Request**</span></span>

<span data-ttu-id="437d6-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="437d6-138">Here is an example of the request.</span></span>
```json
PATCH https://graph.microsoft.com/beta/financials/companies('{id}')/taxAreas('{id}')
Content-type: application/json

{
  "code": "28012001T",
  "displayName": "tax area",
}
```

<span data-ttu-id="437d6-139">**Antwort**</span><span class="sxs-lookup"><span data-stu-id="437d6-139">**Response**</span></span>

<span data-ttu-id="437d6-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="437d6-140">Here is an example of the response.</span></span> 

> <span data-ttu-id="437d6-141">**Hinweis**: das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="437d6-141">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="437d6-142">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="437d6-142">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "code": "28012001T",
  "displayName": "tax area",
  "taxType": "Sales Tax",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```

