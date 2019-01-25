---
title: 'Rufen Sie: stumm schalten'
description: Ermöglicht der Anwendung selbst stumm geschaltet werden sollen.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2f619cdc42ff914999ad8826ff31452ff82ea6a1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524079"
---
# <a name="call-mute"></a><span data-ttu-id="fa83e-103">Rufen Sie: stumm schalten</span><span class="sxs-lookup"><span data-stu-id="fa83e-103">call: mute</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa83e-104">Ermöglicht der Anwendung selbst stumm geschaltet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="fa83e-104">Allows the application to mute itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa83e-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fa83e-105">Permissions</span></span>
<span data-ttu-id="fa83e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa83e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fa83e-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fa83e-108">Permission type</span></span>                        | <span data-ttu-id="fa83e-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fa83e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fa83e-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fa83e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fa83e-111">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fa83e-111">Not Supported.</span></span>                               |
| <span data-ttu-id="fa83e-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fa83e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa83e-113">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fa83e-113">Not Supported.</span></span>                               |
| <span data-ttu-id="fa83e-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fa83e-114">Application</span></span>                            | <span data-ttu-id="fa83e-115">Keine.</span><span class="sxs-lookup"><span data-stu-id="fa83e-115">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="fa83e-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa83e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/mute
POST /applications/{id}/calls/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="fa83e-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fa83e-117">Request headers</span></span>
| <span data-ttu-id="fa83e-118">Name</span><span class="sxs-lookup"><span data-stu-id="fa83e-118">Name</span></span>          | <span data-ttu-id="fa83e-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa83e-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="fa83e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa83e-120">Authorization</span></span> | <span data-ttu-id="fa83e-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fa83e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa83e-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fa83e-123">Request body</span></span>
<span data-ttu-id="fa83e-124">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="fa83e-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fa83e-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="fa83e-125">Parameter</span></span>      | <span data-ttu-id="fa83e-126">Typ</span><span class="sxs-lookup"><span data-stu-id="fa83e-126">Type</span></span>    |<span data-ttu-id="fa83e-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa83e-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa83e-128">ClientContext</span><span class="sxs-lookup"><span data-stu-id="fa83e-128">clientContext</span></span>|<span data-ttu-id="fa83e-129">String</span><span class="sxs-lookup"><span data-stu-id="fa83e-129">String</span></span>|<span data-ttu-id="fa83e-130">Der Clientkontext.</span><span class="sxs-lookup"><span data-stu-id="fa83e-130">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="fa83e-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa83e-131">Response</span></span>
<span data-ttu-id="fa83e-132">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortcode und eines [CommsOperation](../resources/commsoperation.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="fa83e-132">If successful, this method returns `200 OK` response code and a [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa83e-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fa83e-133">Example</span></span>
<span data-ttu-id="fa83e-134">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="fa83e-134">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="fa83e-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa83e-135">Request</span></span>
<span data-ttu-id="fa83e-136">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="fa83e-136">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-mute"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/mute
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="fa83e-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa83e-137">Response</span></span>

> <span data-ttu-id="fa83e-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="fa83e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: mute",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-mute.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
