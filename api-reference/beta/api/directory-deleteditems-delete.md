---
title: Element endgültig löschen
description: Dauerhaftes Löschen eines Elements aus dem Ordner Gelöschte Elemente.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 048008e31bc5cd7884dd3d7e9259412070404d9d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528200"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="4ee8e-103">Element endgültig löschen</span><span class="sxs-lookup"><span data-stu-id="4ee8e-103">Permanently delete item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ee8e-104">Dauerhaftes Löschen eines Elements aus dem Ordner [Gelöschte Elemente](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="4ee8e-104">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="4ee8e-105">Die Funktion für gelöschte Elemente wird derzeit nur für die Ressourcen [group](../resources/group.md) und [user](../resources/user.md) unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4ee8e-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="4ee8e-106">Sie können ein Element aus den gelöschten Elementen dauerhaft löschen.</span><span class="sxs-lookup"><span data-stu-id="4ee8e-106">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="4ee8e-107">Aber nachdem ein Element dauerhaft gelöscht wurde, **kann es nicht** wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="4ee8e-107">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ee8e-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4ee8e-108">Permissions</span></span>
<span data-ttu-id="4ee8e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ee8e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="4ee8e-111">Für Benutzer: User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4ee8e-111">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="4ee8e-112">Für Gruppen: Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4ee8e-112">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="4ee8e-113">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4ee8e-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deleteditems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4ee8e-114">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4ee8e-114">Request headers</span></span>
| <span data-ttu-id="4ee8e-115">Name</span><span class="sxs-lookup"><span data-stu-id="4ee8e-115">Name</span></span>       | <span data-ttu-id="4ee8e-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4ee8e-116">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4ee8e-117">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4ee8e-117">Authorization</span></span>  | <span data-ttu-id="4ee8e-118">Bearer&lt;code&gt; *erforderlich*</span><span class="sxs-lookup"><span data-stu-id="4ee8e-118">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="4ee8e-119">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4ee8e-119">Accept</span></span>  | <span data-ttu-id="4ee8e-120">application/json</span><span class="sxs-lookup"><span data-stu-id="4ee8e-120">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ee8e-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4ee8e-121">Request body</span></span>
<span data-ttu-id="4ee8e-122">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4ee8e-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ee8e-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="4ee8e-123">Response</span></span>

<span data-ttu-id="4ee8e-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4ee8e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ee8e-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4ee8e-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ee8e-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4ee8e-127">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
##### <a name="response"></a><span data-ttu-id="4ee8e-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="4ee8e-128">Response</span></span>
<span data-ttu-id="4ee8e-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4ee8e-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directory-deleteditems-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
