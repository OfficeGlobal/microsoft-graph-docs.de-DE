---
title: Gelöschtes Element abrufen
description: Abrufen der Eigenschaften eines kürzlich gelöschten Elements aus den gelöschten Elementen.
ms.openlocfilehash: 513b9d8e48cbf4474024b61b7274aa9943daa025
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016189"
---
# <a name="get-deleted-item"></a><span data-ttu-id="743c8-103">Gelöschtes Element abrufen</span><span class="sxs-lookup"><span data-stu-id="743c8-103">Get deleted item</span></span>

<span data-ttu-id="743c8-104">Abrufen der Eigenschaften eines kürzlich gelöschten Elements aus den [gelöschten Elementen](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="743c8-104">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="743c8-105">Die Funktion für gelöschte Elemente wird derzeit nur für die Ressourcen [group](../resources/group.md) und [user](../resources/user.md) unterstützt.</span><span class="sxs-lookup"><span data-stu-id="743c8-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="743c8-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="743c8-106">Permissions</span></span>
<span data-ttu-id="743c8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="743c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="743c8-109">Für Benutzer:</span><span class="sxs-lookup"><span data-stu-id="743c8-109">For users:</span></span>

|<span data-ttu-id="743c8-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="743c8-110">Permission type</span></span>      | <span data-ttu-id="743c8-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="743c8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="743c8-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="743c8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="743c8-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="743c8-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span></span> |
|<span data-ttu-id="743c8-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="743c8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="743c8-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="743c8-115">Not supported.</span></span> |
|<span data-ttu-id="743c8-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="743c8-116">Application</span></span> | <span data-ttu-id="743c8-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="743c8-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="743c8-118">Für Gruppen:</span><span class="sxs-lookup"><span data-stu-id="743c8-118">For groups:</span></span>

|<span data-ttu-id="743c8-119">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="743c8-119">Permission type</span></span>      | <span data-ttu-id="743c8-120">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="743c8-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="743c8-121">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="743c8-121">Delegated (work or school account)</span></span> | <span data-ttu-id="743c8-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="743c8-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="743c8-123">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="743c8-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="743c8-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="743c8-124">Not supported.</span></span>    |
|<span data-ttu-id="743c8-125">Anwendung</span><span class="sxs-lookup"><span data-stu-id="743c8-125">Application</span></span> | <span data-ttu-id="743c8-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="743c8-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="743c8-127">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="743c8-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deletedItems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="743c8-128">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="743c8-128">Optional query parameters</span></span>
<span data-ttu-id="743c8-129">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="743c8-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="743c8-130">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="743c8-130">Request headers</span></span>
| <span data-ttu-id="743c8-131">Name</span><span class="sxs-lookup"><span data-stu-id="743c8-131">Name</span></span>      |<span data-ttu-id="743c8-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="743c8-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="743c8-133">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="743c8-133">Authorization</span></span>  | <span data-ttu-id="743c8-134">Bearer&lt;code&gt; *erforderlich*</span><span class="sxs-lookup"><span data-stu-id="743c8-134">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="743c8-135">Annehmen</span><span class="sxs-lookup"><span data-stu-id="743c8-135">Accept</span></span>  | <span data-ttu-id="743c8-136">application/json</span><span class="sxs-lookup"><span data-stu-id="743c8-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="743c8-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="743c8-137">Request body</span></span>
<span data-ttu-id="743c8-138">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="743c8-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="743c8-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="743c8-139">Response</span></span>

<span data-ttu-id="743c8-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [directoryObject](../resources/directoryobject.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="743c8-140">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="743c8-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="743c8-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="743c8-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="743c8-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
##### <a name="response"></a><span data-ttu-id="743c8-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="743c8-143">Response</span></span>
<span data-ttu-id="743c8-p102">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="743c8-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
  "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
  "displayName":"SampleGroup",
  "groupTypes":["Unified"],
  "mail":"example@contoso.com",
  "mailEnabled":true,
  "mailNickname":"Example",
  "securityEnabled":false,
  "visibility":"Public"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->