---
title: Währungen aktualisieren
description: Aktualisiert ein Currency-Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: e243325d4a7e7536c1e079385f695ef2cc7359c7
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365647"
---
# <a name="update-currencies"></a><span data-ttu-id="4df0b-103">Währungen aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4df0b-103">Update currencies</span></span>
<span data-ttu-id="4df0b-104">Aktualisieren der Eigenschaften eines Currency-Objekts für Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="4df0b-104">Update the properties of a currency object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="4df0b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4df0b-105">Permissions</span></span>
<span data-ttu-id="4df0b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4df0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4df0b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4df0b-108">Permission type</span></span> |<span data-ttu-id="4df0b-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4df0b-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="4df0b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4df0b-110">Delegated (work or school account)</span></span>|<span data-ttu-id="4df0b-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4df0b-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="4df0b-112">Delegiert (persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="4df0b-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="4df0b-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4df0b-113">Not supported.</span></span>|
|<span data-ttu-id="4df0b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4df0b-114">Application</span></span>|<span data-ttu-id="4df0b-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4df0b-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4df0b-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4df0b-116">HTTP request</span></span>
```
PATCH /financials/companies('{id}')/currencies('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4df0b-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4df0b-117">Optional query parameters</span></span>
<span data-ttu-id="4df0b-118">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4df0b-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4df0b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4df0b-119">Request headers</span></span>
|<span data-ttu-id="4df0b-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4df0b-120">Header</span></span>       |<span data-ttu-id="4df0b-121">Wert</span><span class="sxs-lookup"><span data-stu-id="4df0b-121">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="4df0b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4df0b-122">Authorization</span></span>|<span data-ttu-id="4df0b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4df0b-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4df0b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4df0b-125">Content-Type</span></span> |<span data-ttu-id="4df0b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4df0b-126">application/json</span></span>         |
|<span data-ttu-id="4df0b-127">If-Match</span><span class="sxs-lookup"><span data-stu-id="4df0b-127">If-Match</span></span>     |<span data-ttu-id="4df0b-128">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4df0b-128">Required.</span></span> <span data-ttu-id="4df0b-129">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag nicht mit dem aktuellen Tag in den **Währungen**übereinstimmt, werden die **Währungen** nicht aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="4df0b-129">When this request header is included and the eTag provided does not match the current tag on the **currencies**, the **currencies** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4df0b-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4df0b-130">Request body</span></span>
<span data-ttu-id="4df0b-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="4df0b-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="4df0b-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="4df0b-134">Response</span></span>
<span data-ttu-id="4df0b-135">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes **Währungen** -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4df0b-135">If successful, this method returns a `200 OK` response code and an updated **currencies** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4df0b-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4df0b-136">Example</span></span>

<span data-ttu-id="4df0b-137">**Anforderung**</span><span class="sxs-lookup"><span data-stu-id="4df0b-137">**Request**</span></span>

<span data-ttu-id="4df0b-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4df0b-138">Here is an example of the request.</span></span>
```json
PATCH https://graph.microsoft.com/beta/financials/companies('{id}')/currencies('{id}')
Content-type: application/json

{
    "displayName": "United States Dollar"
}
```

<span data-ttu-id="4df0b-139">**Antwort**</span><span class="sxs-lookup"><span data-stu-id="4df0b-139">**Response**</span></span>

<span data-ttu-id="4df0b-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4df0b-140">Here is an example of the response.</span></span> 

> <span data-ttu-id="4df0b-141">**Hinweis**: das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="4df0b-141">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4df0b-142">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="4df0b-142">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "code": "US",
  "displayName": "United States Dollar",
  "symbol": "$",
  "amountDecimalPlaces": "2:2",
  "amountRoundingPrecision": 0.01,
  "lastModifiedDateTime": "2017-03-22T21:12:18.793Z"
}
```
