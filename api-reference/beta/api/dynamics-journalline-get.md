---
title: JournalLines abrufen
description: Ruft ein Journal Zeile-Objekt in Dynamics 365 Business Central ab.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 361731a346d1a7e649d92629d41d9aa83a4cf5d2
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366662"
---
# <a name="get-journallines"></a><span data-ttu-id="a978b-103">JournalLines abrufen</span><span class="sxs-lookup"><span data-stu-id="a978b-103">Get journalLines</span></span>
<span data-ttu-id="a978b-104">Dient zum Abrufen der Eigenschaften und Beziehungen eines Journal linienobjekts für Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="a978b-104">Retrieve the properties and relationships of a journal line object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="a978b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a978b-105">Permissions</span></span>
<span data-ttu-id="a978b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a978b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a978b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a978b-108">Permission type</span></span> |<span data-ttu-id="a978b-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a978b-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="a978b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a978b-110">Delegated (work or school account)</span></span>|<span data-ttu-id="a978b-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a978b-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="a978b-112">Delegiert (persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="a978b-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="a978b-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a978b-113">Not supported.</span></span>|
|<span data-ttu-id="a978b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a978b-114">Application</span></span>|<span data-ttu-id="a978b-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a978b-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a978b-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a978b-116">HTTP request</span></span>

```
GET /financials/companies('{id}')/journals('{id}')/journalLines('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a978b-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a978b-117">Optional query parameters</span></span>
<span data-ttu-id="a978b-118">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a978b-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a978b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a978b-119">Request headers</span></span>
|<span data-ttu-id="a978b-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a978b-120">Header</span></span>       |<span data-ttu-id="a978b-121">Wert</span><span class="sxs-lookup"><span data-stu-id="a978b-121">Value</span></span>                     |
|-------------|--------------------------|
|<span data-ttu-id="a978b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a978b-122">Authorization</span></span>|<span data-ttu-id="a978b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a978b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a978b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a978b-125">Request body</span></span>
<span data-ttu-id="a978b-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a978b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a978b-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="a978b-127">Response</span></span>
<span data-ttu-id="a978b-128">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein **journalLines** -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a978b-128">If successful, this method returns a `200 OK` response code and a **journalLines** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a978b-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a978b-129">Example</span></span>

<span data-ttu-id="a978b-130">**Anforderung**</span><span class="sxs-lookup"><span data-stu-id="a978b-130">**Request**</span></span>

<span data-ttu-id="a978b-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a978b-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/journals('{id}')/journalLines('{id}')
```

<span data-ttu-id="a978b-132">**Antwort**</span><span class="sxs-lookup"><span data-stu-id="a978b-132">**Response**</span></span>

<span data-ttu-id="a978b-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a978b-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="a978b-134">**Hinweis**: das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="a978b-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a978b-135">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="a978b-135">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "journalDisplayName": "DEFAULT",
  "lineNumber": 10000,
  "accountId": "id-value",
  "accountNumber": "10400",
  "postingDate": "2015-12-31",
  "documentNumber": "1234",
  "externalDocumentNumber": "",
  "amount": 1500,
  "description": "Accounts Receivable",
  "comment": "",
  "lastModifiedDateTime": "2017-03-17T19:02:22.043Z"
}
```

