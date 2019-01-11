---
title: Abrufen von synchronizationJob
description: Abrufen der vorhandenen Synchronisierungsauftrag und seine Eigenschaften.
localization_priority: Normal
ms.openlocfilehash: 5e6be3cc707fdb70b80c6bd2ebe924232aaa674c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850316"
---
# <a name="get-synchronizationjob"></a><span data-ttu-id="8af4e-103">Abrufen von synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="8af4e-103">Get synchronizationJob</span></span>

> <span data-ttu-id="8af4e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8af4e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8af4e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8af4e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8af4e-106">Abrufen der vorhandenen Synchronisierungsauftrag und seine Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="8af4e-106">Retrieve the existing synchronization job and its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="8af4e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8af4e-107">Permissions</span></span>
<span data-ttu-id="8af4e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8af4e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8af4e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8af4e-110">Permission type</span></span>                        | <span data-ttu-id="8af4e-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8af4e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8af4e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8af4e-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="8af4e-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8af4e-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="8af4e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8af4e-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="8af4e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8af4e-115">Not supported.</span></span>  |
|<span data-ttu-id="8af4e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8af4e-116">Application</span></span>                            |<span data-ttu-id="8af4e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8af4e-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8af4e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8af4e-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="8af4e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8af4e-119">Request headers</span></span>

| <span data-ttu-id="8af4e-120">Name</span><span class="sxs-lookup"><span data-stu-id="8af4e-120">Name</span></span>           | <span data-ttu-id="8af4e-121">Typ</span><span class="sxs-lookup"><span data-stu-id="8af4e-121">Type</span></span>    | <span data-ttu-id="8af4e-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8af4e-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="8af4e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8af4e-123">Authorization</span></span>  | <span data-ttu-id="8af4e-124">string</span><span class="sxs-lookup"><span data-stu-id="8af4e-124">string</span></span>  | <span data-ttu-id="8af4e-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8af4e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8af4e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8af4e-127">Request body</span></span>

<span data-ttu-id="8af4e-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8af4e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8af4e-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="8af4e-129">Response</span></span>

<span data-ttu-id="8af4e-130">Bei erfolgreicher gibt eine `200 OK` Antwort mit einer [SynchronizationJob](../resources/synchronization-synchronizationjob.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="8af4e-130">If successful, returns a `200 OK` response with a [synchronizationJob](../resources/synchronization-synchronizationjob.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8af4e-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8af4e-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8af4e-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8af4e-132">Request</span></span>
<span data-ttu-id="8af4e-133">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8af4e-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

##### <a name="response"></a><span data-ttu-id="8af4e-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="8af4e-134">Response</span></span>
<span data-ttu-id="8af4e-135">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="8af4e-135">The following is an example of a response.</span></span> 

><span data-ttu-id="8af4e-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="8af4e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
