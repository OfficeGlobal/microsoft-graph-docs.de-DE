---
title: Gelöschtes Element abrufen
description: Abrufen der Eigenschaften eines kürzlich gelöschten Elements aus den gelöschten Elementen.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d77161c19807ab99b3c9c8771ea910d1d6e90e42
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514453"
---
# <a name="get-deleted-item"></a><span data-ttu-id="1e55e-103">Gelöschtes Element abrufen</span><span class="sxs-lookup"><span data-stu-id="1e55e-103">Get deleted item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e55e-104">Abrufen der Eigenschaften eines kürzlich gelöschten Elements aus den [gelöschten Elementen](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="1e55e-104">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="1e55e-105">Die Funktion für gelöschte Elemente wird derzeit nur für die Ressourcen [group](../resources/group.md) und [user](../resources/user.md) unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1e55e-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e55e-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1e55e-106">Permissions</span></span>
<span data-ttu-id="1e55e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e55e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="1e55e-109">Für Benutzer: User.Read.All, User.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e55e-109">For users: User.Read.All, User.ReadWrite.All, Directory.Read.All</span></span>
* <span data-ttu-id="1e55e-110">Für Gruppen: Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e55e-110">For groups: Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span>

## <a name="http-request"></a><span data-ttu-id="1e55e-111">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1e55e-111">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deleteditems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1e55e-112">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1e55e-112">Optional query parameters</span></span>
<span data-ttu-id="1e55e-113">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1e55e-113">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1e55e-114">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1e55e-114">Request headers</span></span>
| <span data-ttu-id="1e55e-115">Name</span><span class="sxs-lookup"><span data-stu-id="1e55e-115">Name</span></span>      |<span data-ttu-id="1e55e-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1e55e-116">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1e55e-117">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1e55e-117">Authorization</span></span>  | <span data-ttu-id="1e55e-118">Bearer&lt;code&gt; *erforderlich*</span><span class="sxs-lookup"><span data-stu-id="1e55e-118">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="1e55e-119">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1e55e-119">Accept</span></span>  | <span data-ttu-id="1e55e-120">application/json</span><span class="sxs-lookup"><span data-stu-id="1e55e-120">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e55e-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1e55e-121">Request body</span></span>
<span data-ttu-id="1e55e-122">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1e55e-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e55e-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="1e55e-123">Response</span></span>

<span data-ttu-id="1e55e-124">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [directoryObject](../resources/directoryobject.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1e55e-124">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1e55e-125">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1e55e-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1e55e-126">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1e55e-126">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
##### <a name="response"></a><span data-ttu-id="1e55e-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="1e55e-127">Response</span></span>
<span data-ttu-id="1e55e-p102">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1e55e-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directory"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects/$entity",
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
<!--
{
  "type": "#page.annotation",
  "description": "Get directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directory-deleteditems-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
