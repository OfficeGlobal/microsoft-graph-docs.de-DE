---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Verschieben einer Datei oder eines Ordners
ms.openlocfilehash: ebffe8451c6cf5ce7f025b70225054cfb8080cf6
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="move-a-driveitem-to-a-new-folder"></a><span data-ttu-id="4b26c-102">Ein DriveItem in einen neuen Ordner verschieben</span><span class="sxs-lookup"><span data-stu-id="4b26c-102">Move a DriveItem to a new folder</span></span>

<span data-ttu-id="4b26c-103">Zum Verschieben eines DriveItem-Elements zu einem neuen übergeordneten Element fordert die App die Aktualisierung von **ParentReference** des zu verschiebenden DriveItem-Elements an.</span><span class="sxs-lookup"><span data-stu-id="4b26c-103">To move a DriveItem to a new parent item, your app requests to update the **parentReference** of the DriveItem to move.</span></span>

<span data-ttu-id="4b26c-104">Dies ist ein Sonderfall der [Update](driveitem_update.md)-Methode.</span><span class="sxs-lookup"><span data-stu-id="4b26c-104">This is a special case of the [update](driveitem_update.md) method.</span></span>
<span data-ttu-id="4b26c-105">Die App kann das Verschieben eines Elements zu einem neuen Container und das Aktualisieren anderer Eigenschaften des Elements in einer einzigen Anforderung verbinden.</span><span class="sxs-lookup"><span data-stu-id="4b26c-105">To move a DriveItem to a new parent item, your app requests to update the parentReference of the DriveItem to move. This is a special case of the Update method. Your app can combine moving an item to a new container and updating other properties of the item into a single request.</span></span>

<span data-ttu-id="4b26c-106">Elemente können mit dieser Anforderung nicht zwischen verschiedenen Ressourcen des Typs [Drive](../resources/drive.md) verschoben werden.</span><span class="sxs-lookup"><span data-stu-id="4b26c-106">Items cannot be moved between [Drives](../resources/drive.md) using this request.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b26c-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4b26c-107">Permissions</span></span>
<span data-ttu-id="4b26c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4b26c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4b26c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4b26c-110">Permission type</span></span>      | <span data-ttu-id="4b26c-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4b26c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b26c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4b26c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4b26c-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b26c-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4b26c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4b26c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b26c-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b26c-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="4b26c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4b26c-116">Application</span></span> | <span data-ttu-id="4b26c-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b26c-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b26c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b26c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="4b26c-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4b26c-119">Optional request headers</span></span>

| <span data-ttu-id="4b26c-120">Name</span><span class="sxs-lookup"><span data-stu-id="4b26c-120">Name</span></span>          | <span data-ttu-id="4b26c-121">Typ</span><span class="sxs-lookup"><span data-stu-id="4b26c-121">Type</span></span>   | <span data-ttu-id="4b26c-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4b26c-122">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4b26c-123">if-match</span><span class="sxs-lookup"><span data-stu-id="4b26c-123">if-match</span></span>      | <span data-ttu-id="4b26c-124">String</span><span class="sxs-lookup"><span data-stu-id="4b26c-124">String</span></span> | <span data-ttu-id="4b26c-125">Wenn dieser Anforderungsheader enthalten ist und das angegebene etag (oder cTag) nicht mit dem aktuellen etag des Ordners übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4b26c-125">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b26c-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4b26c-126">Request body</span></span>

<span data-ttu-id="4b26c-p103">Geben Sie im Anforderungstext den neuen Wert für die **parentReference**-Eigenschaft an. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="4b26c-p103">In the request body, supply the new value for the **parentReference** property. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

<span data-ttu-id="4b26c-130">**Hinweis:** Ihre App kann die `"id:" "root"`-Syntax beim Verschieben von Elementen in den Stammordner eines Laufwerks nicht verwenden.</span><span class="sxs-lookup"><span data-stu-id="4b26c-130">**Note:** When moving items to the root of a drive your app cannot use the `"id:" "root"` syntax.</span></span>
<span data-ttu-id="4b26c-131">Ihre App muss die tatsächliche ID des Stammordners für den übergeordneten Verweis bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="4b26c-131">Your app needs to provide the actual ID of the root folder for the parent reference.</span></span>

## <a name="response"></a><span data-ttu-id="4b26c-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b26c-132">Response</span></span>

<span data-ttu-id="4b26c-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und die aktualisierte [DriveItem](../resources/driveitem.md)-Ressource im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4b26c-133">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b26c-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4b26c-134">Example</span></span>

<span data-ttu-id="4b26c-135">In diesem Beispiel wird ein durch {item-id} angegebenes Element mit der ID `new-parent-folder-id` auf das Laufwerk des Benutzers verschoben.</span><span class="sxs-lookup"><span data-stu-id="4b26c-135">This example moves an item specified by {item-id} into the `new-parent-folder-id` folder in the user's OneDrive.</span></span>

<!-- { "blockType": "request", "name": "move-item", "scopes": "files.readwrite" } -->

```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
  "parentReference": {
    "id": "new-parent-folder-id"
  },
  "name": "new-item-name.txt"
}
```

### <a name="response"></a><span data-ttu-id="4b26c-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b26c-136">Response</span></span>

<span data-ttu-id="4b26c-137">Das folgende Beispiel zeigt die Antwort für diese Verschiebungsanforderung.</span><span class="sxs-lookup"><span data-stu-id="4b26c-137">The following example shows the response for this move request.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0123456789abc",
  "name": "new-item-name.txt",
  "parentReference":
  {
    "driveId": "11231001",
    "path": "/drive/root:/Documents",
    "id": "1231203102!1011"
  }
}
```

## <a name="error-responses"></a><span data-ttu-id="4b26c-138">Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="4b26c-138">Error responses</span></span>

<span data-ttu-id="4b26c-139">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie unter [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="4b26c-139">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: ../../../concepts/errors.md

<!-- {
  "type": "#page.annotation",
  "description": "Move an item to another location or rename the item.",
  "keywords": "move,rename,mv,change location",
  "section": "documentation",
  "tocPath": "Items/Move"
} -->
