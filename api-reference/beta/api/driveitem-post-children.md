---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Einen neuen Ordner erstellen
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a81d8fe2c7511b4fe971ccdf114883088bea65b3
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482322"
---
# <a name="create-a-new-folder-in-a-drive"></a><span data-ttu-id="03599-102">Neuen Ordner in OneDrive erstellen</span><span class="sxs-lookup"><span data-stu-id="03599-102">Create a new folder in a drive</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03599-103">Mit dieser API können Sie einen neuen Ordner oder eine neue Ressource des Typs [DriveItem](../resources/driveitem.md) in der Ressource des Typs [Drive](../resources/drive.md) mit dem jeweils angegebenen übergeordneten Element oder Pfad erstellen.</span><span class="sxs-lookup"><span data-stu-id="03599-103">Create a new folder or [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) with a specified parent item or path.</span></span>

## <a name="permissions"></a><span data-ttu-id="03599-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="03599-104">Permissions</span></span>

<span data-ttu-id="03599-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03599-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03599-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="03599-107">Permission type</span></span>      | <span data-ttu-id="03599-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="03599-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03599-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="03599-109">Delegated (work or school account)</span></span> | <span data-ttu-id="03599-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03599-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="03599-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="03599-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03599-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03599-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="03599-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="03599-113">Application</span></span> | <span data-ttu-id="03599-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03599-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="03599-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="03599-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{parent-item-id}/children
POST /groups/{group-id}/drive/items/{parent-item-id}/children
POST /me/drive/items/{parent-item-id}/children
POST /sites/{site-id}/drive/items/{parent-item-id}/children
POST /users/{user-id}/drive/items/{parent-item-id}/children
```

## <a name="request-body"></a><span data-ttu-id="03599-116">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="03599-116">Request body</span></span>

<span data-ttu-id="03599-117">Geben Sie im Anforderungstext eine JSON-Darstellung der zu erstellenden [DriveItem](../resources/driveitem.md)-Ressource an.</span><span class="sxs-lookup"><span data-stu-id="03599-117">In the request body, supply a JSON representation of the [DriveItem](../resources/driveitem.md) resource to create.</span></span>

## <a name="response"></a><span data-ttu-id="03599-118">Antwort</span><span class="sxs-lookup"><span data-stu-id="03599-118">Response</span></span>

<span data-ttu-id="03599-119">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und die [DriveItem](../resources/driveitem.md)-Ressource im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="03599-119">If successful, this method returns `201 Created` response code and a [Driveitem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03599-120">Beispiel</span><span class="sxs-lookup"><span data-stu-id="03599-120">Example</span></span>

### <a name="request"></a><span data-ttu-id="03599-121">Anforderung</span><span class="sxs-lookup"><span data-stu-id="03599-121">Request</span></span>

<span data-ttu-id="03599-122">Nachfolgend finden Sie ein Beispiel der Anforderung zum Erstellen eines neues Ordners am OneDrive-Stammordner des angemeldeten Benutzers.</span><span class="sxs-lookup"><span data-stu-id="03599-122">Here is an example of the request to create a new folder in the signed-in user's OneDrive root folder.</span></span>
<span data-ttu-id="03599-123">Die verwendete `@microsoft.graph.conflictBehavior`-Eigenschaft zeigt an, wenn ein Element bereits mit dem gleichen Namen vorhanden ist. Der Dienst sollte bei der Erstellung einen neuen Namen für den Ordner auswählen.</span><span class="sxs-lookup"><span data-stu-id="03599-123">The `@microsoft.graph.conflictBehavior` property used indicates that if an item already exists with the same name, the service should choose a new name for the folder while creating it.</span></span>

<!-- { "blockType": "request", "name": "create-folder", "scopes": "files.readwrite" } -->

```http
POST /me/drive/root/children
Content-Type: application/json

{
  "name": "New Folder",
  "folder": { },
  "@microsoft.graph.conflictBehavior": "rename"
}
```

### <a name="response"></a><span data-ttu-id="03599-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="03599-124">Response</span></span>

<span data-ttu-id="03599-125">Wenn die Methode erfolgreich verläuft, wird der neu erstelle Ordner als [DriveItem][item-resource]-Ressource zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="03599-125">If successful, this method returns the newly created folder as a [DriveItem][item-resource] resource.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "createdBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "309EC495-3E92-431D-9124-F0299633171D"
    }
  },
  "createdDateTime": "2016-09-20T14:34:00Z",
  "eTag": "343F1FBD-E9B3-4DDE-BCA7-D61AEAFF44E5,1",
  "id": "ACEA49D1-1444-45A9-A1CB-68B1B28AE491",
  "lastModifiedBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "309EC495-3E92-431D-9124-F0299633171D"
    }
  },
  "lastModifiedDateTime": "2016-09-20T14:34:00Z",
  "name": "New Folder",
  "parentReference": {
    "driveId": "5FE38E3C-051C-4D55-9B83-8A437658275B",
    "id": "E67A8F34-B0AA-46E1-8FF7-0750A29553DF",
    "path": "/drive/root:/"
  },
  "size": 0,
  "folder": {
    "childCount": 0
  }
}
```

## <a name="error-response"></a><span data-ttu-id="03599-126">Fehlerantwort</span><span class="sxs-lookup"><span data-stu-id="03599-126">Error response</span></span>

<span data-ttu-id="03599-127">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie unter [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="03599-127">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md
[folder-facet]: ../resources/folder.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a folder item in a drive.",
  "keywords": "create,folder,new item",
  "section": "documentation",
  "tocPath": "Items/Create folder",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-post-children.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
