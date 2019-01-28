---
title: 'user: findRoomLists'
description: Abrufen der in einem Mandanten definierten Raumlisten.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1cc26367c9cecd16604f7cfefb3be5ce265e3c2c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520578"
---
# <a name="user-findroomlists"></a><span data-ttu-id="f008e-103">user: findRoomLists</span><span class="sxs-lookup"><span data-stu-id="f008e-103">user: findRoomLists</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f008e-104">Abrufen der in einem Mandanten definierten Raumlisten.</span><span class="sxs-lookup"><span data-stu-id="f008e-104">Get the room lists defined in a tenant.</span></span>

<span data-ttu-id="f008e-105">Mandanten können Besprechungsräume in Raumlisten organisieren.</span><span class="sxs-lookup"><span data-stu-id="f008e-105">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="f008e-106">Jeder Besprechungsraum und jede Raumliste wird durch eine [emailAddress](../resources/emailaddress.md)-Instanz dargestellt.</span><span class="sxs-lookup"><span data-stu-id="f008e-106">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span>
<span data-ttu-id="f008e-107">Sie können alle Raumlisten im Mandanten, [alle Räume](user-findrooms.md) im Mandanten oder [alle Räume](user-findrooms.md) in einer bestimmten Raumliste abrufen.</span><span class="sxs-lookup"><span data-stu-id="f008e-107">You can get all the room lists in the tenant, [get all the rooms](user-findrooms.md) in the tenant, or [get all the rooms](user-findrooms.md) in a specific room list.</span></span>


## <a name="permissions"></a><span data-ttu-id="f008e-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f008e-108">Permissions</span></span>
<span data-ttu-id="f008e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f008e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f008e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f008e-111">Permission type</span></span>      | <span data-ttu-id="f008e-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f008e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f008e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f008e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f008e-114">User.ReadBasic.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="f008e-114">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f008e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f008e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f008e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f008e-116">Not supported.</span></span>    |
|<span data-ttu-id="f008e-117">Application</span><span class="sxs-lookup"><span data-stu-id="f008e-117">Application</span></span> | <span data-ttu-id="f008e-118">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="f008e-118">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f008e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f008e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/findRoomLists
GET /users/<id>/findRoomLists

```

## <a name="request-headers"></a><span data-ttu-id="f008e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f008e-120">Request headers</span></span>
| <span data-ttu-id="f008e-121">Name</span><span class="sxs-lookup"><span data-stu-id="f008e-121">Name</span></span>       | <span data-ttu-id="f008e-122">Typ</span><span class="sxs-lookup"><span data-stu-id="f008e-122">Type</span></span> | <span data-ttu-id="f008e-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f008e-123">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="f008e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f008e-124">Authorization</span></span>  | <span data-ttu-id="f008e-125">string</span><span class="sxs-lookup"><span data-stu-id="f008e-125">string</span></span>  | <span data-ttu-id="f008e-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f008e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f008e-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f008e-128">Content-Type</span></span>  | <span data-ttu-id="f008e-129">string</span><span class="sxs-lookup"><span data-stu-id="f008e-129">string</span></span>  | <span data-ttu-id="f008e-p104">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="f008e-p104">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="f008e-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f008e-132">Request body</span></span>
<span data-ttu-id="f008e-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f008e-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f008e-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f008e-134">Response</span></span>

<span data-ttu-id="f008e-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [emailAddress](../resources/emailaddress.md)-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f008e-135">If successful, this method returns a `200 OK` response code and [emailAddress](../resources/emailaddress.md) collection object in the response body.</span></span>

<span data-ttu-id="f008e-136">Wenn keine Listen im Mandanten definiert sind, wird ein leeres Array zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f008e-136">If no lists are defined in the tenant, then an empty array is returned.</span></span>

## <a name="example"></a><span data-ttu-id="f008e-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f008e-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f008e-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f008e-138">Request</span></span>

<span data-ttu-id="f008e-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f008e-139">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_room_lists"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRoomLists
```

##### <a name="response"></a><span data-ttu-id="f008e-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="f008e-140">Response</span></span>
<span data-ttu-id="f008e-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f008e-141">Here is an example of the response.</span></span> 

<span data-ttu-id="f008e-p105">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f008e-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "user: findRoomLists",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-findroomlists.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
