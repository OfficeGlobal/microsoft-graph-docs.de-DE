---
title: 'SynchronizationJob: anhalten'
description: Synchronisierung vorübergehend anhalten. Der Fortschritt Auftragsstatus, einschließlich wird beibehalten, und der Auftrag wird weiterhin aus, wo es beim Start aufgerufen wird unterbrochen.
localization_priority: Normal
ms.openlocfilehash: 9f8cac05511b5efd17234ccf16b763999418bf2a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513921"
---
# <a name="synchronizationjob-pause"></a><span data-ttu-id="0cd39-104">SynchronizationJob: anhalten</span><span class="sxs-lookup"><span data-stu-id="0cd39-104">synchronizationJob: pause</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cd39-105">Synchronisierung vorübergehend anhalten.</span><span class="sxs-lookup"><span data-stu-id="0cd39-105">Temporarily stop synchronization.</span></span> <span data-ttu-id="0cd39-106">Der Fortschritt Auftragsstatus, einschließlich wird beibehalten, und der Auftrag wird weiterhin aus, wo es beim [Starten](../api/synchronization-synchronizationjob-start.md) aufgerufen wird unterbrochen.</span><span class="sxs-lookup"><span data-stu-id="0cd39-106">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>

## <a name="permissions"></a><span data-ttu-id="0cd39-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0cd39-107">Permissions</span></span>
<span data-ttu-id="0cd39-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cd39-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cd39-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0cd39-110">Permission type</span></span>                        | <span data-ttu-id="0cd39-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0cd39-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0cd39-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0cd39-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="0cd39-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cd39-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="0cd39-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0cd39-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="0cd39-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0cd39-115">Not supported.</span></span>  |
|<span data-ttu-id="0cd39-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0cd39-116">Application</span></span>                            |<span data-ttu-id="0cd39-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0cd39-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0cd39-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0cd39-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

## <a name="request-headers"></a><span data-ttu-id="0cd39-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0cd39-119">Request headers</span></span>

| <span data-ttu-id="0cd39-120">Name</span><span class="sxs-lookup"><span data-stu-id="0cd39-120">Name</span></span>           | <span data-ttu-id="0cd39-121">Typ</span><span class="sxs-lookup"><span data-stu-id="0cd39-121">Type</span></span>    | <span data-ttu-id="0cd39-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0cd39-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="0cd39-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0cd39-123">Authorization</span></span>  | <span data-ttu-id="0cd39-124">string</span><span class="sxs-lookup"><span data-stu-id="0cd39-124">string</span></span>  | <span data-ttu-id="0cd39-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0cd39-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0cd39-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0cd39-127">Request body</span></span>

<span data-ttu-id="0cd39-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0cd39-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0cd39-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="0cd39-129">Response</span></span>

<span data-ttu-id="0cd39-130">Bei erfolgreicher gibt eine `204 No Content` Antwort.</span><span class="sxs-lookup"><span data-stu-id="0cd39-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="0cd39-131">Es gibt keine Suchzeichenfolge im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0cd39-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cd39-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0cd39-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0cd39-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0cd39-133">Request</span></span>
<span data-ttu-id="0cd39-134">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0cd39-134">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_pause"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

##### <a name="response"></a><span data-ttu-id="0cd39-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="0cd39-135">Response</span></span>
<span data-ttu-id="0cd39-136">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="0cd39-136">The following is an example of a response.</span></span>
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
  "description": "synchronizationJob: pause",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-pause.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
