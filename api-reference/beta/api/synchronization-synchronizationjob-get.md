---
title: Abrufen von synchronizationJob
description: Abrufen der vorhandenen Synchronisierungsauftrag und seine Eigenschaften.
localization_priority: Normal
ms.openlocfilehash: bb7c61192b165e5d05c0bb3434488ed2ff7ee8c3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521691"
---
# <a name="get-synchronizationjob"></a><span data-ttu-id="a650e-103">Abrufen von synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="a650e-103">Get synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a650e-104">Abrufen der vorhandenen Synchronisierungsauftrag und seine Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="a650e-104">Retrieve the existing synchronization job and its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="a650e-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a650e-105">Permissions</span></span>
<span data-ttu-id="a650e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a650e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a650e-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a650e-108">Permission type</span></span>                        | <span data-ttu-id="a650e-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a650e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a650e-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a650e-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="a650e-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a650e-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="a650e-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a650e-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="a650e-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a650e-113">Not supported.</span></span>  |
|<span data-ttu-id="a650e-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a650e-114">Application</span></span>                            |<span data-ttu-id="a650e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a650e-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a650e-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a650e-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="a650e-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a650e-117">Request headers</span></span>

| <span data-ttu-id="a650e-118">Name</span><span class="sxs-lookup"><span data-stu-id="a650e-118">Name</span></span>           | <span data-ttu-id="a650e-119">Typ</span><span class="sxs-lookup"><span data-stu-id="a650e-119">Type</span></span>    | <span data-ttu-id="a650e-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a650e-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="a650e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a650e-121">Authorization</span></span>  | <span data-ttu-id="a650e-122">string</span><span class="sxs-lookup"><span data-stu-id="a650e-122">string</span></span>  | <span data-ttu-id="a650e-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a650e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a650e-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a650e-125">Request body</span></span>

<span data-ttu-id="a650e-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a650e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a650e-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="a650e-127">Response</span></span>

<span data-ttu-id="a650e-128">Bei erfolgreicher gibt eine `200 OK` Antwort mit einer [SynchronizationJob](../resources/synchronization-synchronizationjob.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="a650e-128">If successful, returns a `200 OK` response with a [synchronizationJob](../resources/synchronization-synchronizationjob.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a650e-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a650e-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a650e-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a650e-130">Request</span></span>
<span data-ttu-id="a650e-131">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a650e-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

##### <a name="response"></a><span data-ttu-id="a650e-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="a650e-132">Response</span></span>
<span data-ttu-id="a650e-133">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="a650e-133">The following is an example of a response.</span></span> 

><span data-ttu-id="a650e-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="a650e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
