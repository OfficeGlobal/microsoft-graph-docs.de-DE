---
title: SynchronizationJob starten
description: Starten Sie eine vorhandene Synchronisierungsauftrag. Wenn der Auftrag angehalten ist, wird Verarbeitung Änderungen an der Stelle fortgesetzt, in dem er angehalten wurde. Wenn der Auftrag in Quarantäne befindet, wird der Quarantänestatus gelöscht.
ms.openlocfilehash: c9f326a2c00564f25fb0ff982ede7e8454e14c8c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065034"
---
# <a name="start-synchronizationjob"></a><span data-ttu-id="f24d9-105">SynchronizationJob starten</span><span class="sxs-lookup"><span data-stu-id="f24d9-105">Start synchronizationJob</span></span>

> <span data-ttu-id="f24d9-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f24d9-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f24d9-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f24d9-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f24d9-108">Starten Sie eine vorhandene Synchronisierungsauftrag.</span><span class="sxs-lookup"><span data-stu-id="f24d9-108">Start an existing synchronization job.</span></span> <span data-ttu-id="f24d9-109">Wenn der Auftrag angehalten ist, wird Verarbeitung Änderungen an der Stelle fortgesetzt, in dem er angehalten wurde.</span><span class="sxs-lookup"><span data-stu-id="f24d9-109">If the job is in a paused state, it will continue processing changes from the point where it was paused.</span></span> <span data-ttu-id="f24d9-110">Wenn der Auftrag in Quarantäne befindet, wird der Quarantänestatus gelöscht.</span><span class="sxs-lookup"><span data-stu-id="f24d9-110">If the job is in quarantine, the quarantine status will be cleared.</span></span>

## <a name="permissions"></a><span data-ttu-id="f24d9-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f24d9-111">Permissions</span></span>
<span data-ttu-id="f24d9-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f24d9-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f24d9-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f24d9-114">Permission type</span></span>                        | <span data-ttu-id="f24d9-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f24d9-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f24d9-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f24d9-116">Delegated (work or school account)</span></span>     |<span data-ttu-id="f24d9-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f24d9-117">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="f24d9-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f24d9-118">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="f24d9-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f24d9-119">Not supported.</span></span> |
|<span data-ttu-id="f24d9-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f24d9-120">Application</span></span>                            |<span data-ttu-id="f24d9-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f24d9-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f24d9-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f24d9-122">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="f24d9-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f24d9-123">Request headers</span></span>

| <span data-ttu-id="f24d9-124">Name</span><span class="sxs-lookup"><span data-stu-id="f24d9-124">Name</span></span>           | <span data-ttu-id="f24d9-125">Typ</span><span class="sxs-lookup"><span data-stu-id="f24d9-125">Type</span></span>    | <span data-ttu-id="f24d9-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f24d9-126">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="f24d9-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="f24d9-127">Authorization</span></span>  | <span data-ttu-id="f24d9-128">string</span><span class="sxs-lookup"><span data-stu-id="f24d9-128">string</span></span>  | <span data-ttu-id="f24d9-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f24d9-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f24d9-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f24d9-131">Request body</span></span>

<span data-ttu-id="f24d9-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f24d9-132">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="f24d9-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f24d9-133">Response</span></span>

<span data-ttu-id="f24d9-134">Bei erfolgreicher gibt eine `204 No Content` Antwort.</span><span class="sxs-lookup"><span data-stu-id="f24d9-134">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="f24d9-135">Es gibt keine Suchzeichenfolge im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f24d9-135">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f24d9-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f24d9-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f24d9-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f24d9-137">Request</span></span>
<span data-ttu-id="f24d9-138">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f24d9-138">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

##### <a name="response"></a><span data-ttu-id="f24d9-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="f24d9-139">Response</span></span>
<span data-ttu-id="f24d9-140">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="f24d9-140">The following is an example of a response.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationJob: start",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
