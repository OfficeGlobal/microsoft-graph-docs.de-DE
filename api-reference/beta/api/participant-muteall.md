---
title: 'Teilnehmer: MuteAll'
description: Stummschalten Sie aller Teilnehmer in den Anruf.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2a74a224141b77f0a09718bbafee3cf1dab0e8e9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522833"
---
# <a name="participant-muteall"></a><span data-ttu-id="2266b-103">Teilnehmer: MuteAll</span><span class="sxs-lookup"><span data-stu-id="2266b-103">participant: muteAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2266b-104">Stummschalten Sie aller Teilnehmer in den Anruf.</span><span class="sxs-lookup"><span data-stu-id="2266b-104">Mute all participants in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="2266b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2266b-105">Permissions</span></span>
<span data-ttu-id="2266b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2266b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2266b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2266b-108">Permission type</span></span>                        | <span data-ttu-id="2266b-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2266b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2266b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2266b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2266b-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2266b-111">Not Supported</span></span>                               |
| <span data-ttu-id="2266b-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2266b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2266b-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2266b-113">Not Supported</span></span>                               |
| <span data-ttu-id="2266b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2266b-114">Application</span></span>                            | <span data-ttu-id="2266b-115">Keine</span><span class="sxs-lookup"><span data-stu-id="2266b-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="2266b-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2266b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/muteAll
POST /applications/{id}/calls/{id}/participants/muteAll
```

## <a name="request-headers"></a><span data-ttu-id="2266b-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2266b-117">Request headers</span></span>
| <span data-ttu-id="2266b-118">Name</span><span class="sxs-lookup"><span data-stu-id="2266b-118">Name</span></span>          | <span data-ttu-id="2266b-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2266b-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="2266b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2266b-120">Authorization</span></span> | <span data-ttu-id="2266b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2266b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2266b-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2266b-123">Request body</span></span>
<span data-ttu-id="2266b-124">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="2266b-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2266b-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="2266b-125">Parameter</span></span>      | <span data-ttu-id="2266b-126">Typ</span><span class="sxs-lookup"><span data-stu-id="2266b-126">Type</span></span>    |<span data-ttu-id="2266b-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2266b-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2266b-128">participants</span><span class="sxs-lookup"><span data-stu-id="2266b-128">participants</span></span>|<span data-ttu-id="2266b-129">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="2266b-129">String collection</span></span>|<span data-ttu-id="2266b-130">Die Teilnehmer stummgeschaltet werden.</span><span class="sxs-lookup"><span data-stu-id="2266b-130">The participants to be muted.</span></span>|
|<span data-ttu-id="2266b-131">ClientContext</span><span class="sxs-lookup"><span data-stu-id="2266b-131">clientContext</span></span>|<span data-ttu-id="2266b-132">String</span><span class="sxs-lookup"><span data-stu-id="2266b-132">String</span></span>|<span data-ttu-id="2266b-133">Der Clientkontext.</span><span class="sxs-lookup"><span data-stu-id="2266b-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="2266b-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="2266b-134">Response</span></span>
<span data-ttu-id="2266b-135">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortobjekt Code und [CommsOperation](../resources/commsoperation.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="2266b-135">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2266b-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2266b-136">Example</span></span>
<span data-ttu-id="2266b-137">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="2266b-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="2266b-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2266b-138">Request</span></span>
<span data-ttu-id="2266b-139">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="2266b-139">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "participant-muteAll"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/participants/muteAll
Content-Type: application/json
Content-Length: 81

{
  "participants": [
    ""
  ],
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="2266b-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="2266b-140">Response</span></span>

> <span data-ttu-id="2266b-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="2266b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "participant: muteAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/participant-muteall.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
