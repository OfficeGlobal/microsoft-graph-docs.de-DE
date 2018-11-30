---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Verschieben einer Datei oder eines Ordners
ms.openlocfilehash: 4fdf9b079068f3a07a74f117c3e3ad6798a2cd1f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060889"
---
# <a name="move-a-driveitem-to-a-new-folder"></a><span data-ttu-id="7b14e-102">Ein DriveItem in einen neuen Ordner verschieben</span><span class="sxs-lookup"><span data-stu-id="7b14e-102">Move a DriveItem to a new folder</span></span>

> <span data-ttu-id="7b14e-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7b14e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b14e-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7b14e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7b14e-105">Zum Verschieben eines DriveItem-Elements zu einem neuen übergeordneten Element fordert die App die Aktualisierung von **ParentReference** des zu verschiebenden DriveItem-Elements an.</span><span class="sxs-lookup"><span data-stu-id="7b14e-105">To move a DriveItem to a new parent item, your app requests to update the **parentReference** of the DriveItem to move.</span></span>

<span data-ttu-id="7b14e-106">Dies ist ein Sonderfall der [Update](driveitem-update.md)-Methode.</span><span class="sxs-lookup"><span data-stu-id="7b14e-106">This is a special case of the [Update](driveitem-update.md) method.</span></span>
<span data-ttu-id="7b14e-107">Die App kann das Verschieben eines Elements zu einem neuen Container und das Aktualisieren anderer Eigenschaften des Elements in einer einzigen Anforderung verbinden.</span><span class="sxs-lookup"><span data-stu-id="7b14e-107">Your app can combine moving an item to a new container and updating other properties of the item into a single request.</span></span>

<span data-ttu-id="7b14e-108">Elemente können mit dieser Anforderung nicht zwischen verschiedenen Ressourcen des Typs [Drive](../resources/drive.md) verschoben werden.</span><span class="sxs-lookup"><span data-stu-id="7b14e-108">Items cannot be moved between [Drives](../resources/drive.md) using this request.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b14e-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7b14e-109">Permissions</span></span>
<span data-ttu-id="7b14e-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b14e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b14e-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7b14e-112">Permission type</span></span>      | <span data-ttu-id="7b14e-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7b14e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b14e-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7b14e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7b14e-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b14e-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7b14e-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7b14e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b14e-117">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b14e-117">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="7b14e-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7b14e-118">Application</span></span> | <span data-ttu-id="7b14e-119">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b14e-119">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b14e-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b14e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="7b14e-121">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7b14e-121">Optional request headers</span></span>

| <span data-ttu-id="7b14e-122">Name</span><span class="sxs-lookup"><span data-stu-id="7b14e-122">Name</span></span>          | <span data-ttu-id="7b14e-123">Typ</span><span class="sxs-lookup"><span data-stu-id="7b14e-123">Type</span></span>   | <span data-ttu-id="7b14e-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7b14e-124">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="7b14e-125">if-match</span><span class="sxs-lookup"><span data-stu-id="7b14e-125">if-match</span></span>      | <span data-ttu-id="7b14e-126">String</span><span class="sxs-lookup"><span data-stu-id="7b14e-126">String</span></span> | <span data-ttu-id="7b14e-127">Wenn dieser Anforderungsheader enthalten ist und das angegebene etag (oder cTag) nicht mit dem aktuellen etag des Ordners übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7b14e-127">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b14e-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7b14e-128">Request body</span></span>

<span data-ttu-id="7b14e-p104">Geben Sie im Anforderungstext den neuen Wert für die **parentReference**-Eigenschaft an. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="7b14e-p104">In the request body, supply the new value for the **parentReference** property. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

<span data-ttu-id="7b14e-132">**Hinweis:** Ihre App kann die `"id:" "root"`-Syntax beim Verschieben von Elementen in den Stammordner eines Laufwerks nicht verwenden.</span><span class="sxs-lookup"><span data-stu-id="7b14e-132">**Note:** When moving items to the root of a drive your app cannot use the `"id:" "root"` syntax.</span></span>
<span data-ttu-id="7b14e-133">Ihre App muss die tatsächliche ID des Stammordners für den übergeordneten Verweis bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="7b14e-133">Your app needs to provide the actual ID of the root folder for the parent reference.</span></span>

## <a name="response"></a><span data-ttu-id="7b14e-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b14e-134">Response</span></span>

<span data-ttu-id="7b14e-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und die aktualisierte [DriveItem](../resources/driveitem.md)-Ressource im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7b14e-135">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b14e-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7b14e-136">Example</span></span>

<span data-ttu-id="7b14e-137">In diesem Beispiel wird ein durch {item-id} angegebenes Element mit der ID `new-parent-folder-id` auf das Laufwerk des Benutzers verschoben.</span><span class="sxs-lookup"><span data-stu-id="7b14e-137">This example moves an item specified by {item-id} into a folder in the user's drive with the ID `new-parent-folder-id`.</span></span>

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

### <a name="response"></a><span data-ttu-id="7b14e-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b14e-138">Response</span></span>

<span data-ttu-id="7b14e-139">Das folgende Beispiel zeigt die Antwort für diese Verschiebungsanforderung.</span><span class="sxs-lookup"><span data-stu-id="7b14e-139">The following example shows the response for this move request.</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="7b14e-140">Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="7b14e-140">Error responses</span></span>

<span data-ttu-id="7b14e-141">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie unter [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="7b14e-141">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Move an item to another location or rename the item.",
  "keywords": "move,rename,mv,change location",
  "section": "documentation",
  "tocPath": "Items/Move"
} -->
