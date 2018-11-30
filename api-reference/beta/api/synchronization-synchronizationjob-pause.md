---
title: 'SynchronizationJob: anhalten'
description: Synchronisierung vorübergehend anhalten. Der Fortschritt Auftragsstatus, einschließlich wird beibehalten, und der Auftrag wird weiterhin aus, wo es beim Start aufgerufen wird unterbrochen.
ms.openlocfilehash: dd46f5760d7ddcfff1e254d7c000e1cd80304f07
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060647"
---
# <a name="synchronizationjob-pause"></a><span data-ttu-id="4919c-104">SynchronizationJob: anhalten</span><span class="sxs-lookup"><span data-stu-id="4919c-104">synchronizationJob: pause</span></span>

> <span data-ttu-id="4919c-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4919c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4919c-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4919c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4919c-107">Synchronisierung vorübergehend anhalten.</span><span class="sxs-lookup"><span data-stu-id="4919c-107">Temporarily stop synchronization.</span></span> <span data-ttu-id="4919c-108">Der Fortschritt Auftragsstatus, einschließlich wird beibehalten, und der Auftrag wird weiterhin aus, wo es beim [Starten](../api/synchronization-synchronizationjob-start.md) aufgerufen wird unterbrochen.</span><span class="sxs-lookup"><span data-stu-id="4919c-108">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>

## <a name="permissions"></a><span data-ttu-id="4919c-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4919c-109">Permissions</span></span>
<span data-ttu-id="4919c-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4919c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4919c-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4919c-112">Permission type</span></span>                        | <span data-ttu-id="4919c-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4919c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4919c-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4919c-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="4919c-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4919c-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="4919c-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4919c-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="4919c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4919c-117">Not supported.</span></span>  |
|<span data-ttu-id="4919c-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4919c-118">Application</span></span>                            |<span data-ttu-id="4919c-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4919c-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4919c-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4919c-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

## <a name="request-headers"></a><span data-ttu-id="4919c-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4919c-121">Request headers</span></span>

| <span data-ttu-id="4919c-122">Name</span><span class="sxs-lookup"><span data-stu-id="4919c-122">Name</span></span>           | <span data-ttu-id="4919c-123">Typ</span><span class="sxs-lookup"><span data-stu-id="4919c-123">Type</span></span>    | <span data-ttu-id="4919c-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4919c-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="4919c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4919c-125">Authorization</span></span>  | <span data-ttu-id="4919c-126">string</span><span class="sxs-lookup"><span data-stu-id="4919c-126">string</span></span>  | <span data-ttu-id="4919c-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4919c-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4919c-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4919c-129">Request body</span></span>

<span data-ttu-id="4919c-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4919c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4919c-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="4919c-131">Response</span></span>

<span data-ttu-id="4919c-132">Bei erfolgreicher gibt eine `204 No Content` Antwort.</span><span class="sxs-lookup"><span data-stu-id="4919c-132">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="4919c-133">Es gibt keine Suchzeichenfolge im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4919c-133">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4919c-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4919c-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4919c-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4919c-135">Request</span></span>
<span data-ttu-id="4919c-136">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4919c-136">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_pause"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

##### <a name="response"></a><span data-ttu-id="4919c-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="4919c-137">Response</span></span>
<span data-ttu-id="4919c-138">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="4919c-138">The following is an example of a response.</span></span>
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
  "description": "synchronizationJob: pause",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->