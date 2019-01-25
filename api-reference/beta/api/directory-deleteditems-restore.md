---
title: Gelöschtes Element wiederherstellen
description: 'Stellt ein kürzlich gelöschtes Element aus den gelöschten Elementen wieder her. '
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 42af211afb9f508e9033f3e77f2b1dd14aa484d7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520732"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="b75a9-103">Gelöschtes Element wiederherstellen</span><span class="sxs-lookup"><span data-stu-id="b75a9-103">Restore deleted item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b75a9-104">Stellt ein kürzlich gelöschtes Element aus den [gelöschten Elementen](../resources/directory.md) wieder her.</span><span class="sxs-lookup"><span data-stu-id="b75a9-104">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="b75a9-105">Die Funktion für gelöschte Elemente wird derzeit nur für die Ressourcen [group](../resources/group.md) und [user](../resources/user.md) unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b75a9-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="b75a9-106">Wenn ein Element versehentlich gelöscht wurde, können es vollständig wiederherstellen.</span><span class="sxs-lookup"><span data-stu-id="b75a9-106">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="b75a9-107">Ein kürzlich gelöschtes Element bleibt bis zu 30 Tage verfügbar.</span><span class="sxs-lookup"><span data-stu-id="b75a9-107">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="b75a9-108">Nach 30 Tagen wird das Element dauerhaft gelöscht.</span><span class="sxs-lookup"><span data-stu-id="b75a9-108">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="b75a9-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b75a9-109">Permissions</span></span>
<span data-ttu-id="b75a9-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b75a9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="b75a9-112">Für Benutzer: User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b75a9-112">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="b75a9-113">Für Gruppen: Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b75a9-113">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="b75a9-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b75a9-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deleteditems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="b75a9-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b75a9-115">Request headers</span></span>
| <span data-ttu-id="b75a9-116">Name</span><span class="sxs-lookup"><span data-stu-id="b75a9-116">Name</span></span>       | <span data-ttu-id="b75a9-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b75a9-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b75a9-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b75a9-118">Authorization</span></span>  | <span data-ttu-id="b75a9-119">Bearer&lt;code&gt; *erforderlich*</span><span class="sxs-lookup"><span data-stu-id="b75a9-119">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="b75a9-120">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b75a9-120">Accept</span></span> | <span data-ttu-id="b75a9-121">application/json</span><span class="sxs-lookup"><span data-stu-id="b75a9-121">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b75a9-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b75a9-122">Request body</span></span>
<span data-ttu-id="b75a9-123">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b75a9-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b75a9-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="b75a9-124">Response</span></span>

<span data-ttu-id="b75a9-125">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [directoryObject](../resources/directoryobject.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b75a9-125">If successful, this method returns `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b75a9-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b75a9-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b75a9-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b75a9-127">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb/restore
```
<span data-ttu-id="b75a9-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryObject](../resources/directoryobject.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="b75a9-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b75a9-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="b75a9-129">Response</span></span>
<span data-ttu-id="b75a9-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b75a9-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects/$entity",
  "@odata.type":"#microsoft.graph.group",
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
  "description": "Create deletedItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directory-deleteditems-restore.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
