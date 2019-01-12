---
title: Gelöschtes Element wiederherstellen
description: 'Stellt ein kürzlich gelöschtes Element aus den gelöschten Elementen wieder her. '
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8c9a6e84a723fc0087f3155e4b2e973e72276233
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935969"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="5bd8a-103">Gelöschtes Element wiederherstellen</span><span class="sxs-lookup"><span data-stu-id="5bd8a-103">Restore deleted item</span></span>

> <span data-ttu-id="5bd8a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5bd8a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5bd8a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5bd8a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5bd8a-106">Stellt ein kürzlich gelöschtes Element aus den [gelöschten Elementen](../resources/directory.md) wieder her.</span><span class="sxs-lookup"><span data-stu-id="5bd8a-106">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="5bd8a-107">Die Funktion für gelöschte Elemente wird derzeit nur für die Ressourcen [group](../resources/group.md) und [user](../resources/user.md) unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5bd8a-107">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="5bd8a-108">Wenn ein Element versehentlich gelöscht wurde, können es vollständig wiederherstellen.</span><span class="sxs-lookup"><span data-stu-id="5bd8a-108">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="5bd8a-109">Ein kürzlich gelöschtes Element bleibt bis zu 30 Tage verfügbar.</span><span class="sxs-lookup"><span data-stu-id="5bd8a-109">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="5bd8a-110">Nach 30 Tagen wird das Element dauerhaft gelöscht.</span><span class="sxs-lookup"><span data-stu-id="5bd8a-110">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="5bd8a-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5bd8a-111">Permissions</span></span>
<span data-ttu-id="5bd8a-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bd8a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="5bd8a-114">Für Benutzer: User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5bd8a-114">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="5bd8a-115">Für Gruppen: Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5bd8a-115">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="5bd8a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5bd8a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deleteditems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="5bd8a-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5bd8a-117">Request headers</span></span>
| <span data-ttu-id="5bd8a-118">Name</span><span class="sxs-lookup"><span data-stu-id="5bd8a-118">Name</span></span>       | <span data-ttu-id="5bd8a-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5bd8a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5bd8a-120">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="5bd8a-120">Authorization</span></span>  | <span data-ttu-id="5bd8a-121">Bearer&lt;code&gt; *erforderlich*</span><span class="sxs-lookup"><span data-stu-id="5bd8a-121">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="5bd8a-122">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5bd8a-122">Accept</span></span> | <span data-ttu-id="5bd8a-123">application/json</span><span class="sxs-lookup"><span data-stu-id="5bd8a-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5bd8a-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5bd8a-124">Request body</span></span>
<span data-ttu-id="5bd8a-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5bd8a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bd8a-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="5bd8a-126">Response</span></span>

<span data-ttu-id="5bd8a-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [directoryObject](../resources/directoryobject.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5bd8a-127">If successful, this method returns `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bd8a-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5bd8a-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5bd8a-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5bd8a-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb/restore
```
<span data-ttu-id="5bd8a-130">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryObject](../resources/directoryobject.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="5bd8a-130">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="5bd8a-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="5bd8a-131">Response</span></span>
<span data-ttu-id="5bd8a-p105">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5bd8a-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create deletedItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
