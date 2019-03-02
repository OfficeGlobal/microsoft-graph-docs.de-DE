---
title: PaymentTerms abrufen
description: Ruft ein Zahlungs Term-Objekt in Dynamics 365 Business Central ab.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 14f7b2b36b687190817dc348e975ba1a23c99aae
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365507"
---
# <a name="get-paymentterms"></a><span data-ttu-id="e0a33-103">PaymentTerms abrufen</span><span class="sxs-lookup"><span data-stu-id="e0a33-103">Get paymentTerms</span></span>
<span data-ttu-id="e0a33-104">Rufen Sie die Eigenschaften und Beziehungen eines Zahlungs Terms-Objekts für Dynamics 365 Business Central ab.</span><span class="sxs-lookup"><span data-stu-id="e0a33-104">Retrieve the properties and relationships of a payment terms object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0a33-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e0a33-105">Permissions</span></span>
<span data-ttu-id="e0a33-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0a33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0a33-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e0a33-108">Permission type</span></span> |<span data-ttu-id="e0a33-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e0a33-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="e0a33-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e0a33-110">Delegated (work or school account)</span></span>|<span data-ttu-id="e0a33-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0a33-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="e0a33-112">Delegiert (persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="e0a33-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="e0a33-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e0a33-113">Not supported.</span></span>|
|<span data-ttu-id="e0a33-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e0a33-114">Application</span></span>|<span data-ttu-id="e0a33-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0a33-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0a33-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e0a33-116">HTTP request</span></span>

```
GET /financials/companies('{id}')/paymentTerms('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e0a33-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e0a33-117">Optional query parameters</span></span>
<span data-ttu-id="e0a33-118">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e0a33-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0a33-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e0a33-119">Request headers</span></span>
|<span data-ttu-id="e0a33-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e0a33-120">Header</span></span>         |<span data-ttu-id="e0a33-121">Wert</span><span class="sxs-lookup"><span data-stu-id="e0a33-121">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="e0a33-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0a33-122">Authorization</span></span>  |<span data-ttu-id="e0a33-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e0a33-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0a33-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e0a33-125">Request body</span></span>
<span data-ttu-id="e0a33-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e0a33-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0a33-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="e0a33-127">Response</span></span>
<span data-ttu-id="e0a33-128">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein **paymentTerms** -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e0a33-128">If successful, this method returns a `200 OK` response code and a **paymentTerms** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0a33-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e0a33-129">Example</span></span>

<span data-ttu-id="e0a33-130">**Anforderung**</span><span class="sxs-lookup"><span data-stu-id="e0a33-130">**Request**</span></span>

<span data-ttu-id="e0a33-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e0a33-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/paymentTerms('{id}')
```

<span data-ttu-id="e0a33-132">**Antwort**</span><span class="sxs-lookup"><span data-stu-id="e0a33-132">**Response**</span></span>

<span data-ttu-id="e0a33-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e0a33-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="e0a33-134">**Hinweis**: das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="e0a33-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e0a33-135">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="e0a33-135">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "7 DAYS",
  "displayName": "Net 7 days",
  "dueDateCalculation": "7D",
  "discountDateCalculation": "",
  "discountPercent": 0,
  "calculateDiscountOnCreditMemos": false,
  "lastModifiedDateTime": "2017-03-15T02:20:55.203Z"
}
```
