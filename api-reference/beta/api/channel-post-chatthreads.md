---
title: Chat Thread erstellen
description: Erstellen Sie einen neuen Chat Thread in den angegebenen DDE-Kanal, durch die Stamm-Nachrichten bereitstellen.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: d748826b98336feffcded345f356663f8fb80f4f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946357"
---
# <a name="create-chat-thread"></a><span data-ttu-id="dcc56-103">Chat Thread erstellen</span><span class="sxs-lookup"><span data-stu-id="dcc56-103">Create chat thread</span></span>

> <span data-ttu-id="dcc56-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dcc56-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dcc56-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dcc56-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dcc56-106">Erstellen Sie einen neuen Chat Thread in den angegebenen [DDE-Kanal](../resources/channel.md) , durch die Stamm-Nachrichten bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="dcc56-106">Create a new chat thread in the specified [channel](../resources/channel.md) by supplying the root messages.</span></span>

## <a name="permissions"></a><span data-ttu-id="dcc56-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="dcc56-107">Permissions</span></span>
<span data-ttu-id="dcc56-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcc56-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcc56-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dcc56-110">Permission type</span></span>      | <span data-ttu-id="dcc56-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dcc56-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dcc56-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dcc56-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dcc56-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcc56-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dcc56-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dcc56-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcc56-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dcc56-115">Not supported.</span></span>    |
|<span data-ttu-id="dcc56-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dcc56-116">Application</span></span> | <span data-ttu-id="dcc56-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dcc56-117">Not supported.</span></span> |

> <span data-ttu-id="dcc56-118">Nur die [Berechtigungen delegiert](/graph/permissions-reference) werden gegenwärtig unterstützt für diesen Vorgang.</span><span class="sxs-lookup"><span data-stu-id="dcc56-118">Currently, only [delegated permissions](/graph/permissions-reference) are supported for this operation.</span></span>  <span data-ttu-id="dcc56-119">Zukünftige Versionen werden Anwendungsberechtigungen unterstützen.</span><span class="sxs-lookup"><span data-stu-id="dcc56-119">Future releases will support application permissions.</span></span> 

## <a name="http-request"></a><span data-ttu-id="dcc56-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dcc56-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/chatThreads
```
## <a name="request-headers"></a><span data-ttu-id="dcc56-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dcc56-121">Request headers</span></span>
| <span data-ttu-id="dcc56-122">Name</span><span class="sxs-lookup"><span data-stu-id="dcc56-122">Name</span></span>       | <span data-ttu-id="dcc56-123">Typ</span><span class="sxs-lookup"><span data-stu-id="dcc56-123">Type</span></span> | <span data-ttu-id="dcc56-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dcc56-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dcc56-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="dcc56-125">Authorization</span></span>  | <span data-ttu-id="dcc56-126">string</span><span class="sxs-lookup"><span data-stu-id="dcc56-126">string</span></span>  | <span data-ttu-id="dcc56-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dcc56-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dcc56-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dcc56-129">Request body</span></span>
<span data-ttu-id="dcc56-130">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der ein [ChatThread](../resources/chatthread.md) -Objekt, das die RootMessage-Eigenschaft enthält.</span><span class="sxs-lookup"><span data-stu-id="dcc56-130">In the request body, supply a JSON representation of a [chatThread](../resources/chatthread.md) object that contains the rootMessage property.</span></span>

## <a name="response"></a><span data-ttu-id="dcc56-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="dcc56-131">Response</span></span>

<span data-ttu-id="dcc56-132">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortcode mit einem leeren Antwort Meldungstext.</span><span class="sxs-lookup"><span data-stu-id="dcc56-132">If successful, this method returns `201 Created` response code with an empty reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="dcc56-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dcc56-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dcc56-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dcc56-134">Request</span></span>
<span data-ttu-id="dcc56-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dcc56-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chatthread_from_channel"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/chatThreads
Content-type: application/json

{
  "rootMessage": {
      "body": {
        "contentType": 1,
        "content": "<h1>Hello world</h1>"
      }
  }
}
```

> <span data-ttu-id="dcc56-136">Derzeit ContentType muss eine ganze Zahl, sondern als eine Zeichenfolge angegeben werden: 0 für "Text" oder "html" 1.</span><span class="sxs-lookup"><span data-stu-id="dcc56-136">Currently, the contentType must be specified as an integer rather than a string: 0 for "text" or 1 for "html".</span></span>  <span data-ttu-id="dcc56-137">Zukünftige Versionen der API werden dieses Problem zu beheben.</span><span class="sxs-lookup"><span data-stu-id="dcc56-137">Future API releases will fix this.</span></span>

##### <a name="response"></a><span data-ttu-id="dcc56-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="dcc56-138">Response</span></span>

<span data-ttu-id="dcc56-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="dcc56-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatThread"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
