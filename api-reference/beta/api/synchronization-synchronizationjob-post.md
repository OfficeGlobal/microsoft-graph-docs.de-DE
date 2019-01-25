---
title: Erstellen von synchronizationJob
description: Erstellen Sie neue Synchronisierungsauftrag mit ein Standardschema für die Synchronisierung aus. Der Auftrag wird in deaktiviertem Zustand erstellt. Rufen Sie Start Auftrag zur Synchronisierung starten.
localization_priority: Normal
ms.openlocfilehash: f41ebe87d8ca935a355c37ea53d1c7bd62b1652e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507915"
---
# <a name="create-synchronizationjob"></a><span data-ttu-id="8b1c0-105">Erstellen von synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="8b1c0-105">Create synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b1c0-106">Erstellen Sie neue Synchronisierungsauftrag mit ein Standardschema für die Synchronisierung aus.</span><span class="sxs-lookup"><span data-stu-id="8b1c0-106">Create new synchronization job with a default synchronization schema.</span></span> <span data-ttu-id="8b1c0-107">Der Auftrag wird in deaktiviertem Zustand erstellt.</span><span class="sxs-lookup"><span data-stu-id="8b1c0-107">The job is created in a disabled state.</span></span> <span data-ttu-id="8b1c0-108">Rufen Sie [Auftrag starten](synchronization-synchronizationjob-start.md) , um die Synchronisierung starten.</span><span class="sxs-lookup"><span data-stu-id="8b1c0-108">Call [Start job](synchronization-synchronizationjob-start.md) to start synchronization.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b1c0-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8b1c0-109">Permissions</span></span>
<span data-ttu-id="8b1c0-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b1c0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b1c0-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8b1c0-112">Permission type</span></span>                        | <span data-ttu-id="8b1c0-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8b1c0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b1c0-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8b1c0-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="8b1c0-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b1c0-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="8b1c0-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8b1c0-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="8b1c0-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8b1c0-117">Not supported.</span></span>|
|<span data-ttu-id="8b1c0-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8b1c0-118">Application</span></span>                            |<span data-ttu-id="8b1c0-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8b1c0-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="8b1c0-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b1c0-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="8b1c0-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8b1c0-121">Request headers</span></span>

| <span data-ttu-id="8b1c0-122">Name</span><span class="sxs-lookup"><span data-stu-id="8b1c0-122">Name</span></span>           | <span data-ttu-id="8b1c0-123">Typ</span><span class="sxs-lookup"><span data-stu-id="8b1c0-123">Type</span></span>    | <span data-ttu-id="8b1c0-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8b1c0-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="8b1c0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b1c0-125">Authorization</span></span>  | <span data-ttu-id="8b1c0-126">string</span><span class="sxs-lookup"><span data-stu-id="8b1c0-126">string</span></span>  | <span data-ttu-id="8b1c0-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8b1c0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b1c0-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8b1c0-129">Request body</span></span>

<span data-ttu-id="8b1c0-130">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [SynchronizationJob](../resources/synchronization-synchronizationjob.md) -Objekts erstellt werden soll.</span><span class="sxs-lookup"><span data-stu-id="8b1c0-130">In the request body, supply a JSON representation of the [synchronizationJob](../resources/synchronization-synchronizationjob.md) object to be created.</span></span> <span data-ttu-id="8b1c0-131">Ist die einzige erforderliche Eigenschaft `templateId`.</span><span class="sxs-lookup"><span data-stu-id="8b1c0-131">The only required property is `templateId`.</span></span> <span data-ttu-id="8b1c0-132">Die `templateId` Eigenschaft muss eine der Vorlagen erstellt für diese Anwendung/Dienstprinzipal übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="8b1c0-132">The `templateId` property must match one of the templates created for this application/service principal.</span></span> <span data-ttu-id="8b1c0-133">Verwenden Sie verfügbare Vorlagen, um [Listenvorlagen](synchronization-synchronizationtemplate-list.md).</span><span class="sxs-lookup"><span data-stu-id="8b1c0-133">To find available templates, use [List templates](synchronization-synchronizationtemplate-list.md).</span></span>

## <a name="response"></a><span data-ttu-id="8b1c0-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b1c0-134">Response</span></span>

<span data-ttu-id="8b1c0-135">Bei erfolgreicher gibt eine `201 Created` Antwortcode und eines [SynchronizationJob](../resources/synchronization-synchronizationjob.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="8b1c0-135">If successful, returns a `201 Created` response code and a [synchronizationJob](../resources/synchronization-synchronizationjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b1c0-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8b1c0-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8b1c0-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b1c0-137">Request</span></span>
<span data-ttu-id="8b1c0-138">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8b1c0-138">The following is an example of a request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="8b1c0-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b1c0-139">Response</span></span>
<span data-ttu-id="8b1c0-140">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="8b1c0-140">The following is an example of a response.</span></span> 

><span data-ttu-id="8b1c0-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="8b1c0-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Create synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
