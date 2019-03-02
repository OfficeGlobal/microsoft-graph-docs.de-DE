---
title: CustomerPaymentJournals erstellen
description: Erstellt ein Kunden Zahlungsjournal-Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: a633ef91fe15b4999285d7290ca6eed8c10846a3
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365465"
---
# <a name="create-customerpaymentjournals"></a><span data-ttu-id="2eeaa-103">CustomerPaymentJournals erstellen</span><span class="sxs-lookup"><span data-stu-id="2eeaa-103">Create customerPaymentJournals</span></span>
<span data-ttu-id="2eeaa-104">Erstellt ein Kunden-Zahlungsjournal Objekt in Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="2eeaa-104">Creates a customer payment journal object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="2eeaa-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2eeaa-105">Permissions</span></span>
<span data-ttu-id="2eeaa-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2eeaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2eeaa-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2eeaa-108">Permission type</span></span> |<span data-ttu-id="2eeaa-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2eeaa-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="2eeaa-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2eeaa-110">Delegated (work or school account)</span></span>|<span data-ttu-id="2eeaa-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2eeaa-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="2eeaa-112">Delegiert (persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="2eeaa-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="2eeaa-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2eeaa-113">Not supported.</span></span>|
|<span data-ttu-id="2eeaa-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2eeaa-114">Application</span></span>|<span data-ttu-id="2eeaa-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2eeaa-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2eeaa-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2eeaa-116">HTTP request</span></span>

```
POST /financials/companies('{id}')/customerPaymentJournals('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2eeaa-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="2eeaa-117">Optional query parameters</span></span>
<span data-ttu-id="2eeaa-118">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2eeaa-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2eeaa-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2eeaa-119">Request headers</span></span>
|<span data-ttu-id="2eeaa-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2eeaa-120">Header</span></span>        |<span data-ttu-id="2eeaa-121">Wert</span><span class="sxs-lookup"><span data-stu-id="2eeaa-121">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="2eeaa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2eeaa-122">Authorization</span></span> |<span data-ttu-id="2eeaa-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2eeaa-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2eeaa-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2eeaa-125">Content-Type</span></span>  |<span data-ttu-id="2eeaa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2eeaa-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="2eeaa-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2eeaa-127">Request body</span></span>
<span data-ttu-id="2eeaa-128">Geben Sie im Anforderungstext eine JSON-Darstellung des **customerPaymentJournals** -Objekts an.</span><span class="sxs-lookup"><span data-stu-id="2eeaa-128">In the request body, supply a JSON representation of **customerPaymentJournals** object.</span></span>

## <a name="response"></a><span data-ttu-id="2eeaa-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="2eeaa-129">Response</span></span>
<span data-ttu-id="2eeaa-130">Bei erfolgreicher Ausführung gibt diese Methode ```201 Created``` den Antwortcode und ein **customerPaymentJournals** -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2eeaa-130">If successful, this method returns ```201 Created``` response code and a **customerPaymentJournals** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2eeaa-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2eeaa-131">Example</span></span>

<span data-ttu-id="2eeaa-132">**Anforderung**</span><span class="sxs-lookup"><span data-stu-id="2eeaa-132">**Request**</span></span>

<span data-ttu-id="2eeaa-133">Hier ist ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2eeaa-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/customerPaymentJournals
Content-type: application/json

```json
{
  "code": "DEFAULT"
}
```

<span data-ttu-id="2eeaa-134">**Antwort**</span><span class="sxs-lookup"><span data-stu-id="2eeaa-134">**Response**</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "DEFAULT",
  "displayName": "Default Journal Batch",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```


