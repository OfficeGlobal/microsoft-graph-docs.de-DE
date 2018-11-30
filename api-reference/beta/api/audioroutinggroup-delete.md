---
title: Audio Routinggruppe löschen
description: Löschen der angegebenen AudioRoutingGroup.
ms.openlocfilehash: 2683c31f2df4f6913019f6a5f8c58cb009684043
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060624"
---
# <a name="delete-audio-routing-group"></a><span data-ttu-id="60875-103">Audio Routinggruppe löschen</span><span class="sxs-lookup"><span data-stu-id="60875-103">Delete audio routing group</span></span>

> <span data-ttu-id="60875-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="60875-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60875-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="60875-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="60875-106">Löschen der angegebenen [AudioRoutingGroup](../resources/audioroutinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="60875-106">Delete the specified [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="60875-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="60875-107">Permissions</span></span>
<span data-ttu-id="60875-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60875-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="60875-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="60875-110">Permission type</span></span> | <span data-ttu-id="60875-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="60875-111">Permissions (from least to most privileged)</span></span>  |
| :-------------- | :------------------------------------------- |
| <span data-ttu-id="60875-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="60875-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="60875-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="60875-113">Not Supported</span></span>        |
| <span data-ttu-id="60875-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="60875-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60875-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="60875-115">Not Supported</span></span>        |
| <span data-ttu-id="60875-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="60875-116">Application</span></span>     | <span data-ttu-id="60875-117">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="60875-117">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="60875-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="60875-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/audioRoutingGroups/{id}
DELETE /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="60875-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="60875-119">Request headers</span></span>
| <span data-ttu-id="60875-120">Name</span><span class="sxs-lookup"><span data-stu-id="60875-120">Name</span></span>          | <span data-ttu-id="60875-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="60875-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="60875-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="60875-122">Authorization</span></span> | <span data-ttu-id="60875-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="60875-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60875-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="60875-125">Request body</span></span>
<span data-ttu-id="60875-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="60875-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60875-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="60875-127">Response</span></span>
<span data-ttu-id="60875-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="60875-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60875-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="60875-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="60875-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="60875-131">Request</span></span>
<span data-ttu-id="60875-132">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="60875-132">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_audioRoutingGroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="60875-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="60875-133">Response</span></span>

> <span data-ttu-id="60875-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="60875-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Delete audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
