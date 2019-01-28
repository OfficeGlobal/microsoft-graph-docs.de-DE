---
title: 'user: findRooms'
description: 'Abrufen aller Besprechungsräume im Mandanten des Benutzers oder in einer bestimmten Raumliste. '
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 70bd060f3c2d5722dca365e4d5f4c7595eab26cd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524170"
---
# <a name="user-findrooms"></a><span data-ttu-id="4cfc2-103">user: findRooms</span><span class="sxs-lookup"><span data-stu-id="4cfc2-103">user: findRooms</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4cfc2-104">Abrufen aller Besprechungsräume im Mandanten des Benutzers oder in einer bestimmten Raumliste.</span><span class="sxs-lookup"><span data-stu-id="4cfc2-104">Get all the meeting rooms in the user's tenant or in a specific room list.</span></span> 

<span data-ttu-id="4cfc2-105">Mandanten können Besprechungsräume in Raumlisten organisieren.</span><span class="sxs-lookup"><span data-stu-id="4cfc2-105">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="4cfc2-106">Jeder Besprechungsraum und jede Raumliste wird durch eine [emailAddress](../resources/emailaddress.md)-Instanz dargestellt.</span><span class="sxs-lookup"><span data-stu-id="4cfc2-106">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span> <span data-ttu-id="4cfc2-107">Sie können [alle Raumlisten im Mandanten](user-findroomlists.md), alle Räume im Mandanten oder alle Räume in einer bestimmten Raumliste abrufen.</span><span class="sxs-lookup"><span data-stu-id="4cfc2-107">You can [get all the room lists](user-findroomlists.md) in the tenant, get all the rooms in the tenant, or get all the rooms in a specific room list.</span></span> <span data-ttu-id="4cfc2-108">Sie können die ersten 100 Räume im Mandanten abrufen.</span><span class="sxs-lookup"><span data-stu-id="4cfc2-108">You can get up to the first 100 rooms in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="4cfc2-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4cfc2-109">Permissions</span></span>
<span data-ttu-id="4cfc2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cfc2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4cfc2-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4cfc2-112">Permission type</span></span>      | <span data-ttu-id="4cfc2-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4cfc2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4cfc2-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4cfc2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4cfc2-115">User.ReadBasic.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4cfc2-115">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4cfc2-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4cfc2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4cfc2-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4cfc2-117">Not supported.</span></span>    |
|<span data-ttu-id="4cfc2-118">Application</span><span class="sxs-lookup"><span data-stu-id="4cfc2-118">Application</span></span> | <span data-ttu-id="4cfc2-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4cfc2-119">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4cfc2-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4cfc2-120">HTTP request</span></span>

<span data-ttu-id="4cfc2-121">So rufen Sie alle Räume im Mandanten ab:</span><span class="sxs-lookup"><span data-stu-id="4cfc2-121">To get all the rooms in the tenant:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms
GET /users/<id>/findRooms
```

<span data-ttu-id="4cfc2-122">So rufen Sie alle Räume in einer bestimmten Raumliste des Mandanten ab:</span><span class="sxs-lookup"><span data-stu-id="4cfc2-122">To get all the rooms in a specific room list of the tenant's:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms(RoomList='{room_list}')
GET /users/<id>/findRooms(RoomList='{room_list}')
```

## <a name="query-parameters"></a><span data-ttu-id="4cfc2-123">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4cfc2-123">Query parameters</span></span>

| <span data-ttu-id="4cfc2-124">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4cfc2-124">Query parameter</span></span>       | <span data-ttu-id="4cfc2-125">Typ</span><span class="sxs-lookup"><span data-stu-id="4cfc2-125">Type</span></span> | <span data-ttu-id="4cfc2-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4cfc2-126">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="4cfc2-127">RoomList</span><span class="sxs-lookup"><span data-stu-id="4cfc2-127">RoomList</span></span> | <span data-ttu-id="4cfc2-128">string</span><span class="sxs-lookup"><span data-stu-id="4cfc2-128">string</span></span> | <span data-ttu-id="4cfc2-129">Die der Raumliste zugeordnete SMTP-Adresse.</span><span class="sxs-lookup"><span data-stu-id="4cfc2-129">The SMTP address associated with the room list.</span></span> <span data-ttu-id="4cfc2-130">Jede Raumliste wird durch eine [emailAddress](../resources/emailaddress.md)-Instanz dargestellt, die eine SMTP-Adresse enthält.</span><span class="sxs-lookup"><span data-stu-id="4cfc2-130">Each room list is represented by an [emailAddress](../resources/emailaddress.md) instance that includes an SMTP address.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="4cfc2-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4cfc2-131">Request headers</span></span>
| <span data-ttu-id="4cfc2-132">Name</span><span class="sxs-lookup"><span data-stu-id="4cfc2-132">Name</span></span>       | <span data-ttu-id="4cfc2-133">Typ</span><span class="sxs-lookup"><span data-stu-id="4cfc2-133">Type</span></span> | <span data-ttu-id="4cfc2-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4cfc2-134">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="4cfc2-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="4cfc2-135">Authorization</span></span>  | <span data-ttu-id="4cfc2-136">string</span><span class="sxs-lookup"><span data-stu-id="4cfc2-136">string</span></span>  | <span data-ttu-id="4cfc2-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4cfc2-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4cfc2-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4cfc2-139">Content-Type</span></span>  | <span data-ttu-id="4cfc2-140">string</span><span class="sxs-lookup"><span data-stu-id="4cfc2-140">string</span></span>  | <span data-ttu-id="4cfc2-p105">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="4cfc2-p105">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="4cfc2-143">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4cfc2-143">Request body</span></span>
<span data-ttu-id="4cfc2-144">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4cfc2-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4cfc2-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="4cfc2-145">Response</span></span>

<span data-ttu-id="4cfc2-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [emailAddress](../resources/emailaddress.md)-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4cfc2-146">If successful, this method returns a `200 OK` response code and [message](../resources/emailaddress.md) collection object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="4cfc2-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4cfc2-147">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="4cfc2-148">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="4cfc2-148">Request 1</span></span>

<span data-ttu-id="4cfc2-149">Das erste Beispiel ruft alle Räume ab, die im Mandanten des angemeldeten Benutzers definiert sind.</span><span class="sxs-lookup"><span data-stu-id="4cfc2-149">The first example gets all the rooms defined in the signed-in user's tenant.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_rooms_in_tenant"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms
```

##### <a name="response-1"></a><span data-ttu-id="4cfc2-150">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="4cfc2-150">Response 1</span></span>
<span data-ttu-id="4cfc2-151">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4cfc2-151">Here is an example of the response.</span></span> 

<span data-ttu-id="4cfc2-p106">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4cfc2-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="4cfc2-154">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="4cfc2-154">Request 2</span></span>

<span data-ttu-id="4cfc2-155">Das zweite Beispiel ruft die Räume in der angegebenen Raumliste ab, die durch die E-Mail-Adresse Building2Rooms@contoso.onmicrosoft.com gekennzeichnet ist.</span><span class="sxs-lookup"><span data-stu-id="4cfc2-155">The second example gets the rooms in the specified room list identified by the email address Building2Rooms@contoso.onmicrosoft.com.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_rooms_from_specific_list"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms(RoomList='Building2Rooms@contoso.onmicrosoft.com') 
```

##### <a name="response-2"></a><span data-ttu-id="4cfc2-156">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="4cfc2-156">Response 2</span></span>
<span data-ttu-id="4cfc2-157">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4cfc2-157">Here is an example of the response.</span></span> 

<span data-ttu-id="4cfc2-p107">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4cfc2-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "user: findRooms",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-findrooms.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
