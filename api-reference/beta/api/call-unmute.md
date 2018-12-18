---
title: 'Rufen Sie: stummschaltung aufheben'
description: Ermöglicht die Anwendung selbst stummschaltung aufheben.
author: VinodRavichandran
ms.openlocfilehash: 7ac86b12363e692930597e3394ca0f78b30b0dee
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343470"
---
# <a name="call-unmute"></a><span data-ttu-id="dd02c-103">Rufen Sie: stummschaltung aufheben</span><span class="sxs-lookup"><span data-stu-id="dd02c-103">call: unmute</span></span>

> <span data-ttu-id="dd02c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dd02c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd02c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dd02c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dd02c-106">Ermöglicht die Anwendung selbst stummschaltung aufheben.</span><span class="sxs-lookup"><span data-stu-id="dd02c-106">Allows the application to unmute itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd02c-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="dd02c-107">Permissions</span></span>
<span data-ttu-id="dd02c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd02c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dd02c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dd02c-110">Permission type</span></span>                        | <span data-ttu-id="dd02c-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dd02c-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dd02c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dd02c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="dd02c-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd02c-113">Not supported.</span></span>                               |
| <span data-ttu-id="dd02c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dd02c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd02c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd02c-115">Not supported.</span></span>                               |
| <span data-ttu-id="dd02c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dd02c-116">Application</span></span>                            | <span data-ttu-id="dd02c-117">Keine.</span><span class="sxs-lookup"><span data-stu-id="dd02c-117">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="dd02c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd02c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/unmute
POST /applications/{id}/calls/{id}/unmute
```

## <a name="request-headers"></a><span data-ttu-id="dd02c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dd02c-119">Request headers</span></span>
| <span data-ttu-id="dd02c-120">Name</span><span class="sxs-lookup"><span data-stu-id="dd02c-120">Name</span></span>          | <span data-ttu-id="dd02c-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dd02c-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="dd02c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd02c-122">Authorization</span></span> | <span data-ttu-id="dd02c-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dd02c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd02c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dd02c-125">Request body</span></span>
<span data-ttu-id="dd02c-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="dd02c-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dd02c-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="dd02c-127">Parameter</span></span>      | <span data-ttu-id="dd02c-128">Typ</span><span class="sxs-lookup"><span data-stu-id="dd02c-128">Type</span></span>    |<span data-ttu-id="dd02c-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dd02c-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd02c-130">clientContext</span><span class="sxs-lookup"><span data-stu-id="dd02c-130">clientContext</span></span>|<span data-ttu-id="dd02c-131">String</span><span class="sxs-lookup"><span data-stu-id="dd02c-131">String</span></span>|<span data-ttu-id="dd02c-132">Der Clientkontext.</span><span class="sxs-lookup"><span data-stu-id="dd02c-132">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="dd02c-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd02c-133">Response</span></span>
<span data-ttu-id="dd02c-134">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortobjekt Code und [CommsOperation](../resources/commsoperation.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="dd02c-134">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd02c-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dd02c-135">Example</span></span>
<span data-ttu-id="dd02c-136">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="dd02c-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="dd02c-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd02c-137">Request</span></span>
<span data-ttu-id="dd02c-138">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="dd02c-138">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call_unmute"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/unmute
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="dd02c-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd02c-139">Response</span></span>

> <span data-ttu-id="dd02c-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="dd02c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "call: unmute",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
