---
title: Gelöschtes Element abrufen
description: Abrufen der Eigenschaften eines kürzlich gelöschten Elements aus den gelöschten Elementen.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 09996c27aec0183ded5b09b490c95fb95d57893a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926428"
---
# <a name="get-deleted-item"></a><span data-ttu-id="f0f28-103">Gelöschtes Element abrufen</span><span class="sxs-lookup"><span data-stu-id="f0f28-103">Get deleted item</span></span>

> <span data-ttu-id="f0f28-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f0f28-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0f28-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f0f28-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f0f28-106">Abrufen der Eigenschaften eines kürzlich gelöschten Elements aus den [gelöschten Elementen](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="f0f28-106">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="f0f28-107">Die Funktion für gelöschte Elemente wird derzeit nur für die Ressourcen [group](../resources/group.md) und [user](../resources/user.md) unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f0f28-107">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0f28-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f0f28-108">Permissions</span></span>
<span data-ttu-id="f0f28-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0f28-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="f0f28-111">Für Benutzer: User.Read.All, User.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0f28-111">For users: User.Read.All, User.ReadWrite.All, Directory.Read.All</span></span>
* <span data-ttu-id="f0f28-112">Für Gruppen: Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0f28-112">For groups: Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span>

## <a name="http-request"></a><span data-ttu-id="f0f28-113">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f0f28-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deleteditems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f0f28-114">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f0f28-114">Optional query parameters</span></span>
<span data-ttu-id="f0f28-115">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f0f28-115">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f0f28-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f0f28-116">Request headers</span></span>
| <span data-ttu-id="f0f28-117">Name</span><span class="sxs-lookup"><span data-stu-id="f0f28-117">Name</span></span>      |<span data-ttu-id="f0f28-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f0f28-118">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f0f28-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f0f28-119">Authorization</span></span>  | <span data-ttu-id="f0f28-120">Bearer&lt;code&gt; *erforderlich*</span><span class="sxs-lookup"><span data-stu-id="f0f28-120">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="f0f28-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f0f28-121">Accept</span></span>  | <span data-ttu-id="f0f28-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f0f28-122">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0f28-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f0f28-123">Request body</span></span>
<span data-ttu-id="f0f28-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f0f28-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0f28-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="f0f28-125">Response</span></span>

<span data-ttu-id="f0f28-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [directoryObject](../resources/directoryobject.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f0f28-126">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f0f28-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f0f28-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f0f28-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f0f28-128">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
##### <a name="response"></a><span data-ttu-id="f0f28-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f0f28-129">Response</span></span>
<span data-ttu-id="f0f28-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f0f28-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
