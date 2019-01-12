---
title: Auflisten von Fotos
description: Mit dieser API können Sie eine Liste von Objekten des Typs profilePhoto abrufen.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 51c8ba85aa183b07c8e7497dbd2b64ded0b87ad0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951068"
---
# <a name="list-photos"></a><span data-ttu-id="50a8e-103">Auflisten von Fotos</span><span class="sxs-lookup"><span data-stu-id="50a8e-103">List photos</span></span>

> <span data-ttu-id="50a8e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="50a8e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="50a8e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="50a8e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="50a8e-106">Mit dieser API können Sie eine Liste von Objekten des Typs [profilePhoto](../resources/profilephoto.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="50a8e-106">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="50a8e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="50a8e-107">Permissions</span></span>
<span data-ttu-id="50a8e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50a8e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50a8e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="50a8e-110">Permission type</span></span>      | <span data-ttu-id="50a8e-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="50a8e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50a8e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="50a8e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="50a8e-113">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50a8e-113">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="50a8e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="50a8e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50a8e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50a8e-115">Not supported.</span></span>    |
|<span data-ttu-id="50a8e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="50a8e-116">Application</span></span> | <span data-ttu-id="50a8e-117">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50a8e-117">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="50a8e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="50a8e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```

## <a name="optional-query-parameters"></a><span data-ttu-id="50a8e-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="50a8e-119">Optional query parameters</span></span>
<span data-ttu-id="50a8e-120">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="50a8e-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50a8e-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="50a8e-121">Request headers</span></span>
| <span data-ttu-id="50a8e-122">Name</span><span class="sxs-lookup"><span data-stu-id="50a8e-122">Name</span></span>       | <span data-ttu-id="50a8e-123">Typ</span><span class="sxs-lookup"><span data-stu-id="50a8e-123">Type</span></span> | <span data-ttu-id="50a8e-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="50a8e-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="50a8e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="50a8e-125">Authorization</span></span>  | <span data-ttu-id="50a8e-126">string</span><span class="sxs-lookup"><span data-stu-id="50a8e-126">string</span></span>  | <span data-ttu-id="50a8e-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="50a8e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50a8e-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="50a8e-129">Request body</span></span>
<span data-ttu-id="50a8e-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="50a8e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50a8e-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="50a8e-131">Response</span></span>
<span data-ttu-id="50a8e-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von  [profilePhoto](../resources/profilephoto.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="50a8e-132">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50a8e-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="50a8e-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="50a8e-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="50a8e-134">Request</span></span>
<span data-ttu-id="50a8e-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="50a8e-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/photos
```

#### <a name="response"></a><span data-ttu-id="50a8e-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="50a8e-136">Response</span></span>
<span data-ttu-id="50a8e-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="50a8e-137">The following is an example of the response.</span></span>
><span data-ttu-id="50a8e-138">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="50a8e-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="50a8e-139">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="50a8e-139">All the properties will be returned from an actual call.</span></span>
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
