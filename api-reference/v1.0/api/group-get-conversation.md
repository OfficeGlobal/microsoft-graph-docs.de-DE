---
title: Unterhaltung abrufen
description: Abrufen eines conversation-Objekts.
author: dkershaw10
ms.openlocfilehash: 37a3f12c3d72be230e289a9f321b10910ab762be
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327041"
---
# <a name="get-conversation"></a><span data-ttu-id="b30cf-103">Unterhaltung abrufen</span><span class="sxs-lookup"><span data-stu-id="b30cf-103">Get conversation</span></span>
<span data-ttu-id="b30cf-104">Abrufen eines [conversation](../resources/conversation.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b30cf-104">Get a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b30cf-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b30cf-105">Permissions</span></span>
<span data-ttu-id="b30cf-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b30cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b30cf-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b30cf-108">Permission type</span></span>      | <span data-ttu-id="b30cf-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b30cf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b30cf-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b30cf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b30cf-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b30cf-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b30cf-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b30cf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b30cf-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b30cf-113">Not supported.</span></span>    |
|<span data-ttu-id="b30cf-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b30cf-114">Application</span></span> | <span data-ttu-id="b30cf-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b30cf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b30cf-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b30cf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b30cf-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b30cf-117">Optional query parameters</span></span>
<span data-ttu-id="b30cf-118">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b30cf-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b30cf-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b30cf-119">Request headers</span></span>
| <span data-ttu-id="b30cf-120">Header</span><span class="sxs-lookup"><span data-stu-id="b30cf-120">Header</span></span>       | <span data-ttu-id="b30cf-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b30cf-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b30cf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b30cf-122">Authorization</span></span>  | <span data-ttu-id="b30cf-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b30cf-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b30cf-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b30cf-125">Request body</span></span>
<span data-ttu-id="b30cf-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b30cf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b30cf-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="b30cf-127">Response</span></span>
<span data-ttu-id="b30cf-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [conversation](../resources/conversation.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b30cf-128">If successful, this method returns a `200 OK` response code and a [conversation](../resources/conversation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b30cf-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b30cf-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b30cf-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b30cf-130">Request</span></span>
<span data-ttu-id="b30cf-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b30cf-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU="],
  "name": "get_group_conversation"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```

#### <a name="response"></a><span data-ttu-id="b30cf-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="b30cf-132">Response</span></span>
<span data-ttu-id="b30cf-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b30cf-133">The following is an example of the response.</span></span>
><span data-ttu-id="b30cf-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="b30cf-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 644

{
    "id": "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=",
    "topic": "New Training Plans",
    "hasAttachments": false,
    "lastDeliveredDateTime": "2017-07-31T18:59:05Z",
    "uniqueSenders": [
        "HR Taskforce"
    ],
    "preview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
