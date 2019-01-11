---
title: Gelöschte Elemente auflisten
description: Abrufen einer Liste kürzlich gelöschter Elemente aus den gelöschten Elementen.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: ef23704c01a7d1b6cd3a85ffcab1dc34ded0936d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879436"
---
# <a name="list-deleted-items"></a><span data-ttu-id="09826-103">Gelöschte Elemente auflisten</span><span class="sxs-lookup"><span data-stu-id="09826-103">List deleted items</span></span>

> <span data-ttu-id="09826-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="09826-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="09826-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="09826-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="09826-106">Abrufen einer Liste kürzlich gelöschter Elemente aus den [gelöschten Elementen](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="09826-106">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="09826-107">Die Funktion für gelöschte Elemente wird derzeit nur für die Ressourcen [group](../resources/group.md) und [user](../resources/user.md) unterstützt.</span><span class="sxs-lookup"><span data-stu-id="09826-107">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="09826-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="09826-108">Permissions</span></span>
<span data-ttu-id="09826-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09826-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="09826-111">Für Benutzer: User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="09826-111">For users: User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="09826-112">Für Gruppen: Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="09826-112">For groups: Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="09826-113">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="09826-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="09826-114">Diese API unterstützt derzeit das Abrufen von Objekttypen von Gruppen (microsoft.graph.group) oder Benutzern (microsoft.graph.user) aus den gelöschten Elementen.</span><span class="sxs-lookup"><span data-stu-id="09826-114">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="09826-115">Der Typ wird als ein erforderlicher Bestandteil der URI angegeben.</span><span class="sxs-lookup"><span data-stu-id="09826-115">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="09826-116">Das Aufrufen von GET/Verzeichnis/deleteditems ohne Typ wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="09826-116">Calling GET /directory/deleteditems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="09826-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="09826-117">Optional query parameters</span></span>
<span data-ttu-id="09826-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="09826-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="09826-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="09826-119">Request headers</span></span>
| <span data-ttu-id="09826-120">Name</span><span class="sxs-lookup"><span data-stu-id="09826-120">Name</span></span>      |<span data-ttu-id="09826-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="09826-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="09826-122">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="09826-122">Authorization</span></span>  | <span data-ttu-id="09826-123">Bearer&lt;code&gt; *erforderlich*</span><span class="sxs-lookup"><span data-stu-id="09826-123">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="09826-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="09826-124">Accept</span></span>  | <span data-ttu-id="09826-125">application/json</span><span class="sxs-lookup"><span data-stu-id="09826-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="09826-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="09826-126">Request body</span></span>
<span data-ttu-id="09826-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="09826-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09826-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="09826-128">Response</span></span>

<span data-ttu-id="09826-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="09826-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="09826-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="09826-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="09826-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="09826-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```http
GET https://graph.microsoft.com/beta/directory/deleteditems/microsoft.graph.group
```
##### <a name="response"></a><span data-ttu-id="09826-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="09826-132">Response</span></span>
<span data-ttu-id="09826-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="09826-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
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
