---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Einen neuen Ordner erstellen
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 0bdd5f76303d5097af3edd1fd9e2a8469d4a47a2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984619"
---
# <a name="create-a-new-folder-in-a-drive"></a><span data-ttu-id="e4480-102">Neuen Ordner in OneDrive erstellen</span><span class="sxs-lookup"><span data-stu-id="e4480-102">Create a new folder in a drive</span></span>

> <span data-ttu-id="e4480-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e4480-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4480-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e4480-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e4480-105">Mit dieser API können Sie einen neuen Ordner oder eine neue Ressource des Typs [DriveItem](../resources/driveitem.md) in der Ressource des Typs [Drive](../resources/drive.md) mit dem jeweils angegebenen übergeordneten Element oder Pfad erstellen.</span><span class="sxs-lookup"><span data-stu-id="e4480-105">Create a new folder or [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) with a specified parent item or path.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4480-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e4480-106">Permissions</span></span>

<span data-ttu-id="e4480-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4480-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4480-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e4480-109">Permission type</span></span>      | <span data-ttu-id="e4480-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e4480-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4480-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e4480-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e4480-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4480-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e4480-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e4480-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4480-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4480-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e4480-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e4480-115">Application</span></span> | <span data-ttu-id="e4480-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4480-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4480-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4480-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{parent-item-id}/children
POST /groups/{group-id}/drive/items/{parent-item-id}/children
POST /me/drive/items/{parent-item-id}/children
POST /sites/{site-id}/drive/items/{parent-item-id}/children
POST /users/{user-id}/drive/items/{parent-item-id}/children
```

## <a name="request-body"></a><span data-ttu-id="e4480-118">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e4480-118">Request body</span></span>

<span data-ttu-id="e4480-119">Geben Sie im Anforderungstext eine JSON-Darstellung der zu erstellenden [DriveItem](../resources/driveitem.md)-Ressource an.</span><span class="sxs-lookup"><span data-stu-id="e4480-119">In the request body, supply a JSON representation of the [DriveItem](../resources/driveitem.md) resource to create.</span></span>

## <a name="response"></a><span data-ttu-id="e4480-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4480-120">Response</span></span>

<span data-ttu-id="e4480-121">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und die [DriveItem](../resources/driveitem.md)-Ressource im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e4480-121">If successful, this method returns `201 Created` response code and a [Driveitem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4480-122">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e4480-122">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4480-123">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4480-123">Request</span></span>

<span data-ttu-id="e4480-124">Nachfolgend finden Sie ein Beispiel der Anforderung zum Erstellen eines neues Ordners am OneDrive-Stammordner des angemeldeten Benutzers.</span><span class="sxs-lookup"><span data-stu-id="e4480-124">Here is an example of the request to create a new folder in the signed-in user's OneDrive root folder.</span></span>
<span data-ttu-id="e4480-125">Die verwendete `@microsoft.graph.conflictBehavior`-Eigenschaft zeigt an, wenn ein Element bereits mit dem gleichen Namen vorhanden ist. Der Dienst sollte bei der Erstellung einen neuen Namen für den Ordner auswählen.</span><span class="sxs-lookup"><span data-stu-id="e4480-125">The `@microsoft.graph.conflictBehavior` property used indicates that if an item already exists with the same name, the service should choose a new name for the folder while creating it.</span></span>

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

### <a name="response"></a><span data-ttu-id="e4480-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4480-126">Response</span></span>

<span data-ttu-id="e4480-127">Wenn die Methode erfolgreich verläuft, wird der neu erstelle Ordner als [DriveItem][item-resource]- zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e4480-127">If successful, this method returns the newly created folder as a [DriveItem][item-resource] resource.</span></span>

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

## <a name="error-response"></a><span data-ttu-id="e4480-128">Fehlerantwort</span><span class="sxs-lookup"><span data-stu-id="e4480-128">Error response</span></span>

<span data-ttu-id="e4480-129">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie im Artikel zum Thema [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="e4480-129">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>
[Fehlerantwort]: / Diagramm/Fehler [Element-Ressource]:... /Resources/driveitem.MD [Ordner Facetten]:... /Resources/Folder.MD
[error-response]: /graph/errors [item-resource]: ../resources/driveitem.md [folder-facet]: ../resources/folder.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a folder item in a drive.",
  "keywords": "create,folder,new item",
  "section": "documentation",
  "tocPath": "Items/Create folder"
} -->
