---
title: Auflisten von Fotos
description: Mit dieser API können Sie eine Liste von Objekten des Typs profilePhoto abrufen.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 01fd069173fff1a7a6868f1596326fcb44d77fb7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932273"
---
# <a name="list-photos"></a><span data-ttu-id="d7074-103">Auflisten von Fotos</span><span class="sxs-lookup"><span data-stu-id="d7074-103">List photos</span></span>
<span data-ttu-id="d7074-104">Mit dieser API können Sie eine Liste von Objekten des Typs [profilePhoto](../resources/profilephoto.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="d7074-104">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7074-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d7074-105">Permissions</span></span>
<span data-ttu-id="d7074-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7074-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7074-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d7074-108">Permission type</span></span>      | <span data-ttu-id="d7074-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d7074-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7074-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d7074-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d7074-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7074-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="d7074-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d7074-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7074-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d7074-113">Not supported.</span></span>    |
|<span data-ttu-id="d7074-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d7074-114">Application</span></span> | <span data-ttu-id="d7074-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7074-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7074-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7074-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d7074-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d7074-117">Optional query parameters</span></span>
<span data-ttu-id="d7074-118">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d7074-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d7074-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d7074-119">Request headers</span></span>
| <span data-ttu-id="d7074-120">Name</span><span class="sxs-lookup"><span data-stu-id="d7074-120">Name</span></span>       | <span data-ttu-id="d7074-121">Typ</span><span class="sxs-lookup"><span data-stu-id="d7074-121">Type</span></span> | <span data-ttu-id="d7074-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d7074-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d7074-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7074-123">Authorization</span></span>  | <span data-ttu-id="d7074-124">string</span><span class="sxs-lookup"><span data-stu-id="d7074-124">string</span></span>  | <span data-ttu-id="d7074-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d7074-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7074-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d7074-127">Request body</span></span>
<span data-ttu-id="d7074-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d7074-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7074-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7074-129">Response</span></span>
<span data-ttu-id="d7074-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von  [profilePhoto](../resources/profilephoto.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d7074-130">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7074-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d7074-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d7074-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7074-132">Request</span></span>
<span data-ttu-id="d7074-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d7074-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/photos
```

#### <a name="response"></a><span data-ttu-id="d7074-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7074-134">Response</span></span>
<span data-ttu-id="d7074-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d7074-135">The following is an example of the response.</span></span>
><span data-ttu-id="d7074-136">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="d7074-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d7074-137">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="d7074-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profilePhoto",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 94

{
  "value": [
    {
      "height": 99,
      "width": 99,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List photos",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
