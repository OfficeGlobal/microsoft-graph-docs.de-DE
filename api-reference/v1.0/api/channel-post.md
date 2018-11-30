---
title: Erstellen von DDE-Kanal
description: Erstellen Sie einen neuen Kanal in einem Microsoft-Team, wie im Textkörper Anforderung angegeben.
ms.openlocfilehash: 8cb6beed2758ac225bbef2b028abff68547b3eda
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017762"
---
# <a name="create-channel"></a><span data-ttu-id="c912d-103">Erstellen von DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="c912d-103">Create Channel</span></span>



<span data-ttu-id="c912d-104">Erstellen Sie einen neuen [Channel](../resources/channel.md) in einem Microsoft-Team, wie im Textkörper Anforderung angegeben.</span><span class="sxs-lookup"><span data-stu-id="c912d-104">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

> <span data-ttu-id="c912d-105">**Hinweis**: Es ist ein bekanntes Problem mit Berechtigungen und diese API.</span><span class="sxs-lookup"><span data-stu-id="c912d-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="c912d-106">Weitere Informationen hierzu finden Sie unter der [Problemliste bezeichnet](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="c912d-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="c912d-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c912d-107">Permissions</span></span>
<span data-ttu-id="c912d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c912d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c912d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c912d-110">Permission type</span></span>      | <span data-ttu-id="c912d-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c912d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c912d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c912d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c912d-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c912d-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c912d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c912d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c912d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c912d-115">Not supported.</span></span>    |
|<span data-ttu-id="c912d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c912d-116">Application</span></span> | <span data-ttu-id="c912d-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c912d-117">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="c912d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c912d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```
## <a name="request-headers"></a><span data-ttu-id="c912d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c912d-119">Request headers</span></span>
| <span data-ttu-id="c912d-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c912d-120">Header</span></span>       | <span data-ttu-id="c912d-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c912d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c912d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c912d-122">Authorization</span></span>  | <span data-ttu-id="c912d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c912d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c912d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c912d-125">Content-Type</span></span>  | <span data-ttu-id="c912d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c912d-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c912d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c912d-127">Request body</span></span>
<span data-ttu-id="c912d-128">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Channel](../resources/channel.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c912d-128">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c912d-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="c912d-129">Response</span></span>

<span data-ttu-id="c912d-130">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Code und [Channel](../resources/channel.md) -Antwortobjekt im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="c912d-130">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c912d-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c912d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c912d-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c912d-132">Request</span></span>
<span data-ttu-id="c912d-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c912d-133">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="c912d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c912d-134">Response</span></span>
<span data-ttu-id="c912d-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c912d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
