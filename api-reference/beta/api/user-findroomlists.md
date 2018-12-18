---
title: 'Benutzer: FindRoomLists'
description: Abrufen von Raumlisten in einem Mandanten definiert.
author: dkershaw10
ms.openlocfilehash: f96f8e5c6349e87d2d71820b7b7cd3b0367908f9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310773"
---
# <a name="user-findroomlists"></a><span data-ttu-id="b077b-103">Benutzer: FindRoomLists</span><span class="sxs-lookup"><span data-stu-id="b077b-103">user: findRoomLists</span></span>

> <span data-ttu-id="b077b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b077b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b077b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b077b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b077b-106">Abrufen von Raumlisten in einem Mandanten definiert.</span><span class="sxs-lookup"><span data-stu-id="b077b-106">Get the room lists defined in a tenant.</span></span>

<span data-ttu-id="b077b-107">Mandanten können Besprechungsräumen in Raumlisten zu organisieren.</span><span class="sxs-lookup"><span data-stu-id="b077b-107">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="b077b-108">Jede Besprechungsraum und Raumliste wird von einer Instanz [EmailAddress](../resources/emailaddress.md) dargestellt.</span><span class="sxs-lookup"><span data-stu-id="b077b-108">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span>
<span data-ttu-id="b077b-109">Sie können die Chatroom-Listen in den Mandanten, [erhalten alle Chatrooms](user-findrooms.md) im Mandanten oder eine bestimmte Raumliste [aller Chatrooms abrufen](user-findrooms.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="b077b-109">You can get all the room lists in the tenant, [get all the rooms](user-findrooms.md) in the tenant, or [get all the rooms](user-findrooms.md) in a specific room list.</span></span>


## <a name="permissions"></a><span data-ttu-id="b077b-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b077b-110">Permissions</span></span>
<span data-ttu-id="b077b-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b077b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b077b-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b077b-113">Permission type</span></span>      | <span data-ttu-id="b077b-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b077b-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b077b-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b077b-115">Delegated (work or school account)</span></span> | <span data-ttu-id="b077b-116">User.ReadBasic.All User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b077b-116">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="b077b-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b077b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b077b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b077b-118">Not supported.</span></span>    |
|<span data-ttu-id="b077b-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b077b-119">Application</span></span> | <span data-ttu-id="b077b-120">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b077b-120">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b077b-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b077b-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/findRoomLists
GET /users/<id>/findRoomLists

```

## <a name="request-headers"></a><span data-ttu-id="b077b-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b077b-122">Request headers</span></span>
| <span data-ttu-id="b077b-123">Name</span><span class="sxs-lookup"><span data-stu-id="b077b-123">Name</span></span>       | <span data-ttu-id="b077b-124">Typ</span><span class="sxs-lookup"><span data-stu-id="b077b-124">Type</span></span> | <span data-ttu-id="b077b-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b077b-125">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="b077b-126">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b077b-126">Authorization</span></span>  | <span data-ttu-id="b077b-127">string</span><span class="sxs-lookup"><span data-stu-id="b077b-127">string</span></span>  | <span data-ttu-id="b077b-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b077b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b077b-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b077b-130">Content-Type</span></span>  | <span data-ttu-id="b077b-131">string</span><span class="sxs-lookup"><span data-stu-id="b077b-131">string</span></span>  | <span data-ttu-id="b077b-p105">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="b077b-p105">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="b077b-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b077b-134">Request body</span></span>
<span data-ttu-id="b077b-135">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b077b-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b077b-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="b077b-136">Response</span></span>

<span data-ttu-id="b077b-137">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwort Code und [EmailAddress](../resources/emailaddress.md) -Auflistungsobjekt in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b077b-137">If successful, this method returns a `200 OK` response code and [emailAddress](../resources/emailaddress.md) collection object in the response body.</span></span>

<span data-ttu-id="b077b-138">Wenn keine Listen in den Mandanten definiert sind, wird ein leeres Array zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b077b-138">If no lists are defined in the tenant, then an empty array is returned.</span></span>

## <a name="example"></a><span data-ttu-id="b077b-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b077b-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b077b-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b077b-140">Request</span></span>

<span data-ttu-id="b077b-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b077b-141">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_room_lists"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRoomLists
```

##### <a name="response"></a><span data-ttu-id="b077b-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="b077b-142">Response</span></span>
<span data-ttu-id="b077b-143">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b077b-143">Here is an example of the response.</span></span> 

<span data-ttu-id="b077b-p106">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b077b-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_get_room_lists",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAddress",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAddress)",
    "value": [
        {
            "name": "Building 1 Rooms",
            "address": "Building1Rooms@contoso.onmicrosoft.com"
        },
        {
            "name": "Building 2 Rooms",
            "address": "Building2Rooms@contoso.onmicrosoft.com"
        }
    ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: findRoomLists",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->