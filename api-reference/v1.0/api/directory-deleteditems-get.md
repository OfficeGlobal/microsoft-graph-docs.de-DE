---
title: Gelöschtes Element abrufen
description: Abrufen der Eigenschaften eines kürzlich gelöschten Elements aus den gelöschten Elementen.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: de025535058c8b796b591b5bcac2f91f4d3397e3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932329"
---
# <a name="get-deleted-item"></a><span data-ttu-id="51ec3-103">Gelöschtes Element abrufen</span><span class="sxs-lookup"><span data-stu-id="51ec3-103">Get deleted item</span></span>

<span data-ttu-id="51ec3-104">Abrufen der Eigenschaften eines kürzlich gelöschten Elements aus den [gelöschten Elementen](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="51ec3-104">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="51ec3-105">Die Funktion für gelöschte Elemente wird derzeit nur für die Ressourcen [group](../resources/group.md) und [user](../resources/user.md) unterstützt.</span><span class="sxs-lookup"><span data-stu-id="51ec3-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="51ec3-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="51ec3-106">Permissions</span></span>
<span data-ttu-id="51ec3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51ec3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="51ec3-109">Für Benutzer:</span><span class="sxs-lookup"><span data-stu-id="51ec3-109">For users:</span></span>

|<span data-ttu-id="51ec3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="51ec3-110">Permission type</span></span>      | <span data-ttu-id="51ec3-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="51ec3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51ec3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="51ec3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="51ec3-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="51ec3-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span></span> |
|<span data-ttu-id="51ec3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="51ec3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51ec3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="51ec3-115">Not supported.</span></span> |
|<span data-ttu-id="51ec3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="51ec3-116">Application</span></span> | <span data-ttu-id="51ec3-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51ec3-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="51ec3-118">Für Gruppen:</span><span class="sxs-lookup"><span data-stu-id="51ec3-118">For groups:</span></span>

|<span data-ttu-id="51ec3-119">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="51ec3-119">Permission type</span></span>      | <span data-ttu-id="51ec3-120">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="51ec3-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51ec3-121">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="51ec3-121">Delegated (work or school account)</span></span> | <span data-ttu-id="51ec3-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="51ec3-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="51ec3-123">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="51ec3-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51ec3-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="51ec3-124">Not supported.</span></span>    |
|<span data-ttu-id="51ec3-125">Anwendung</span><span class="sxs-lookup"><span data-stu-id="51ec3-125">Application</span></span> | <span data-ttu-id="51ec3-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51ec3-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="51ec3-127">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="51ec3-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deletedItems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51ec3-128">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="51ec3-128">Optional query parameters</span></span>
<span data-ttu-id="51ec3-129">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="51ec3-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="51ec3-130">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="51ec3-130">Request headers</span></span>
| <span data-ttu-id="51ec3-131">Name</span><span class="sxs-lookup"><span data-stu-id="51ec3-131">Name</span></span>      |<span data-ttu-id="51ec3-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="51ec3-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="51ec3-133">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="51ec3-133">Authorization</span></span>  | <span data-ttu-id="51ec3-134">Bearer&lt;code&gt; *erforderlich*</span><span class="sxs-lookup"><span data-stu-id="51ec3-134">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="51ec3-135">Annehmen</span><span class="sxs-lookup"><span data-stu-id="51ec3-135">Accept</span></span>  | <span data-ttu-id="51ec3-136">application/json</span><span class="sxs-lookup"><span data-stu-id="51ec3-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="51ec3-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="51ec3-137">Request body</span></span>
<span data-ttu-id="51ec3-138">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="51ec3-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51ec3-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="51ec3-139">Response</span></span>

<span data-ttu-id="51ec3-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [directoryObject](../resources/directoryobject.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="51ec3-140">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="51ec3-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="51ec3-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="51ec3-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="51ec3-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
##### <a name="response"></a><span data-ttu-id="51ec3-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="51ec3-143">Response</span></span>
<span data-ttu-id="51ec3-p102">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="51ec3-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
