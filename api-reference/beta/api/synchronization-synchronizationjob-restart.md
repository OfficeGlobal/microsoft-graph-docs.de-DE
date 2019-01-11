---
title: Starten Sie SynchronizationJob neu
description: Starten Sie den Synchronisierungsauftrag erzwingen, um alle Objekte im Verzeichnis erneut zu verarbeiten. Optional löscht vorhandene Synchronisierungsstatus und vorherigen Fehler.
localization_priority: Normal
ms.openlocfilehash: 154ae4234eea6fb3499d36720e71b40cac727f9c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841027"
---
# <a name="restart-synchronizationjob"></a><span data-ttu-id="903f9-104">Starten Sie SynchronizationJob neu</span><span class="sxs-lookup"><span data-stu-id="903f9-104">Restart synchronizationJob</span></span>

> <span data-ttu-id="903f9-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="903f9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="903f9-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="903f9-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="903f9-107">Starten Sie den Synchronisierungsauftrag erzwingen, um alle Objekte im Verzeichnis erneut zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="903f9-107">Restart the synchronization job, forcing it to reprocess all the objects in the directory.</span></span> <span data-ttu-id="903f9-108">Optional löscht vorhandene Synchronisierungsstatus und vorherigen Fehler.</span><span class="sxs-lookup"><span data-stu-id="903f9-108">Optionally clears existing synchronization state and previous errors.</span></span>

## <a name="permissions"></a><span data-ttu-id="903f9-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="903f9-109">Permissions</span></span>
<span data-ttu-id="903f9-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="903f9-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="903f9-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="903f9-112">Permission type</span></span>                        | <span data-ttu-id="903f9-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="903f9-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="903f9-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="903f9-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="903f9-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="903f9-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="903f9-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="903f9-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="903f9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="903f9-117">Not supported.</span></span> |
|<span data-ttu-id="903f9-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="903f9-118">Application</span></span>                            |<span data-ttu-id="903f9-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="903f9-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="903f9-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="903f9-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
```

## <a name="request-headers"></a><span data-ttu-id="903f9-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="903f9-121">Request headers</span></span>

| <span data-ttu-id="903f9-122">Name</span><span class="sxs-lookup"><span data-stu-id="903f9-122">Name</span></span>           | <span data-ttu-id="903f9-123">Typ</span><span class="sxs-lookup"><span data-stu-id="903f9-123">Type</span></span>    | <span data-ttu-id="903f9-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="903f9-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="903f9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="903f9-125">Authorization</span></span>  | <span data-ttu-id="903f9-126">string</span><span class="sxs-lookup"><span data-stu-id="903f9-126">string</span></span>  | <span data-ttu-id="903f9-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="903f9-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="903f9-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="903f9-129">Request body</span></span>

<span data-ttu-id="903f9-130">Geben Sie im Textkörper Anforderung ein JSON-Objekt mit dem folgenden Parameter ein.</span><span class="sxs-lookup"><span data-stu-id="903f9-130">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="903f9-131">Parameter</span><span class="sxs-lookup"><span data-stu-id="903f9-131">Parameter</span></span>     | <span data-ttu-id="903f9-132">Typ</span><span class="sxs-lookup"><span data-stu-id="903f9-132">Type</span></span>      | <span data-ttu-id="903f9-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="903f9-133">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="903f9-134">criteria</span><span class="sxs-lookup"><span data-stu-id="903f9-134">criteria</span></span>       |[<span data-ttu-id="903f9-135">synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="903f9-135">synchronizationJobRestartCriteria</span></span>](../resources/synchronization-synchronizationjobrestartcriteria.md) |<span data-ttu-id="903f9-136">Starten Sie Kriterien</span><span class="sxs-lookup"><span data-stu-id="903f9-136">Restart criteria</span></span>|

## <a name="response"></a><span data-ttu-id="903f9-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="903f9-137">Response</span></span>

<span data-ttu-id="903f9-138">Bei erfolgreicher gibt eine `204 No Content` Antwort.</span><span class="sxs-lookup"><span data-stu-id="903f9-138">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="903f9-139">Es gibt keine Suchzeichenfolge im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="903f9-139">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="903f9-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="903f9-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="903f9-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="903f9-141">Request</span></span>
<span data-ttu-id="903f9-142">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="903f9-142">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_restart"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
Authorization: Bearer <token>
Content-type: application/json

{
   "criteria": {
       "resetScope": "ConnectorDataStore, Escrows, QuarantineState"
   }
}
```

##### <a name="response"></a><span data-ttu-id="903f9-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="903f9-143">Response</span></span>
<span data-ttu-id="903f9-144">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="903f9-144">The following is an example of a response.</span></span>

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
  "description": "synchronizationJob: restart",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
