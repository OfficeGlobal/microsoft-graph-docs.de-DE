---
title: Chatthread erstellen
description: Erstellen Sie einen neuen Chatthread im angegebenen Kanal, indem Sie die Stammnachrichten bereitstellen.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: ef8d341310296c810c433a23f0d29be166ca47c5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511247"
---
# <a name="create-chat-thread"></a><span data-ttu-id="c05cb-103">Chatthread erstellen</span><span class="sxs-lookup"><span data-stu-id="c05cb-103">Create chat thread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c05cb-104">Erstellen Sie einen neuen Chatthread im angegebenen [Kanal](../resources/channel.md), indem Sie die Stammnachrichten bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="c05cb-104">Create a new chat thread in the specified [channel](../resources/channel.md) by supplying the root messages.</span></span>

## <a name="permissions"></a><span data-ttu-id="c05cb-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c05cb-105">Permissions</span></span>
<span data-ttu-id="c05cb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c05cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c05cb-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c05cb-108">Permission type</span></span>      | <span data-ttu-id="c05cb-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c05cb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c05cb-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c05cb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c05cb-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c05cb-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c05cb-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c05cb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c05cb-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c05cb-113">Not supported.</span></span>    |
|<span data-ttu-id="c05cb-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c05cb-114">Application</span></span> | <span data-ttu-id="c05cb-115">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c05cb-115">Not supported.</span></span> |

> <span data-ttu-id="c05cb-116">Derzeit werden nur [delegierte Berechtigungen](/graph/permissions-reference) für diesen Vorgang unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c05cb-116">Currently, only [delegated permissions](/graph/permissions-reference) are supported for this operation.</span></span>  <span data-ttu-id="c05cb-117">In künftigen Versionen werden Anwendungsberechtigungen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c05cb-117">Future releases will support application permissions.</span></span> 

## <a name="http-request"></a><span data-ttu-id="c05cb-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c05cb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/chatThreads
```
## <a name="request-headers"></a><span data-ttu-id="c05cb-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c05cb-119">Request headers</span></span>
| <span data-ttu-id="c05cb-120">Name</span><span class="sxs-lookup"><span data-stu-id="c05cb-120">Name</span></span>       | <span data-ttu-id="c05cb-121">Typ</span><span class="sxs-lookup"><span data-stu-id="c05cb-121">Type</span></span> | <span data-ttu-id="c05cb-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c05cb-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c05cb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c05cb-123">Authorization</span></span>  | <span data-ttu-id="c05cb-124">string</span><span class="sxs-lookup"><span data-stu-id="c05cb-124">string</span></span>  | <span data-ttu-id="c05cb-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c05cb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c05cb-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c05cb-127">Request body</span></span>
<span data-ttu-id="c05cb-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [chatThread](../resources/chatthread.md)-Objekts an, das die rootMessage-Eigenschaft enthält.</span><span class="sxs-lookup"><span data-stu-id="c05cb-128">In the request body, supply a JSON representation of a [chatThread](../resources/chatthread.md) object that contains the rootMessage property.</span></span>

## <a name="response"></a><span data-ttu-id="c05cb-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="c05cb-129">Response</span></span>

<span data-ttu-id="c05cb-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` mit einem leeren Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c05cb-130">If successful, this method returns a `201 Created` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="c05cb-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c05cb-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c05cb-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c05cb-132">Request</span></span>
<span data-ttu-id="c05cb-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c05cb-133">Here is an example of the request.</span></span>
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

> <span data-ttu-id="c05cb-134">Derzeit muss der contentType als ganze Zahl und nicht als Zeichenfolge angegeben werden: 0 für „text“ oder 1 für „html“.</span><span class="sxs-lookup"><span data-stu-id="c05cb-134">Currently, the contentType must be specified as an integer rather than a string: 0 for "text" or 1 for "html".</span></span>  <span data-ttu-id="c05cb-135">In künftigen API-Versionen wird dies korrigiert.</span><span class="sxs-lookup"><span data-stu-id="c05cb-135">Future API releases will fix this.</span></span>

##### <a name="response"></a><span data-ttu-id="c05cb-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="c05cb-136">Response</span></span>

<span data-ttu-id="c05cb-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c05cb-137">Here is an example of the response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-post-chatthreads.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
