---
title: 'Rufen Sie: UpdateMetadata'
description: Aktualisieren Sie den Beginn des Debuggings Metadaten zu einem Anruf.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 2b736c56a7a517f0b68d656ab96933a34cf4a09d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813587"
---
# <a name="call-updatemetadata"></a><span data-ttu-id="bfc75-103">Rufen Sie: UpdateMetadata</span><span class="sxs-lookup"><span data-stu-id="bfc75-103">call: updateMetadata</span></span>

> <span data-ttu-id="bfc75-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bfc75-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bfc75-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bfc75-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bfc75-106">Aktualisieren Sie den Beginn des Debuggings Metadaten zu einem Anruf.</span><span class="sxs-lookup"><span data-stu-id="bfc75-106">Update the appliation's metadata associated with a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="bfc75-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bfc75-107">Permissions</span></span>
<span data-ttu-id="bfc75-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfc75-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bfc75-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bfc75-110">Permission type</span></span>                        | <span data-ttu-id="bfc75-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bfc75-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bfc75-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bfc75-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="bfc75-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bfc75-113">Not Supported</span></span>                               |
| <span data-ttu-id="bfc75-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bfc75-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfc75-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bfc75-115">Not Supported</span></span>                               |
| <span data-ttu-id="bfc75-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bfc75-116">Application</span></span>     | <span data-ttu-id="bfc75-117">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="bfc75-117">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfc75-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bfc75-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateMetadata
POST /applications/{id}/calls/{id}/updateMetadata
```

## <a name="request-headers"></a><span data-ttu-id="bfc75-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bfc75-119">Request headers</span></span>
| <span data-ttu-id="bfc75-120">Name</span><span class="sxs-lookup"><span data-stu-id="bfc75-120">Name</span></span>          | <span data-ttu-id="bfc75-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bfc75-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="bfc75-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfc75-122">Authorization</span></span> | <span data-ttu-id="bfc75-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bfc75-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bfc75-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bfc75-125">Request body</span></span>
<span data-ttu-id="bfc75-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="bfc75-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bfc75-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="bfc75-127">Parameter</span></span>      | <span data-ttu-id="bfc75-128">Typ</span><span class="sxs-lookup"><span data-stu-id="bfc75-128">Type</span></span>    |<span data-ttu-id="bfc75-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bfc75-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bfc75-130">metadata</span><span class="sxs-lookup"><span data-stu-id="bfc75-130">metadata</span></span>|<span data-ttu-id="bfc75-131">String</span><span class="sxs-lookup"><span data-stu-id="bfc75-131">String</span></span>|<span data-ttu-id="bfc75-132">Ein Blob von Daten von den Teilnehmer in der Teilnehmerliste einer bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="bfc75-132">A blob of data provided by the participant in the roster.</span></span>|
|<span data-ttu-id="bfc75-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="bfc75-133">clientContext</span></span>|<span data-ttu-id="bfc75-134">String</span><span class="sxs-lookup"><span data-stu-id="bfc75-134">String</span></span>|<span data-ttu-id="bfc75-135">Der Clientkontext.</span><span class="sxs-lookup"><span data-stu-id="bfc75-135">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="bfc75-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="bfc75-136">Response</span></span>
<span data-ttu-id="bfc75-137">Gibt `202 Accepted` Antwortcode und ein Location-Header mit einem Uri, um die [CommsOperation](../resources/commsoperation.md) für diese Anforderung erstellt.</span><span class="sxs-lookup"><span data-stu-id="bfc75-137">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="bfc75-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bfc75-138">Example</span></span>
<span data-ttu-id="bfc75-139">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="bfc75-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="bfc75-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bfc75-140">Request</span></span>
<span data-ttu-id="bfc75-141">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="bfc75-141">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-updateMetadata"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/updateMetadata
Content-Type: application/json
Content-Length: 79

{
  "metadata": "metadata-value",
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="bfc75-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="bfc75-142">Response</span></span>

> <span data-ttu-id="bfc75-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="bfc75-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: updateMetadata",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
