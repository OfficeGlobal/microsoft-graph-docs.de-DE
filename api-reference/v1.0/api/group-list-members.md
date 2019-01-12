---
title: Mitglieder auflisten
description: Rufen Sie eine Liste der direkte Mitglieder der Gruppe. Eine Gruppe kann Benutzer, Kontakte und andere Gruppen als Mitglieder haben.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 70bf3040402c03dc1918d271a2abb8e4adb5d40b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936529"
---
# <a name="list-members"></a><span data-ttu-id="1c8ce-104">Mitglieder auflisten</span><span class="sxs-lookup"><span data-stu-id="1c8ce-104">List members</span></span>
<span data-ttu-id="1c8ce-p102">Dient zum Abrufen einer Liste der direkten Mitglieder einer Gruppe. Eine Gruppe kann Benutzer, Kontakten und andere Gruppen als Mitglieder haben. Dieser Vorgang ist nicht transitiv.</span><span class="sxs-lookup"><span data-stu-id="1c8ce-p102">Get a list of the group's direct members. A group can have users, contacts, and other groups as members. This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c8ce-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1c8ce-108">Permissions</span></span>
<span data-ttu-id="1c8ce-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c8ce-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c8ce-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1c8ce-111">Permission type</span></span>      | <span data-ttu-id="1c8ce-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1c8ce-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c8ce-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1c8ce-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1c8ce-114">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1c8ce-114">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="1c8ce-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1c8ce-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c8ce-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c8ce-116">Not supported.</span></span>    |
|<span data-ttu-id="1c8ce-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1c8ce-117">Application</span></span> | <span data-ttu-id="1c8ce-118">User.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c8ce-118">User.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c8ce-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c8ce-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1c8ce-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1c8ce-120">Optional query parameters</span></span>
<span data-ttu-id="1c8ce-121">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1c8ce-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c8ce-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1c8ce-122">Request headers</span></span>
| <span data-ttu-id="1c8ce-123">Name</span><span class="sxs-lookup"><span data-stu-id="1c8ce-123">Name</span></span>       | <span data-ttu-id="1c8ce-124">Typ</span><span class="sxs-lookup"><span data-stu-id="1c8ce-124">Type</span></span> | <span data-ttu-id="1c8ce-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1c8ce-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1c8ce-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c8ce-126">Authorization</span></span>  | <span data-ttu-id="1c8ce-127">string</span><span class="sxs-lookup"><span data-stu-id="1c8ce-127">string</span></span>  | <span data-ttu-id="1c8ce-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1c8ce-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c8ce-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1c8ce-130">Request body</span></span>
<span data-ttu-id="1c8ce-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1c8ce-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c8ce-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c8ce-132">Response</span></span>
<span data-ttu-id="1c8ce-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1c8ce-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c8ce-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1c8ce-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1c8ce-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c8ce-135">Request</span></span>
<span data-ttu-id="1c8ce-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1c8ce-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```

#### <a name="response"></a><span data-ttu-id="1c8ce-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c8ce-137">Response</span></span>
<span data-ttu-id="1c8ce-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1c8ce-138">The following is an example of the response.</span></span>
><span data-ttu-id="1c8ce-139">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="1c8ce-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1c8ce-140">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="1c8ce-140">All the properties will be returned from an actual call.</span></span>
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
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
