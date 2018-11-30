---
title: Erstellen von DDE-Kanal
description: Erstellen Sie einen neuen Kanal in einem Microsoft-Team, wie im Textkörper Anforderung angegeben.
ms.openlocfilehash: f9767c70c94ce4cfe3379310c425005ace8fbe1a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060612"
---
# <a name="create-channel"></a><span data-ttu-id="06cfe-103">Erstellen von DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="06cfe-103">Create Channel</span></span>

> <span data-ttu-id="06cfe-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="06cfe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06cfe-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="06cfe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="06cfe-106">Erstellen Sie einen neuen [Channel](../resources/channel.md) in einem Microsoft-Team, wie im Textkörper Anforderung angegeben.</span><span class="sxs-lookup"><span data-stu-id="06cfe-106">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

> <span data-ttu-id="06cfe-107">**Hinweis**: Es ist ein bekanntes Problem mit Berechtigungen und diese API.</span><span class="sxs-lookup"><span data-stu-id="06cfe-107">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="06cfe-108">Weitere Informationen hierzu finden Sie unter der [Problemliste bezeichnet](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="06cfe-108">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="06cfe-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="06cfe-109">Permissions</span></span>
<span data-ttu-id="06cfe-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06cfe-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="06cfe-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="06cfe-112">Permission type</span></span>      | <span data-ttu-id="06cfe-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="06cfe-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06cfe-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="06cfe-114">Delegated (work or school account)</span></span> | <span data-ttu-id="06cfe-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06cfe-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="06cfe-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="06cfe-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06cfe-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="06cfe-117">Not supported.</span></span>    |
|<span data-ttu-id="06cfe-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="06cfe-118">Application</span></span> | <span data-ttu-id="06cfe-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06cfe-119">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="06cfe-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="06cfe-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```
## <a name="request-headers"></a><span data-ttu-id="06cfe-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="06cfe-121">Request headers</span></span>
| <span data-ttu-id="06cfe-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="06cfe-122">Header</span></span>       | <span data-ttu-id="06cfe-123">Wert</span><span class="sxs-lookup"><span data-stu-id="06cfe-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="06cfe-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="06cfe-124">Authorization</span></span>  | <span data-ttu-id="06cfe-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="06cfe-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="06cfe-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="06cfe-127">Content-Type</span></span>  | <span data-ttu-id="06cfe-128">application/json</span><span class="sxs-lookup"><span data-stu-id="06cfe-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="06cfe-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="06cfe-129">Request body</span></span>
<span data-ttu-id="06cfe-130">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Channel](../resources/channel.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="06cfe-130">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="06cfe-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="06cfe-131">Response</span></span>

<span data-ttu-id="06cfe-132">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Code und [Channel](../resources/channel.md) -Antwortobjekt im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="06cfe-132">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06cfe-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="06cfe-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="06cfe-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="06cfe-134">Request</span></span>
<span data-ttu-id="06cfe-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="06cfe-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_channel_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels
Content-type: application/json

{
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```
##### <a name="response"></a><span data-ttu-id="06cfe-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="06cfe-136">Response</span></span>
<span data-ttu-id="06cfe-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="06cfe-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
