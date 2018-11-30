---
title: SynchronizationJob löschen
description: Beenden Sie den Synchronisierungsauftrag und löschen Sie den zugeordneten Zustand endgültig. Synchronisierte Konten werden als Links-ist.
ms.openlocfilehash: d77101e8dfaf55a36dfd7260afb30aade81bbae8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064565"
---
# <a name="delete-synchronizationjob"></a><span data-ttu-id="bc83d-104">SynchronizationJob löschen</span><span class="sxs-lookup"><span data-stu-id="bc83d-104">Delete synchronizationJob</span></span>

> <span data-ttu-id="bc83d-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bc83d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc83d-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bc83d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bc83d-107">Beenden Sie den Synchronisierungsauftrag und löschen Sie den zugeordneten Zustand endgültig.</span><span class="sxs-lookup"><span data-stu-id="bc83d-107">Stop the synchronization job, and permanently delete all the state associated with it.</span></span> <span data-ttu-id="bc83d-108">Synchronisierte Konten werden als Links-ist.</span><span class="sxs-lookup"><span data-stu-id="bc83d-108">Synchronized accounts are left as-is.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc83d-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bc83d-109">Permissions</span></span>
<span data-ttu-id="bc83d-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc83d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc83d-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bc83d-112">Permission type</span></span>                        | <span data-ttu-id="bc83d-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bc83d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc83d-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bc83d-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="bc83d-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc83d-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="bc83d-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bc83d-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="bc83d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bc83d-117">Not supported.</span></span>  |
|<span data-ttu-id="bc83d-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bc83d-118">Application</span></span>                            |<span data-ttu-id="bc83d-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bc83d-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="bc83d-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc83d-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="bc83d-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bc83d-121">Request headers</span></span>

| <span data-ttu-id="bc83d-122">Name</span><span class="sxs-lookup"><span data-stu-id="bc83d-122">Name</span></span>           | <span data-ttu-id="bc83d-123">Typ</span><span class="sxs-lookup"><span data-stu-id="bc83d-123">Type</span></span>    | <span data-ttu-id="bc83d-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc83d-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="bc83d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc83d-125">Authorization</span></span>  | <span data-ttu-id="bc83d-126">string</span><span class="sxs-lookup"><span data-stu-id="bc83d-126">string</span></span>  | <span data-ttu-id="bc83d-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bc83d-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc83d-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bc83d-129">Request body</span></span>

<span data-ttu-id="bc83d-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bc83d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc83d-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc83d-131">Response</span></span>

<span data-ttu-id="bc83d-132">Bei erfolgreicher gibt eine `204 No Content` Antwort.</span><span class="sxs-lookup"><span data-stu-id="bc83d-132">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="bc83d-133">Es gibt keine Suchzeichenfolge im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bc83d-133">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc83d-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bc83d-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bc83d-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc83d-135">Request</span></span>
<span data-ttu-id="bc83d-136">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bc83d-136">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_synchronizationjob"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

##### <a name="response"></a><span data-ttu-id="bc83d-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc83d-137">Response</span></span>
<span data-ttu-id="bc83d-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bc83d-138">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->