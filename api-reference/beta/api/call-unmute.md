---
title: 'Rufen Sie: stummschaltung aufheben'
description: Ermöglicht die Anwendung selbst stummschaltung aufheben.
ms.openlocfilehash: de2029a2fa5abeb777f83e8651c8b6c5a2c15991
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061551"
---
# <a name="call-unmute"></a><span data-ttu-id="6e0d8-103">Rufen Sie: stummschaltung aufheben</span><span class="sxs-lookup"><span data-stu-id="6e0d8-103">call: unmute</span></span>

> <span data-ttu-id="6e0d8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6e0d8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e0d8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6e0d8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6e0d8-106">Ermöglicht die Anwendung selbst stummschaltung aufheben.</span><span class="sxs-lookup"><span data-stu-id="6e0d8-106">Allows the application to unmute itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e0d8-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6e0d8-107">Permissions</span></span>
<span data-ttu-id="6e0d8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e0d8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6e0d8-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6e0d8-110">Permission type</span></span>                        | <span data-ttu-id="6e0d8-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6e0d8-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6e0d8-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6e0d8-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6e0d8-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6e0d8-113">Not supported.</span></span>                               |
| <span data-ttu-id="6e0d8-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6e0d8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e0d8-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6e0d8-115">Not supported.</span></span>                               |
| <span data-ttu-id="6e0d8-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6e0d8-116">Application</span></span>                            | <span data-ttu-id="6e0d8-117">Keine.</span><span class="sxs-lookup"><span data-stu-id="6e0d8-117">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="6e0d8-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6e0d8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/unmute
POST /applications/{id}/calls/{id}/unmute
```

## <a name="request-headers"></a><span data-ttu-id="6e0d8-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6e0d8-119">Request headers</span></span>
| <span data-ttu-id="6e0d8-120">Name</span><span class="sxs-lookup"><span data-stu-id="6e0d8-120">Name</span></span>          | <span data-ttu-id="6e0d8-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6e0d8-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="6e0d8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e0d8-122">Authorization</span></span> | <span data-ttu-id="6e0d8-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6e0d8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e0d8-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6e0d8-125">Request body</span></span>
<span data-ttu-id="6e0d8-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="6e0d8-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6e0d8-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="6e0d8-127">Parameter</span></span>      | <span data-ttu-id="6e0d8-128">Typ</span><span class="sxs-lookup"><span data-stu-id="6e0d8-128">Type</span></span>    |<span data-ttu-id="6e0d8-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6e0d8-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e0d8-130">clientContext</span><span class="sxs-lookup"><span data-stu-id="6e0d8-130">clientContext</span></span>|<span data-ttu-id="6e0d8-131">String</span><span class="sxs-lookup"><span data-stu-id="6e0d8-131">String</span></span>|<span data-ttu-id="6e0d8-132">Der Clientkontext.</span><span class="sxs-lookup"><span data-stu-id="6e0d8-132">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="6e0d8-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="6e0d8-133">Response</span></span>
<span data-ttu-id="6e0d8-134">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortobjekt Code und [CommsOperation](../resources/commsoperation.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="6e0d8-134">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e0d8-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6e0d8-135">Example</span></span>
<span data-ttu-id="6e0d8-136">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="6e0d8-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="6e0d8-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6e0d8-137">Request</span></span>
<span data-ttu-id="6e0d8-138">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="6e0d8-138">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="6e0d8-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="6e0d8-139">Response</span></span>

> <span data-ttu-id="6e0d8-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="6e0d8-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
