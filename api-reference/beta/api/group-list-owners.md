---
title: Besitzer auflisten
description: Dient zum Abrufen einer Liste der Besitzer der Gruppe. Bei den Besitzern handelt es sich um eine Reihe von Benutzern, die keine Administratoren sind, die das Gruppenobjekt ändern können.
localization_priority: Normal
ms.openlocfilehash: d173b7a350d4aedbf1ec96b0b5e37da70e87d078
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878974"
---
# <a name="list-owners"></a><span data-ttu-id="cc209-104">Besitzer auflisten</span><span class="sxs-lookup"><span data-stu-id="cc209-104">List owners</span></span>

> <span data-ttu-id="cc209-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cc209-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc209-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cc209-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cc209-p103">Dient zum Abrufen einer Liste der Besitzer der Gruppe. Bei den Besitzern handelt es sich um eine Reihe von Benutzern, die keine Administratoren sind, die das Gruppenobjekt ändern können.</span><span class="sxs-lookup"><span data-stu-id="cc209-p103">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc209-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cc209-109">Permissions</span></span>
<span data-ttu-id="cc209-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc209-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc209-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cc209-112">Permission type</span></span>      | <span data-ttu-id="cc209-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cc209-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc209-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cc209-114">Delegated (work or school account)</span></span> | <span data-ttu-id="cc209-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cc209-115">Not supported.</span></span>    |
|<span data-ttu-id="cc209-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cc209-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc209-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cc209-117">Not supported.</span></span>    |
|<span data-ttu-id="cc209-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cc209-118">Application</span></span> | <span data-ttu-id="cc209-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cc209-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc209-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cc209-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cc209-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cc209-121">Optional query parameters</span></span>
<span data-ttu-id="cc209-122">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cc209-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc209-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cc209-123">Request headers</span></span>
| <span data-ttu-id="cc209-124">Name</span><span class="sxs-lookup"><span data-stu-id="cc209-124">Name</span></span>       | <span data-ttu-id="cc209-125">Typ</span><span class="sxs-lookup"><span data-stu-id="cc209-125">Type</span></span> | <span data-ttu-id="cc209-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cc209-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cc209-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc209-127">Authorization</span></span>  | <span data-ttu-id="cc209-128">string</span><span class="sxs-lookup"><span data-stu-id="cc209-128">string</span></span>  | <span data-ttu-id="cc209-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cc209-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc209-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cc209-131">Request body</span></span>
<span data-ttu-id="cc209-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cc209-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc209-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="cc209-133">Response</span></span>
<span data-ttu-id="cc209-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cc209-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc209-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cc209-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cc209-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cc209-136">Request</span></span>
<span data-ttu-id="cc209-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cc209-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/owners
```

#### <a name="response"></a><span data-ttu-id="cc209-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="cc209-138">Response</span></span>
<span data-ttu-id="cc209-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cc209-139">The following is an example of the response.</span></span>
><span data-ttu-id="cc209-140">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="cc209-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cc209-141">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="cc209-141">All the properties will be returned from an actual call.</span></span>
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
      "id": "id-value"
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
