---
title: Liste Aufträge für die Synchronisierung
description: Vorhandene Aufträge für eine Instanz einer Anwendung (Service Principal) auflisten.
ms.openlocfilehash: 179a6906936fddbfc31ffc7b016de05908f2383a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064564"
---
# <a name="list-synchronization-jobs"></a><span data-ttu-id="90508-103">Liste Aufträge für die Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="90508-103">List synchronization jobs</span></span>

> <span data-ttu-id="90508-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="90508-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="90508-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="90508-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="90508-106">Vorhandene Aufträge für eine Instanz einer Anwendung (Service Principal) auflisten.</span><span class="sxs-lookup"><span data-stu-id="90508-106">List existing jobs for a given application instance (service principal).</span></span>

## <a name="permissions"></a><span data-ttu-id="90508-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="90508-107">Permissions</span></span>
<span data-ttu-id="90508-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90508-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90508-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="90508-110">Permission type</span></span>                        | <span data-ttu-id="90508-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="90508-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="90508-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="90508-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="90508-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90508-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="90508-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="90508-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="90508-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="90508-115">Not supported.</span></span> |
|<span data-ttu-id="90508-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="90508-116">Application</span></span>                            |<span data-ttu-id="90508-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="90508-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="90508-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="90508-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="90508-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="90508-119">Request headers</span></span>

| <span data-ttu-id="90508-120">Name</span><span class="sxs-lookup"><span data-stu-id="90508-120">Name</span></span>           | <span data-ttu-id="90508-121">Typ</span><span class="sxs-lookup"><span data-stu-id="90508-121">Type</span></span>    | <span data-ttu-id="90508-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="90508-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="90508-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="90508-123">Authorization</span></span>  | <span data-ttu-id="90508-124">string</span><span class="sxs-lookup"><span data-stu-id="90508-124">string</span></span>  | <span data-ttu-id="90508-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="90508-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90508-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="90508-127">Request body</span></span>

<span data-ttu-id="90508-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="90508-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90508-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="90508-129">Response</span></span>

<span data-ttu-id="90508-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [SynchronizationJob](../resources/synchronization-synchronizationjob.md) .</span><span class="sxs-lookup"><span data-stu-id="90508-130">If successful, this method returns a `200 OK` response code and a collection of [synchronizationJob](../resources/synchronization-synchronizationjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90508-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="90508-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="90508-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="90508-132">Request</span></span>
<span data-ttu-id="90508-133">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="90508-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_jobs"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/
```

##### <a name="response"></a><span data-ttu-id="90508-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="90508-134">Response</span></span>
<span data-ttu-id="90508-135">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="90508-135">The following is an example of a response.</span></span> 

><span data-ttu-id="90508-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="90508-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationJob",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2958

{
    "value": [
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
                "lastSuccessfulExecutionWithExports": null,
                "steadyStateFirstAchievedTime": "0001-01-01T00:00:00Z",
                "steadyStateLastAchievedTime": "0001-01-01T00:00:00Z",
                "quarantine": null,
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List jobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->