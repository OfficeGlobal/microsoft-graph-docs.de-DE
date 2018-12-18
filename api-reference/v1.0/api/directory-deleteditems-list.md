---
title: Gelöschte Elemente auflisten
description: Abrufen einer Liste kürzlich gelöschter Elemente aus den gelöschten Elementen.
author: lleonard-msft
ms.openlocfilehash: 4c972ca554f7a073ddfb5b3472784240c691c973
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314280"
---
# <a name="list-deleted-items"></a><span data-ttu-id="1bd27-103">Gelöschte Elemente auflisten</span><span class="sxs-lookup"><span data-stu-id="1bd27-103">List deleted items</span></span>

<span data-ttu-id="1bd27-104">Abrufen einer Liste kürzlich gelöschter Elemente aus den [gelöschten Elementen](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="1bd27-104">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="1bd27-105">Die Funktion für gelöschte Elemente wird derzeit nur für die Ressourcen [group](../resources/group.md) und [user](../resources/user.md) unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1bd27-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="1bd27-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1bd27-106">Permissions</span></span>
<span data-ttu-id="1bd27-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bd27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="1bd27-109">Für Benutzer:</span><span class="sxs-lookup"><span data-stu-id="1bd27-109">For users:</span></span>

|<span data-ttu-id="1bd27-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1bd27-110">Permission type</span></span>      | <span data-ttu-id="1bd27-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1bd27-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1bd27-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1bd27-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1bd27-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1bd27-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="1bd27-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1bd27-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bd27-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1bd27-115">Not supported.</span></span> |
|<span data-ttu-id="1bd27-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1bd27-116">Application</span></span> | <span data-ttu-id="1bd27-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bd27-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="1bd27-118">Für Gruppen:</span><span class="sxs-lookup"><span data-stu-id="1bd27-118">For groups:</span></span>

|<span data-ttu-id="1bd27-119">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1bd27-119">Permission type</span></span>      | <span data-ttu-id="1bd27-120">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1bd27-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1bd27-121">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1bd27-121">Delegated (work or school account)</span></span> | <span data-ttu-id="1bd27-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1bd27-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="1bd27-123">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1bd27-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bd27-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1bd27-124">Not supported.</span></span>    |
|<span data-ttu-id="1bd27-125">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1bd27-125">Application</span></span> | <span data-ttu-id="1bd27-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="1bd27-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1bd27-127">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1bd27-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deletedItems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="1bd27-128">Diese API unterstützt derzeit das Abrufen von Objekttypen von Gruppen (microsoft.graph.group) oder Benutzern (microsoft.graph.user) aus den gelöschten Elementen.</span><span class="sxs-lookup"><span data-stu-id="1bd27-128">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="1bd27-129">Der Typ wird als ein erforderlicher Bestandteil der URI angegeben.</span><span class="sxs-lookup"><span data-stu-id="1bd27-129">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="1bd27-130">Aufrufen von GET/Verzeichnis/wird DeletedItems ohne einen Typ nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1bd27-130">Calling GET /directory/deletedItems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="1bd27-131">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1bd27-131">Optional query parameters</span></span>
<span data-ttu-id="1bd27-132">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1bd27-132">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1bd27-133">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1bd27-133">Request headers</span></span>
| <span data-ttu-id="1bd27-134">Name</span><span class="sxs-lookup"><span data-stu-id="1bd27-134">Name</span></span>      |<span data-ttu-id="1bd27-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1bd27-135">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1bd27-136">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1bd27-136">Authorization</span></span>  | <span data-ttu-id="1bd27-137">Bearer&lt;code&gt; *erforderlich*</span><span class="sxs-lookup"><span data-stu-id="1bd27-137">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="1bd27-138">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1bd27-138">Accept</span></span>  | <span data-ttu-id="1bd27-139">application/json</span><span class="sxs-lookup"><span data-stu-id="1bd27-139">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1bd27-140">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1bd27-140">Request body</span></span>
<span data-ttu-id="1bd27-141">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1bd27-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bd27-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="1bd27-142">Response</span></span>

<span data-ttu-id="1bd27-143">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1bd27-143">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1bd27-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1bd27-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1bd27-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1bd27-145">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.group
```
##### <a name="response"></a><span data-ttu-id="1bd27-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="1bd27-146">Response</span></span>
<span data-ttu-id="1bd27-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1bd27-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "value": [
    {
      "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
      "displayName":"SampleGroup",
      "groupTypes":["Unified"],
      "mail":"example@contoso.com",
      "mailEnabled":true,
      "mailNickname":"Example",
      "securityEnabled":false,
      "visibility":"Public"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List deleteditems",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->