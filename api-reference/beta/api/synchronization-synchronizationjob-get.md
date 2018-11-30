---
title: Abrufen von synchronizationJob
description: Abrufen der vorhandenen Synchronisierungsauftrag und seine Eigenschaften.
ms.openlocfilehash: c0c999d5b9ce168ba3f21af20ec5cff026d68f8d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065638"
---
# <a name="get-synchronizationjob"></a><span data-ttu-id="0ece8-103">Abrufen von synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="0ece8-103">Get synchronizationJob</span></span>

> <span data-ttu-id="0ece8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0ece8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ece8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0ece8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0ece8-106">Abrufen der vorhandenen Synchronisierungsauftrag und seine Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="0ece8-106">Retrieve the existing synchronization job and its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ece8-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0ece8-107">Permissions</span></span>
<span data-ttu-id="0ece8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ece8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ece8-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0ece8-110">Permission type</span></span>                        | <span data-ttu-id="0ece8-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0ece8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ece8-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0ece8-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="0ece8-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ece8-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="0ece8-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0ece8-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="0ece8-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0ece8-115">Not supported.</span></span>  |
|<span data-ttu-id="0ece8-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0ece8-116">Application</span></span>                            |<span data-ttu-id="0ece8-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0ece8-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0ece8-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0ece8-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="0ece8-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0ece8-119">Request headers</span></span>

| <span data-ttu-id="0ece8-120">Name</span><span class="sxs-lookup"><span data-stu-id="0ece8-120">Name</span></span>           | <span data-ttu-id="0ece8-121">Typ</span><span class="sxs-lookup"><span data-stu-id="0ece8-121">Type</span></span>    | <span data-ttu-id="0ece8-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0ece8-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="0ece8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ece8-123">Authorization</span></span>  | <span data-ttu-id="0ece8-124">string</span><span class="sxs-lookup"><span data-stu-id="0ece8-124">string</span></span>  | <span data-ttu-id="0ece8-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0ece8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ece8-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0ece8-127">Request body</span></span>

<span data-ttu-id="0ece8-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0ece8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ece8-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="0ece8-129">Response</span></span>

<span data-ttu-id="0ece8-130">Bei erfolgreicher gibt eine `200 OK` Antwort mit einer [SynchronizationJob](../resources/synchronization-synchronizationjob.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0ece8-130">If successful, returns a `200 OK` response with a [synchronizationJob](../resources/synchronization-synchronizationjob.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ece8-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0ece8-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0ece8-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0ece8-132">Request</span></span>
<span data-ttu-id="0ece8-133">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0ece8-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

##### <a name="response"></a><span data-ttu-id="0ece8-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="0ece8-134">Response</span></span>
<span data-ttu-id="0ece8-135">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="0ece8-135">The following is an example of a response.</span></span> 

><span data-ttu-id="0ece8-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="0ece8-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2577

{
    "id": "{jobId}",
    "templateId": "BoxOutDelta",
    "schedule": {
        "expiration": null,
        "interval": "P10675199DT2H48M5.4775807S",
        "state": "Disabled"
    },
    "status": {
        "countSuccessiveCompleteFailures": 0,
        "escrowsPruned": false,
        "synchronizedEntryCountByType": [],
        "code": "Paused",
        "lastExecution": null,
        "lastSuccessfulExecution": null,
        "progress": [],
        "lastSuccessfulExecutionWithExports": null,
        "steadyStateFirstAchievedTime": "0001-01-01T00:00:00Z",
        "steadyStateLastAchievedTime": "0001-01-01T00:00:00Z",
        "quarantine": null,
        "troubleshootingUrl": null
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->