---
title: Unterhaltungsthread abrufen
description: Abrufen eines thread-Objekts.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 2df12f484bbbc35d4f5d5bc3fcbce1d6e5e8b653
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966475"
---
# <a name="get-conversation-thread"></a><span data-ttu-id="a483c-103">Unterhaltungsthread abrufen</span><span class="sxs-lookup"><span data-stu-id="a483c-103">Get conversation thread</span></span>

> <span data-ttu-id="a483c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a483c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a483c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a483c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a483c-106">Abrufen eines [thread](../resources/conversationthread.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a483c-106">Get a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a483c-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a483c-107">Permissions</span></span>
<span data-ttu-id="a483c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a483c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a483c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a483c-110">Permission type</span></span>      | <span data-ttu-id="a483c-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a483c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a483c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a483c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a483c-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a483c-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a483c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a483c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a483c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a483c-115">Not supported.</span></span>    |
|<span data-ttu-id="a483c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a483c-116">Application</span></span> | <span data-ttu-id="a483c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a483c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a483c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a483c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a483c-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a483c-119">Optional query parameters</span></span>
<span data-ttu-id="a483c-120">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a483c-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a483c-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a483c-121">Request headers</span></span>
| <span data-ttu-id="a483c-122">Header</span><span class="sxs-lookup"><span data-stu-id="a483c-122">Header</span></span>       | <span data-ttu-id="a483c-123">Wert</span><span class="sxs-lookup"><span data-stu-id="a483c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a483c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a483c-124">Authorization</span></span>  | <span data-ttu-id="a483c-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a483c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a483c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a483c-127">Request body</span></span>
<span data-ttu-id="a483c-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a483c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a483c-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="a483c-129">Response</span></span>
<span data-ttu-id="a483c-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [thread](../resources/conversationthread.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a483c-130">If successful, this method returns a `200 OK` response code and a [thread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a483c-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a483c-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a483c-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a483c-132">Request</span></span>
<span data-ttu-id="a483c-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a483c-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_thread"
}-->
```http
GET https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```

#### <a name="response"></a><span data-ttu-id="a483c-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="a483c-134">Response</span></span>
<span data-ttu-id="a483c-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a483c-135">The following is an example of the response.</span></span>
><span data-ttu-id="a483c-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="a483c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 655

{
    "id": "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==",
    "topic": "New Training Plans",
    "hasAttachments": false,
    "lastDeliveredDateTime": "2017-07-31T18:59:05Z",
    "uniqueSenders": [
        "HR Taskforce"
    ],
    "preview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
    "isLocked": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
