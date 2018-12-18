---
title: Unterhaltungsthread abrufen
description: Abrufen eines thread-Objekts.
author: dkershaw10
ms.openlocfilehash: ecfb1443c1210271d2fbce330a8237a57bdd07d2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326999"
---
# <a name="get-conversation-thread"></a><span data-ttu-id="97788-103">Unterhaltungsthread abrufen</span><span class="sxs-lookup"><span data-stu-id="97788-103">Get conversation thread</span></span>
<span data-ttu-id="97788-104">Abrufen eines [thread](../resources/conversationthread.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="97788-104">Get a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="97788-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="97788-105">Permissions</span></span>
<span data-ttu-id="97788-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97788-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97788-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="97788-108">Permission type</span></span>      | <span data-ttu-id="97788-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="97788-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97788-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="97788-110">Delegated (work or school account)</span></span> | <span data-ttu-id="97788-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97788-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="97788-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="97788-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97788-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97788-113">Not supported.</span></span>    |
|<span data-ttu-id="97788-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="97788-114">Application</span></span> | <span data-ttu-id="97788-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97788-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="97788-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="97788-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="97788-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="97788-117">Optional query parameters</span></span>
<span data-ttu-id="97788-118">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="97788-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="97788-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="97788-119">Request headers</span></span>
| <span data-ttu-id="97788-120">Header</span><span class="sxs-lookup"><span data-stu-id="97788-120">Header</span></span>       | <span data-ttu-id="97788-121">Wert</span><span class="sxs-lookup"><span data-stu-id="97788-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="97788-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="97788-122">Authorization</span></span>  | <span data-ttu-id="97788-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="97788-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="97788-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="97788-125">Request body</span></span>
<span data-ttu-id="97788-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="97788-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97788-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="97788-127">Response</span></span>
<span data-ttu-id="97788-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [thread](../resources/conversationthread.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="97788-128">If successful, this method returns a `200 OK` response code and a [thread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97788-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="97788-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="97788-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="97788-130">Request</span></span>
<span data-ttu-id="97788-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="97788-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q=="],
  "name": "get_group_thread"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```

#### <a name="response"></a><span data-ttu-id="97788-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="97788-132">Response</span></span>
<span data-ttu-id="97788-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="97788-133">The following is an example of the response.</span></span>
><span data-ttu-id="97788-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="97788-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
