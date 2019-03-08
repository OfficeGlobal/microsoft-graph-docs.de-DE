---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Ändern von Freigabeberechtigungen
localization_priority: Normal
ms.openlocfilehash: 64d6618b17b061293ab4e5b5296f7ad39d5a8512
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480726"
---
# <a name="update-sharing-permission"></a><span data-ttu-id="5ff30-102">Freigabeberechtigung aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5ff30-102">Update sharing permission</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ff30-103">Über diese API können Sie die Eigenschaften einer Freigabeberechtigung aktualisieren, indem Sie einen Patch auf die betreffende Berechtigungsressource anwenden.</span><span class="sxs-lookup"><span data-stu-id="5ff30-103">Update the properties of a sharing permission by patching the permission resource.</span></span>

<span data-ttu-id="5ff30-104">Nur die **roles**-Eigenschaft kann auf diese Weise geändert werden.</span><span class="sxs-lookup"><span data-stu-id="5ff30-104">Only the **roles** property can be modified this way.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ff30-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5ff30-105">Permissions</span></span>

<span data-ttu-id="5ff30-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ff30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ff30-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5ff30-108">Permission type</span></span>      | <span data-ttu-id="5ff30-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5ff30-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ff30-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5ff30-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5ff30-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ff30-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="5ff30-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5ff30-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ff30-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ff30-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="5ff30-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5ff30-114">Application</span></span> | <span data-ttu-id="5ff30-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ff30-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ff30-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5ff30-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
PATCH /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
PATCH /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="5ff30-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5ff30-117">Optional request headers</span></span>

| <span data-ttu-id="5ff30-118">Name</span><span class="sxs-lookup"><span data-stu-id="5ff30-118">Name</span></span>          | <span data-ttu-id="5ff30-119">Typ</span><span class="sxs-lookup"><span data-stu-id="5ff30-119">Type</span></span>   | <span data-ttu-id="5ff30-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5ff30-120">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="5ff30-121">if-match</span><span class="sxs-lookup"><span data-stu-id="5ff30-121">if-match</span></span>      | <span data-ttu-id="5ff30-122">string</span><span class="sxs-lookup"><span data-stu-id="5ff30-122">string</span></span> | <span data-ttu-id="5ff30-123">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag (oder cTag) nicht mit dem aktuellen Tag des Elements übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben, und das Element wird nicht gelöscht.</span><span class="sxs-lookup"><span data-stu-id="5ff30-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ff30-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5ff30-124">Request body</span></span>

<span data-ttu-id="5ff30-125">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="5ff30-125">In the request body, supply the values for relevant fields that should be updated.</span></span>

<span data-ttu-id="5ff30-126">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="5ff30-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="5ff30-127">Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="5ff30-127">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5ff30-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5ff30-128">Property</span></span>     | <span data-ttu-id="5ff30-129">Typ</span><span class="sxs-lookup"><span data-stu-id="5ff30-129">Type</span></span>   | <span data-ttu-id="5ff30-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5ff30-130">Description</span></span>                   |
|:-------------|:-------|:------------------------------|
| <span data-ttu-id="5ff30-131">**roles**</span><span class="sxs-lookup"><span data-stu-id="5ff30-131">**roles**</span></span>    | <span data-ttu-id="5ff30-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5ff30-132">String</span></span> | <span data-ttu-id="5ff30-133">Ein Array von Berechtigungstypen.</span><span class="sxs-lookup"><span data-stu-id="5ff30-133">An array of permission types.</span></span> |

## <a name="response"></a><span data-ttu-id="5ff30-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="5ff30-134">Response</span></span>

<span data-ttu-id="5ff30-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [permission](../resources/permission.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5ff30-135">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ff30-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5ff30-136">Example</span></span>

<span data-ttu-id="5ff30-137">Dies ist ein Beispiel für die Anforderung, welche die Rolle der Freigabeberechtigung zu Schreibgeschützt ändert.</span><span class="sxs-lookup"><span data-stu-id="5ff30-137">Here is an example of the request that changes the role on the sharing permission to read-only.</span></span>

<!-- {"blockType": "request", "name": "update-permission", "@odata.type": "microsoft.graph.permission", "scopes": "files.readwrite"} -->

```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```

### <a name="response"></a><span data-ttu-id="5ff30-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="5ff30-138">Response</span></span>

<span data-ttu-id="5ff30-139">Bei Erfolg gibt diese Methode eine [Permission](../resources/permission.md)-Ressource im Antworttext zurück, die den aktualisierten Status der Berechtigung darstellt.</span><span class="sxs-lookup"><span data-stu-id="5ff30-139">If successful, this method returns a [Permission](../resources/permission.md) resource in the response body that represents the updated state of the permission.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "read" ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update an item's sharing permissions",
  "keywords": "permission, permissions, sharing, change permissions, update permission",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission",
  "suppressions": [
    "Error: /api-reference/beta/api/permission-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
