---
title: Erstellen von synchronizationJob
description: Erstellen Sie neue Synchronisierungsauftrag mit ein Standardschema für die Synchronisierung aus. Der Auftrag wird in deaktiviertem Zustand erstellt. Rufen Sie Start Auftrag zur Synchronisierung starten.
localization_priority: Normal
ms.openlocfilehash: 04b8e383c923968b150067c9d2c3a65ce32bd9c0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842224"
---
# <a name="create-synchronizationjob"></a><span data-ttu-id="f9a81-105">Erstellen von synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="f9a81-105">Create synchronizationJob</span></span>

> <span data-ttu-id="f9a81-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f9a81-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9a81-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f9a81-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f9a81-108">Erstellen Sie neue Synchronisierungsauftrag mit ein Standardschema für die Synchronisierung aus.</span><span class="sxs-lookup"><span data-stu-id="f9a81-108">Create new synchronization job with a default synchronization schema.</span></span> <span data-ttu-id="f9a81-109">Der Auftrag wird in deaktiviertem Zustand erstellt.</span><span class="sxs-lookup"><span data-stu-id="f9a81-109">The job is created in a disabled state.</span></span> <span data-ttu-id="f9a81-110">Rufen Sie [Auftrag starten](synchronization-synchronizationjob-start.md) , um die Synchronisierung starten.</span><span class="sxs-lookup"><span data-stu-id="f9a81-110">Call [Start job](synchronization-synchronizationjob-start.md) to start synchronization.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9a81-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f9a81-111">Permissions</span></span>
<span data-ttu-id="f9a81-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9a81-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9a81-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f9a81-114">Permission type</span></span>                        | <span data-ttu-id="f9a81-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f9a81-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9a81-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f9a81-116">Delegated (work or school account)</span></span>     |<span data-ttu-id="f9a81-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9a81-117">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="f9a81-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f9a81-118">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="f9a81-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f9a81-119">Not supported.</span></span>|
|<span data-ttu-id="f9a81-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f9a81-120">Application</span></span>                            |<span data-ttu-id="f9a81-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f9a81-121">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="f9a81-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f9a81-122">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="f9a81-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f9a81-123">Request headers</span></span>

| <span data-ttu-id="f9a81-124">Name</span><span class="sxs-lookup"><span data-stu-id="f9a81-124">Name</span></span>           | <span data-ttu-id="f9a81-125">Typ</span><span class="sxs-lookup"><span data-stu-id="f9a81-125">Type</span></span>    | <span data-ttu-id="f9a81-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f9a81-126">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="f9a81-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9a81-127">Authorization</span></span>  | <span data-ttu-id="f9a81-128">string</span><span class="sxs-lookup"><span data-stu-id="f9a81-128">string</span></span>  | <span data-ttu-id="f9a81-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f9a81-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9a81-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f9a81-131">Request body</span></span>

<span data-ttu-id="f9a81-132">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [SynchronizationJob](../resources/synchronization-synchronizationjob.md) -Objekts erstellt werden soll.</span><span class="sxs-lookup"><span data-stu-id="f9a81-132">In the request body, supply a JSON representation of the [synchronizationJob](../resources/synchronization-synchronizationjob.md) object to be created.</span></span> <span data-ttu-id="f9a81-133">Ist die einzige erforderliche Eigenschaft `templateId`.</span><span class="sxs-lookup"><span data-stu-id="f9a81-133">The only required property is `templateId`.</span></span> <span data-ttu-id="f9a81-134">Die `templateId` Eigenschaft muss eine der Vorlagen erstellt für diese Anwendung/Dienstprinzipal übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="f9a81-134">The `templateId` property must match one of the templates created for this application/service principal.</span></span> <span data-ttu-id="f9a81-135">Verwenden Sie verfügbare Vorlagen, um [Listenvorlagen](synchronization-synchronizationtemplate-list.md).</span><span class="sxs-lookup"><span data-stu-id="f9a81-135">To find available templates, use [List templates](synchronization-synchronizationtemplate-list.md).</span></span>

## <a name="response"></a><span data-ttu-id="f9a81-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="f9a81-136">Response</span></span>

<span data-ttu-id="f9a81-137">Bei erfolgreicher gibt eine `201 Created` Antwortcode und eines [SynchronizationJob](../resources/synchronization-synchronizationjob.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f9a81-137">If successful, returns a `201 Created` response code and a [synchronizationJob](../resources/synchronization-synchronizationjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9a81-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f9a81-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f9a81-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f9a81-139">Request</span></span>
<span data-ttu-id="f9a81-140">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f9a81-140">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_synchronizationjob_from_synchronization"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
Content-type: application/json

{ 
    "templateId": "BoxOutDelta"
}
```

##### <a name="response"></a><span data-ttu-id="f9a81-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="f9a81-141">Response</span></span>
<span data-ttu-id="f9a81-142">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="f9a81-142">The following is an example of a response.</span></span> 

><span data-ttu-id="f9a81-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="f9a81-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

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
        "code": "NotConfigured",
        "lastExecution": null,
        "lastSuccessfulExecution": null,
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
  "description": "Create synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
