---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Eine Datei oder einen Ordner aktualisieren
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5a10caf65846418013712e89ade7a182726c80a8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514600"
---
# <a name="update-driveitem-properties"></a><span data-ttu-id="fd164-102">DriveItem-Eigenschaften aktualisieren</span><span class="sxs-lookup"><span data-stu-id="fd164-102">Update DriveItem properties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd164-103">Dient zum Aktualisieren der Metadaten für ein [DriveItem](../resources/driveitem.md) anhand ID oder Pfad.</span><span class="sxs-lookup"><span data-stu-id="fd164-103">Update the metadata for a [DriveItem](../resources/driveitem.md) by ID or path.</span></span>

<span data-ttu-id="fd164-104">Mithilfe dieser API können Sie außerdem [Elemente unter ein anderes übergeordnetes Element verschieben](driveitem-move.md), indem Sie die Eigenschaft **parentReference** des zu verschiebenden Elements aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="fd164-104">You can also use update to [move an item](driveitem-move.md) to another parent by updating the item's **parentReference** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd164-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fd164-105">Permissions</span></span>

<span data-ttu-id="fd164-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd164-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd164-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fd164-108">Permission type</span></span>      | <span data-ttu-id="fd164-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fd164-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd164-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fd164-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fd164-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd164-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="fd164-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fd164-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd164-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd164-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="fd164-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fd164-114">Application</span></span> | <span data-ttu-id="fd164-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd164-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd164-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd164-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/items/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="fd164-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fd164-117">Optional request headers</span></span>

| <span data-ttu-id="fd164-118">Name</span><span class="sxs-lookup"><span data-stu-id="fd164-118">Name</span></span>          | <span data-ttu-id="fd164-119">Typ</span><span class="sxs-lookup"><span data-stu-id="fd164-119">Type</span></span>   | <span data-ttu-id="fd164-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd164-120">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="fd164-121">if-match</span><span class="sxs-lookup"><span data-stu-id="fd164-121">if-match</span></span>      | <span data-ttu-id="fd164-122">String</span><span class="sxs-lookup"><span data-stu-id="fd164-122">String</span></span> | <span data-ttu-id="fd164-123">Wenn dieser Anforderungsheader enthalten ist und das angegebene etag (oder cTag) nicht mit dem aktuellen etag des Ordners übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fd164-123">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd164-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fd164-124">Request body</span></span>

<span data-ttu-id="fd164-125">Geben Sie im Anforderungstext die Werte für die Eigenschaften an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="fd164-125">In the request body, supply the values for properties that should be updated.</span></span>

<span data-ttu-id="fd164-126">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="fd164-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="fd164-127">Um eine optimale Leistung zu erzielen, sollte Ihre App keine Eigenschaften umfassen, die sich nicht geändert haben.</span><span class="sxs-lookup"><span data-stu-id="fd164-127">For best performance your app should not include properties that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="fd164-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd164-128">Response</span></span>

<span data-ttu-id="fd164-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und die aktualisierte [DriveItem](../resources/driveitem.md)-Ressource im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fd164-129">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd164-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fd164-130">Example</span></span>

<span data-ttu-id="fd164-131">In diesem Beispiel wird die DriveItem-Ressource in "new-file-name.docx" umbenannt.</span><span class="sxs-lookup"><span data-stu-id="fd164-131">This example renames the DriveItem resource to "new-file-name.docx".</span></span>

<!-- { "blockType": "request", "name": "update-item" } -->

```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
  "name": "new-file-name.docx"
}
```

### <a name="response"></a><span data-ttu-id="fd164-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd164-132">Response</span></span>

<span data-ttu-id="fd164-133">Wenn die Methode erfolgreich verläuft, wird eine [driveItem][item-resource]-Ressource im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fd164-133">If successful, this method returns an [driveItem][item-resource] resource in the response body.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "01NKDM7HMOJTVYMDOSXFDK2QJDXCDI3WUK",
  "name": "new-file-name.docx",
  "file": { }
}
```

## <a name="error-responses"></a><span data-ttu-id="fd164-134">Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="fd164-134">Error responses</span></span>

<span data-ttu-id="fd164-135">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie unter [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="fd164-135">See [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Update or replace the contents or properties of an item.",
  "keywords": "update,replace,contents,item",
  "section": "documentation",
  "tocPath": "Items/Update",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
