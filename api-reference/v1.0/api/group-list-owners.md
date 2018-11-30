---
title: Besitzer auflisten
description: 'Dient zum Abrufen einer Liste der Besitzer der Gruppe. Bei den Besitzern handelt es sich um eine Reihe von Benutzern, die keine Administratoren sind, die das Gruppenobjekt ändern können. '
ms.openlocfilehash: 9bb7592827f5dfe9eef2aff0fa8917fe68f683dc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017961"
---
# <a name="list-owners"></a><span data-ttu-id="052fe-104">Besitzer auflisten</span><span class="sxs-lookup"><span data-stu-id="052fe-104">List owners</span></span>
<span data-ttu-id="052fe-p102">Dient zum Abrufen einer Liste der Besitzer der Gruppe. Bei den Besitzern handelt es sich um eine Reihe von Benutzern, die keine Administratoren sind, die das Gruppenobjekt ändern können.</span><span class="sxs-lookup"><span data-stu-id="052fe-p102">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="052fe-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="052fe-107">Permissions</span></span>
<span data-ttu-id="052fe-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="052fe-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="052fe-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="052fe-110">Permission type</span></span>      | <span data-ttu-id="052fe-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="052fe-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="052fe-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="052fe-112">Delegated (work or school account)</span></span> | <span data-ttu-id="052fe-113">Group.Read.All und User.ReadBasic.All, Group.Read.All und User.Read.All, Group.Read.All und User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="052fe-113">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span>   |
|<span data-ttu-id="052fe-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="052fe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="052fe-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="052fe-115">Not supported.</span></span>    |
|<span data-ttu-id="052fe-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="052fe-116">Application</span></span> | <span data-ttu-id="052fe-117">Group.Read.All und User.Read.All, Group.Read.All und User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="052fe-117">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="052fe-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="052fe-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="052fe-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="052fe-119">Optional query parameters</span></span>
<span data-ttu-id="052fe-120">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="052fe-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="052fe-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="052fe-121">Request headers</span></span>
| <span data-ttu-id="052fe-122">Name</span><span class="sxs-lookup"><span data-stu-id="052fe-122">Name</span></span>       | <span data-ttu-id="052fe-123">Typ</span><span class="sxs-lookup"><span data-stu-id="052fe-123">Type</span></span> | <span data-ttu-id="052fe-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="052fe-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="052fe-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="052fe-125">Authorization</span></span>  | <span data-ttu-id="052fe-126">string</span><span class="sxs-lookup"><span data-stu-id="052fe-126">string</span></span>  | <span data-ttu-id="052fe-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="052fe-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="052fe-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="052fe-129">Request body</span></span>
<span data-ttu-id="052fe-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="052fe-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="052fe-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="052fe-131">Response</span></span>
<span data-ttu-id="052fe-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [user](../resources/user.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="052fe-132">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="052fe-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="052fe-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="052fe-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="052fe-134">Request</span></span>
<span data-ttu-id="052fe-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="052fe-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/owners
```

#### <a name="response"></a><span data-ttu-id="052fe-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="052fe-136">Response</span></span>
<span data-ttu-id="052fe-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="052fe-137">The following is an example of the response.</span></span>
><span data-ttu-id="052fe-138">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="052fe-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="052fe-139">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="052fe-139">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.user"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
