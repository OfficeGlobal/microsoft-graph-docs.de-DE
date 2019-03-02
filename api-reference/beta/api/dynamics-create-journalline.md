---
title: JournalLines erstellen
description: Erstellt eine Journal Zeile in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: c6ed8b1ccbe1f33cad174e1c5e4f9b3832f2a5c9
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365423"
---
# <a name="create-journallines"></a><span data-ttu-id="f47e4-103">JournalLines erstellen</span><span class="sxs-lookup"><span data-stu-id="f47e4-103">Create journalLines</span></span>
<span data-ttu-id="f47e4-104">Erstellt ein Journal Zeile-Objekt in Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="f47e4-104">Creates a journal line object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="f47e4-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f47e4-105">Permissions</span></span>
<span data-ttu-id="f47e4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f47e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f47e4-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f47e4-108">Permission type</span></span> |<span data-ttu-id="f47e4-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f47e4-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="f47e4-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f47e4-110">Delegated (work or school account)</span></span>|<span data-ttu-id="f47e4-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f47e4-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="f47e4-112">Delegiert (persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="f47e4-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="f47e4-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f47e4-113">Not supported.</span></span>|
|<span data-ttu-id="f47e4-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f47e4-114">Application</span></span>|<span data-ttu-id="f47e4-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f47e4-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f47e4-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f47e4-116">HTTP request</span></span>

```
POST /financials/companies('{id}')/journals('{id}')/journalLines('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f47e4-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f47e4-117">Optional query parameters</span></span>
<span data-ttu-id="f47e4-118">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f47e4-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f47e4-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f47e4-119">Request headers</span></span>
|<span data-ttu-id="f47e4-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f47e4-120">Header</span></span>        |<span data-ttu-id="f47e4-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f47e4-121">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="f47e4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f47e4-122">Authorization</span></span> |<span data-ttu-id="f47e4-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f47e4-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f47e4-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f47e4-125">Content-Type</span></span>  |<span data-ttu-id="f47e4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f47e4-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="f47e4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f47e4-127">Request body</span></span>
<span data-ttu-id="f47e4-128">Geben Sie im Anforderungstext eine JSON-Darstellung des **journalLines** -Objekts an.</span><span class="sxs-lookup"><span data-stu-id="f47e4-128">In the request body, supply a JSON representation of **journalLines** object.</span></span>

## <a name="response"></a><span data-ttu-id="f47e4-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f47e4-129">Response</span></span>
<span data-ttu-id="f47e4-130">Bei erfolgreicher Ausführung gibt diese Methode ```201 Created``` den Antwortcode und das **journalLines** -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f47e4-130">If successful, this method returns ```201 Created``` response code and **journalLines** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f47e4-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f47e4-131">Example</span></span>

<span data-ttu-id="f47e4-132">**Anforderung**</span><span class="sxs-lookup"><span data-stu-id="f47e4-132">**Request**</span></span>

<span data-ttu-id="f47e4-133">Hier ist ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f47e4-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/journals('{id}')/journalLines
Content-type: application/json

{
  "lineNumber": 10000,
  "accountId": "id-value",
  "accountNumber": "10400",
  "postingDate": "2015-12-31",
  "documentNumber": "1234",
  "externalDocumentNumber": "",
  "amount": 1500,
  "description": "Accounts Receivable",
  "comment": ""
}
```
<span data-ttu-id="f47e4-134">**Antwort**</span><span class="sxs-lookup"><span data-stu-id="f47e4-134">**Response**</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

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


