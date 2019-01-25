---
title: 'Rufen Sie: UpdateMetadata'
description: Aktualisieren Sie den Beginn des Debuggings Metadaten zu einem Anruf.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b3dade26dde72acd796cc3751df136fde4a4bbea
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507985"
---
# <a name="call-updatemetadata"></a><span data-ttu-id="f81cb-103">Rufen Sie: UpdateMetadata</span><span class="sxs-lookup"><span data-stu-id="f81cb-103">call: updateMetadata</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f81cb-104">Aktualisieren Sie den Beginn des Debuggings Metadaten zu einem Anruf.</span><span class="sxs-lookup"><span data-stu-id="f81cb-104">Update the appliation's metadata associated with a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="f81cb-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f81cb-105">Permissions</span></span>
<span data-ttu-id="f81cb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f81cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f81cb-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f81cb-108">Permission type</span></span>                        | <span data-ttu-id="f81cb-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f81cb-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f81cb-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f81cb-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f81cb-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f81cb-111">Not Supported</span></span>                               |
| <span data-ttu-id="f81cb-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f81cb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f81cb-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f81cb-113">Not Supported</span></span>                               |
| <span data-ttu-id="f81cb-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f81cb-114">Application</span></span>     | <span data-ttu-id="f81cb-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="f81cb-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f81cb-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f81cb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateMetadata
POST /applications/{id}/calls/{id}/updateMetadata
```

## <a name="request-headers"></a><span data-ttu-id="f81cb-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f81cb-117">Request headers</span></span>
| <span data-ttu-id="f81cb-118">Name</span><span class="sxs-lookup"><span data-stu-id="f81cb-118">Name</span></span>          | <span data-ttu-id="f81cb-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f81cb-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f81cb-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f81cb-120">Authorization</span></span> | <span data-ttu-id="f81cb-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f81cb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f81cb-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f81cb-123">Request body</span></span>
<span data-ttu-id="f81cb-124">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="f81cb-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f81cb-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="f81cb-125">Parameter</span></span>      | <span data-ttu-id="f81cb-126">Typ</span><span class="sxs-lookup"><span data-stu-id="f81cb-126">Type</span></span>    |<span data-ttu-id="f81cb-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f81cb-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f81cb-128">metadata</span><span class="sxs-lookup"><span data-stu-id="f81cb-128">metadata</span></span>|<span data-ttu-id="f81cb-129">String</span><span class="sxs-lookup"><span data-stu-id="f81cb-129">String</span></span>|<span data-ttu-id="f81cb-130">Ein Blob von Daten von den Teilnehmer in der Teilnehmerliste einer bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="f81cb-130">A blob of data provided by the participant in the roster.</span></span>|
|<span data-ttu-id="f81cb-131">ClientContext</span><span class="sxs-lookup"><span data-stu-id="f81cb-131">clientContext</span></span>|<span data-ttu-id="f81cb-132">String</span><span class="sxs-lookup"><span data-stu-id="f81cb-132">String</span></span>|<span data-ttu-id="f81cb-133">Der Clientkontext.</span><span class="sxs-lookup"><span data-stu-id="f81cb-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="f81cb-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f81cb-134">Response</span></span>
<span data-ttu-id="f81cb-135">Gibt `202 Accepted` Antwortcode und ein Location-Header mit einem Uri, um die [CommsOperation](../resources/commsoperation.md) für diese Anforderung erstellt.</span><span class="sxs-lookup"><span data-stu-id="f81cb-135">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="f81cb-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f81cb-136">Example</span></span>
<span data-ttu-id="f81cb-137">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="f81cb-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="f81cb-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f81cb-138">Request</span></span>
<span data-ttu-id="f81cb-139">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="f81cb-139">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="f81cb-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="f81cb-140">Response</span></span>

> <span data-ttu-id="f81cb-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="f81cb-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "call: updateMetadata",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-updatemetadata.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
