---
title: CustomerPayments löschen
description: Löscht ein Kunden-Zahlungs Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: ab4f40785401353887cba22eaeca620c75276051
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365703"
---
# <a name="delete-customerpayments"></a><span data-ttu-id="9c042-103">CustomerPayments löschen</span><span class="sxs-lookup"><span data-stu-id="9c042-103">Delete customerPayments</span></span>
<span data-ttu-id="9c042-104">Löschen eines customerPayment aus Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="9c042-104">Delete a customerPayment from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c042-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9c042-105">Permissions</span></span>
<span data-ttu-id="9c042-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c042-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c042-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9c042-108">Permission type</span></span> |<span data-ttu-id="9c042-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9c042-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="9c042-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9c042-110">Delegated (work or school account)</span></span>|<span data-ttu-id="9c042-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c042-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="9c042-112">Delegiert (persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="9c042-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="9c042-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9c042-113">Not supported.</span></span>|
|<span data-ttu-id="9c042-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9c042-114">Application</span></span>|<span data-ttu-id="9c042-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c042-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c042-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9c042-116">HTTP request</span></span>
```
DELETE /financials/companies('{id}')/customerPaymentJournals('{id}')/customerPayments('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9c042-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9c042-117">Optional query parameters</span></span>
<span data-ttu-id="9c042-118">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9c042-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9c042-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9c042-119">Request headers</span></span>
|<span data-ttu-id="9c042-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9c042-120">Header</span></span>         |<span data-ttu-id="9c042-121">Wert</span><span class="sxs-lookup"><span data-stu-id="9c042-121">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="9c042-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c042-122">Authorization</span></span>  |<span data-ttu-id="9c042-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9c042-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="9c042-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="9c042-125">If-Match</span></span>       |<span data-ttu-id="9c042-126">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9c042-126">Required.</span></span> <span data-ttu-id="9c042-127">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag nicht mit dem aktuellen Tag in der **customerPayments**übereinstimmt, wird die **customerPayments** nicht aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="9c042-127">When this request header is included and the eTag provided does not match the current tag on the **customerPayments**, the **customerPayments** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c042-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9c042-128">Request body</span></span>

<span data-ttu-id="9c042-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9c042-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c042-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="9c042-130">Response</span></span>

<span data-ttu-id="9c042-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode ```204 No Content``` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9c042-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c042-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9c042-133">Example</span></span>

<span data-ttu-id="9c042-134">**Anforderung**</span><span class="sxs-lookup"><span data-stu-id="9c042-134">**Request**</span></span>

<span data-ttu-id="9c042-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9c042-135">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies('{id}')/customerPaymentJournals('{id}')/customerPayments('{id}')
```

<span data-ttu-id="9c042-136">**Antwort**</span><span class="sxs-lookup"><span data-stu-id="9c042-136">**Response**</span></span> 

<span data-ttu-id="9c042-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9c042-137">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```
