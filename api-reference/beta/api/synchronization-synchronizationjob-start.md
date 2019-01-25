---
title: SynchronizationJob starten
description: Starten Sie eine vorhandene Synchronisierungsauftrag. Wenn der Auftrag angehalten ist, wird Verarbeitung Änderungen an der Stelle fortgesetzt, in dem er angehalten wurde. Wenn der Auftrag in Quarantäne befindet, wird der Quarantänestatus gelöscht.
localization_priority: Normal
ms.openlocfilehash: 4648d9d3d889adf2cd7ec06e4fcf79b761c77132
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515370"
---
# <a name="start-synchronizationjob"></a><span data-ttu-id="5ea71-105">SynchronizationJob starten</span><span class="sxs-lookup"><span data-stu-id="5ea71-105">Start synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ea71-106">Starten Sie eine vorhandene Synchronisierungsauftrag.</span><span class="sxs-lookup"><span data-stu-id="5ea71-106">Start an existing synchronization job.</span></span> <span data-ttu-id="5ea71-107">Wenn der Auftrag angehalten ist, wird Verarbeitung Änderungen an der Stelle fortgesetzt, in dem er angehalten wurde.</span><span class="sxs-lookup"><span data-stu-id="5ea71-107">If the job is in a paused state, it will continue processing changes from the point where it was paused.</span></span> <span data-ttu-id="5ea71-108">Wenn der Auftrag in Quarantäne befindet, wird der Quarantänestatus gelöscht.</span><span class="sxs-lookup"><span data-stu-id="5ea71-108">If the job is in quarantine, the quarantine status will be cleared.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ea71-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5ea71-109">Permissions</span></span>
<span data-ttu-id="5ea71-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ea71-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ea71-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5ea71-112">Permission type</span></span>                        | <span data-ttu-id="5ea71-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5ea71-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ea71-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5ea71-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="5ea71-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ea71-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="5ea71-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5ea71-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="5ea71-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5ea71-117">Not supported.</span></span> |
|<span data-ttu-id="5ea71-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5ea71-118">Application</span></span>                            |<span data-ttu-id="5ea71-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5ea71-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5ea71-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5ea71-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="5ea71-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5ea71-121">Request headers</span></span>

| <span data-ttu-id="5ea71-122">Name</span><span class="sxs-lookup"><span data-stu-id="5ea71-122">Name</span></span>           | <span data-ttu-id="5ea71-123">Typ</span><span class="sxs-lookup"><span data-stu-id="5ea71-123">Type</span></span>    | <span data-ttu-id="5ea71-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5ea71-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="5ea71-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ea71-125">Authorization</span></span>  | <span data-ttu-id="5ea71-126">string</span><span class="sxs-lookup"><span data-stu-id="5ea71-126">string</span></span>  | <span data-ttu-id="5ea71-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5ea71-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ea71-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5ea71-129">Request body</span></span>

<span data-ttu-id="5ea71-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5ea71-130">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="5ea71-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="5ea71-131">Response</span></span>

<span data-ttu-id="5ea71-132">Bei erfolgreicher gibt eine `204 No Content` Antwort.</span><span class="sxs-lookup"><span data-stu-id="5ea71-132">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="5ea71-133">Es gibt keine Suchzeichenfolge im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5ea71-133">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ea71-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5ea71-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5ea71-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5ea71-135">Request</span></span>
<span data-ttu-id="5ea71-136">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5ea71-136">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

##### <a name="response"></a><span data-ttu-id="5ea71-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="5ea71-137">Response</span></span>
<span data-ttu-id="5ea71-138">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="5ea71-138">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob: start",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-start.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
