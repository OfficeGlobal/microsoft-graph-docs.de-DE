---
title: Element endgültig löschen
description: Dauerhaftes Löschen eines Elements aus dem Ordner Gelöschte Elemente.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e8a63418736e9a534ef9ab0279bd9d5472f60af7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926617"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="884fb-103">Element endgültig löschen</span><span class="sxs-lookup"><span data-stu-id="884fb-103">Permanently delete item</span></span>

> <span data-ttu-id="884fb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="884fb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="884fb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="884fb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="884fb-106">Dauerhaftes Löschen eines Elements aus dem Ordner [Gelöschte Elemente](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="884fb-106">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="884fb-107">Die Funktion für gelöschte Elemente wird derzeit nur für die Ressourcen [group](../resources/group.md) und [user](../resources/user.md) unterstützt.</span><span class="sxs-lookup"><span data-stu-id="884fb-107">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="884fb-108">Sie können ein Element aus den gelöschten Elementen dauerhaft löschen.</span><span class="sxs-lookup"><span data-stu-id="884fb-108">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="884fb-109">Aber nachdem ein Element dauerhaft gelöscht wurde, **kann es nicht** wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="884fb-109">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="884fb-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="884fb-110">Permissions</span></span>
<span data-ttu-id="884fb-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="884fb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="884fb-113">Für Benutzer: User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="884fb-113">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="884fb-114">Für Gruppen: Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="884fb-114">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="884fb-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="884fb-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deleteditems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="884fb-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="884fb-116">Request headers</span></span>
| <span data-ttu-id="884fb-117">Name</span><span class="sxs-lookup"><span data-stu-id="884fb-117">Name</span></span>       | <span data-ttu-id="884fb-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="884fb-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="884fb-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="884fb-119">Authorization</span></span>  | <span data-ttu-id="884fb-120">Bearer&lt;code&gt; *erforderlich*</span><span class="sxs-lookup"><span data-stu-id="884fb-120">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="884fb-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="884fb-121">Accept</span></span>  | <span data-ttu-id="884fb-122">application/json</span><span class="sxs-lookup"><span data-stu-id="884fb-122">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="884fb-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="884fb-123">Request body</span></span>
<span data-ttu-id="884fb-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="884fb-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="884fb-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="884fb-125">Response</span></span>

<span data-ttu-id="884fb-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="884fb-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="884fb-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="884fb-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="884fb-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="884fb-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
##### <a name="response"></a><span data-ttu-id="884fb-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="884fb-130">Response</span></span>
<span data-ttu-id="884fb-p105">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="884fb-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
