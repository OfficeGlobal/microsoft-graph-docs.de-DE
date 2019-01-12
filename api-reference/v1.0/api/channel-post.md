---
title: Erstellen von DDE-Kanal
description: Erstellen Sie einen neuen Kanal in einem Microsoft-Team, wie im Textkörper Anforderung angegeben.
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 09d058d9dc64fff053cd0ec507357f2990aeb353
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957340"
---
# <a name="create-channel"></a><span data-ttu-id="ec34b-103">Erstellen von DDE-Kanal</span><span class="sxs-lookup"><span data-stu-id="ec34b-103">Create Channel</span></span>



<span data-ttu-id="ec34b-104">Erstellen Sie einen neuen [Channel](../resources/channel.md) in einem Microsoft-Team, wie im Textkörper Anforderung angegeben.</span><span class="sxs-lookup"><span data-stu-id="ec34b-104">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

> <span data-ttu-id="ec34b-105">**Hinweis**: Es ist ein bekanntes Problem mit Berechtigungen und diese API.</span><span class="sxs-lookup"><span data-stu-id="ec34b-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="ec34b-106">Weitere Informationen hierzu finden Sie unter der [Problemliste bezeichnet](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="ec34b-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="ec34b-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ec34b-107">Permissions</span></span>
<span data-ttu-id="ec34b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec34b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ec34b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ec34b-110">Permission type</span></span>      | <span data-ttu-id="ec34b-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ec34b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec34b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ec34b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ec34b-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec34b-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ec34b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ec34b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec34b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ec34b-115">Not supported.</span></span>    |
|<span data-ttu-id="ec34b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ec34b-116">Application</span></span> | <span data-ttu-id="ec34b-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec34b-117">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="ec34b-118">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="ec34b-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ec34b-119">Globale Administratoren und Microsoft-Teams Dienstadministratoren können Teams zugreifen, denen sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="ec34b-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ec34b-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec34b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```
## <a name="request-headers"></a><span data-ttu-id="ec34b-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ec34b-121">Request headers</span></span>
| <span data-ttu-id="ec34b-122">Header</span><span class="sxs-lookup"><span data-stu-id="ec34b-122">Header</span></span>       | <span data-ttu-id="ec34b-123">Wert</span><span class="sxs-lookup"><span data-stu-id="ec34b-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ec34b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec34b-124">Authorization</span></span>  | <span data-ttu-id="ec34b-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ec34b-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ec34b-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ec34b-127">Content-Type</span></span>  | <span data-ttu-id="ec34b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ec34b-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ec34b-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ec34b-129">Request body</span></span>
<span data-ttu-id="ec34b-130">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Channel](../resources/channel.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ec34b-130">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ec34b-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec34b-131">Response</span></span>

<span data-ttu-id="ec34b-132">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Code und [Channel](../resources/channel.md) -Antwortobjekt im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ec34b-132">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec34b-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ec34b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec34b-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec34b-134">Request</span></span>
<span data-ttu-id="ec34b-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ec34b-135">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="ec34b-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec34b-136">Response</span></span>
<span data-ttu-id="ec34b-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ec34b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
