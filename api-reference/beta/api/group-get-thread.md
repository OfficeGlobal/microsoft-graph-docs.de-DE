---
title: Unterhaltungsthread abrufen
description: Abrufen eines thread-Objekts.
author: dkershaw10
ms.openlocfilehash: 615a606bbe0e58da233642c55baccb3f05dc3dd6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347726"
---
# <a name="get-conversation-thread"></a><span data-ttu-id="f9183-103">Unterhaltungsthread abrufen</span><span class="sxs-lookup"><span data-stu-id="f9183-103">Get conversation thread</span></span>

> <span data-ttu-id="f9183-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f9183-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9183-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f9183-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f9183-106">Abrufen eines [thread](../resources/conversationthread.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f9183-106">Get a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9183-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f9183-107">Permissions</span></span>
<span data-ttu-id="f9183-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9183-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9183-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f9183-110">Permission type</span></span>      | <span data-ttu-id="f9183-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f9183-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9183-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f9183-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f9183-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9183-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f9183-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f9183-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9183-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f9183-115">Not supported.</span></span>    |
|<span data-ttu-id="f9183-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f9183-116">Application</span></span> | <span data-ttu-id="f9183-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f9183-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9183-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f9183-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f9183-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f9183-119">Optional query parameters</span></span>
<span data-ttu-id="f9183-120">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f9183-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f9183-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f9183-121">Request headers</span></span>
| <span data-ttu-id="f9183-122">Header</span><span class="sxs-lookup"><span data-stu-id="f9183-122">Header</span></span>       | <span data-ttu-id="f9183-123">Wert</span><span class="sxs-lookup"><span data-stu-id="f9183-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f9183-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9183-124">Authorization</span></span>  | <span data-ttu-id="f9183-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f9183-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f9183-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f9183-127">Request body</span></span>
<span data-ttu-id="f9183-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f9183-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9183-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f9183-129">Response</span></span>
<span data-ttu-id="f9183-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [thread](../resources/conversationthread.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f9183-130">If successful, this method returns a `200 OK` response code and a [thread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9183-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f9183-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f9183-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f9183-132">Request</span></span>
<span data-ttu-id="f9183-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f9183-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_thread"
}-->
```http
GET https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```

#### <a name="response"></a><span data-ttu-id="f9183-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f9183-134">Response</span></span>
<span data-ttu-id="f9183-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f9183-135">The following is an example of the response.</span></span>
><span data-ttu-id="f9183-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="f9183-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
