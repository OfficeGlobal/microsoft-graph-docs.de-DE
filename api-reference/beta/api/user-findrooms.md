---
title: 'Benutzer: FindRooms'
description: 'Rufen Sie allen Besprechungsräumen Mandant des Benutzers oder in einer bestimmten Raumliste. '
ms.openlocfilehash: 3169202f83af0696cbd2aaadd83d3beb9a3c01d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063493"
---
# <a name="user-findrooms"></a><span data-ttu-id="bfd3b-103">Benutzer: FindRooms</span><span class="sxs-lookup"><span data-stu-id="bfd3b-103">user: findRooms</span></span>

> <span data-ttu-id="bfd3b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bfd3b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bfd3b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bfd3b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bfd3b-106">Rufen Sie allen Besprechungsräumen Mandant des Benutzers oder in einer bestimmten Raumliste.</span><span class="sxs-lookup"><span data-stu-id="bfd3b-106">Get all the meeting rooms in the user's tenant or in a specific room list.</span></span> 

<span data-ttu-id="bfd3b-107">Mandanten können Besprechungsräumen in Raumlisten zu organisieren.</span><span class="sxs-lookup"><span data-stu-id="bfd3b-107">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="bfd3b-108">Jede Besprechungsraum und Raumliste wird von einer Instanz [EmailAddress](../resources/emailaddress.md) dargestellt.</span><span class="sxs-lookup"><span data-stu-id="bfd3b-108">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span> <span data-ttu-id="bfd3b-109">Sie können [Alle Chatroom-Listen abrufen](user-findroomlists.md) im Mandanten, Abrufen von allen Chatrooms im Mandanten oder alle Chatrooms in einer bestimmten Raumliste abrufen.</span><span class="sxs-lookup"><span data-stu-id="bfd3b-109">You can [get all the room lists](user-findroomlists.md) in the tenant, get all the rooms in the tenant, or get all the rooms in a specific room list.</span></span> <span data-ttu-id="bfd3b-110">Sie können die ersten 100 Räume im Mandanten Einstieg.</span><span class="sxs-lookup"><span data-stu-id="bfd3b-110">You can get up to the first 100 rooms in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="bfd3b-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bfd3b-111">Permissions</span></span>
<span data-ttu-id="bfd3b-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfd3b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bfd3b-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bfd3b-114">Permission type</span></span>      | <span data-ttu-id="bfd3b-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bfd3b-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfd3b-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bfd3b-116">Delegated (work or school account)</span></span> | <span data-ttu-id="bfd3b-117">User.ReadBasic.All User.Read.All</span><span class="sxs-lookup"><span data-stu-id="bfd3b-117">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="bfd3b-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bfd3b-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfd3b-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bfd3b-119">Not supported.</span></span>    |
|<span data-ttu-id="bfd3b-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bfd3b-120">Application</span></span> | <span data-ttu-id="bfd3b-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="bfd3b-121">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfd3b-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bfd3b-122">HTTP request</span></span>

<span data-ttu-id="bfd3b-123">So erhalten Sie alle Chatrooms im Mandanten:</span><span class="sxs-lookup"><span data-stu-id="bfd3b-123">To get all the rooms in the tenant:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms
GET /users/<id>/findRooms
```

<span data-ttu-id="bfd3b-124">So erhalten Sie alle Chatrooms in einer speziellen Raum des Mandantenverwaltungs</span><span class="sxs-lookup"><span data-stu-id="bfd3b-124">To get all the rooms in a specific room list of the tenant's:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms(RoomList='{room_list}')
GET /users/<id>/findRooms(RoomList='{room_list}')
```

## <a name="query-parameters"></a><span data-ttu-id="bfd3b-125">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="bfd3b-125">Query parameters</span></span>

| <span data-ttu-id="bfd3b-126">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="bfd3b-126">Query parameter</span></span>       | <span data-ttu-id="bfd3b-127">Typ</span><span class="sxs-lookup"><span data-stu-id="bfd3b-127">Type</span></span> | <span data-ttu-id="bfd3b-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bfd3b-128">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="bfd3b-129">RoomList</span><span class="sxs-lookup"><span data-stu-id="bfd3b-129">RoomList</span></span> | <span data-ttu-id="bfd3b-130">string</span><span class="sxs-lookup"><span data-stu-id="bfd3b-130">string</span></span> | <span data-ttu-id="bfd3b-131">Die SMTP-Adresse der Raumliste zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="bfd3b-131">The SMTP address associated with the room list.</span></span> <span data-ttu-id="bfd3b-132">Jede Raumliste wird von einer Instanz [EmailAddress](../resources/emailaddress.md) dargestellt, die eine SMTP-Adresse enthält.</span><span class="sxs-lookup"><span data-stu-id="bfd3b-132">Each room list is represented by an [emailAddress](../resources/emailaddress.md) instance that includes an SMTP address.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="bfd3b-133">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bfd3b-133">Request headers</span></span>
| <span data-ttu-id="bfd3b-134">Name</span><span class="sxs-lookup"><span data-stu-id="bfd3b-134">Name</span></span>       | <span data-ttu-id="bfd3b-135">Typ</span><span class="sxs-lookup"><span data-stu-id="bfd3b-135">Type</span></span> | <span data-ttu-id="bfd3b-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bfd3b-136">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="bfd3b-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfd3b-137">Authorization</span></span>  | <span data-ttu-id="bfd3b-138">string</span><span class="sxs-lookup"><span data-stu-id="bfd3b-138">string</span></span>  | <span data-ttu-id="bfd3b-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bfd3b-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bfd3b-141">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bfd3b-141">Content-Type</span></span>  | <span data-ttu-id="bfd3b-142">string</span><span class="sxs-lookup"><span data-stu-id="bfd3b-142">string</span></span>  | <span data-ttu-id="bfd3b-p106">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="bfd3b-p106">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="bfd3b-145">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bfd3b-145">Request body</span></span>
<span data-ttu-id="bfd3b-146">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bfd3b-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bfd3b-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="bfd3b-147">Response</span></span>

<span data-ttu-id="bfd3b-148">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwort Code und [EmailAddress](../resources/emailaddress.md) -Auflistungsobjekt in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="bfd3b-148">If successful, this method returns a `200 OK` response code and [emailAddress](../resources/emailaddress.md) collection object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="bfd3b-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bfd3b-149">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="bfd3b-150">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="bfd3b-150">Request 1</span></span>

<span data-ttu-id="bfd3b-151">Im erste Beispiel ruft alle Chatrooms, die gemäß der Mandant des angemeldeten Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="bfd3b-151">The first example gets all the rooms defined in the signed-in user's tenant.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_rooms_in_tenant"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms
```

##### <a name="response-1"></a><span data-ttu-id="bfd3b-152">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="bfd3b-152">Response 1</span></span>
<span data-ttu-id="bfd3b-153">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bfd3b-153">Here is an example of the response.</span></span> 

<span data-ttu-id="bfd3b-p107">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bfd3b-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_get_rooms_in_tenant",
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
            "name": "Conf Room Adams",
            "address": "Adams@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Baker",
            "address": "Baker@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Crystal",
            "address": "Crystal@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Hood",
            "address": "Hood@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Rainier",
            "address": "Rainier@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Stevens",
            "address": "Stevens@contoso.onmicrosoft.com"
        }
    ]
}
```

##### <a name="request-2"></a><span data-ttu-id="bfd3b-156">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="bfd3b-156">Request 2</span></span>

<span data-ttu-id="bfd3b-157">Im zweiten Beispiel wird die Chatrooms in der angegebenen Raumliste durch die e-Mail-Adresse Building2Rooms@contoso.onmicrosoft.com identifiziert.</span><span class="sxs-lookup"><span data-stu-id="bfd3b-157">The second example gets the rooms in the specified room list identified by the email address Building2Rooms@contoso.onmicrosoft.com.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_rooms_from_specific_list"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms(RoomList='Building2Rooms@contoso.onmicrosoft.com') 
```

##### <a name="response-2"></a><span data-ttu-id="bfd3b-158">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="bfd3b-158">Response 2</span></span>
<span data-ttu-id="bfd3b-159">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bfd3b-159">Here is an example of the response.</span></span> 

<span data-ttu-id="bfd3b-p108">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bfd3b-p108">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_get_rooms_from_specific_list",
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
            "name": "Conf Room Baker",
            "address": "Baker@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Hood",
            "address": "Hood@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Rainier",
            "address": "Rainier@contoso.onmicrosoft.com"
        }
    ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: findRooms",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->