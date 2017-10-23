---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "Freigabeberechtigungen ändern"
ms.openlocfilehash: ead6babf88b7efc578ef8be6d11cc9fb59dd5fdd
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="update-sharing-permission"></a><span data-ttu-id="69c8d-102">Freigabeberechtigung aktualisieren</span><span class="sxs-lookup"><span data-stu-id="69c8d-102">Update sharing permission</span></span>

<span data-ttu-id="69c8d-103">Über diese API können Sie die Eigenschaften einer Freigabeberechtigung aktualisieren, indem Sie einen Patch auf die betreffende Berechtigungsressource anwenden.</span><span class="sxs-lookup"><span data-stu-id="69c8d-103">Update the properties of a permission by patching the resource.</span></span>

<span data-ttu-id="69c8d-104">Nur die **roles**-Eigenschaft kann auf diese Weise geändert werden.</span><span class="sxs-lookup"><span data-stu-id="69c8d-104">Only the **roles** property can be modified this way.</span></span>

## <a name="permissions"></a><span data-ttu-id="69c8d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="69c8d-105">Permissions</span></span>

<span data-ttu-id="69c8d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="69c8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="69c8d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="69c8d-108">Permission type</span></span>      | <span data-ttu-id="69c8d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="69c8d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69c8d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="69c8d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="69c8d-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69c8d-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="69c8d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="69c8d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69c8d-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69c8d-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="69c8d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="69c8d-114">Application</span></span> | <span data-ttu-id="69c8d-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69c8d-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="69c8d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="69c8d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
PATCH /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
PATCH /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="69c8d-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="69c8d-117">Optional request headers</span></span>

| <span data-ttu-id="69c8d-118">Name</span><span class="sxs-lookup"><span data-stu-id="69c8d-118">Name</span></span>          | <span data-ttu-id="69c8d-119">Typ</span><span class="sxs-lookup"><span data-stu-id="69c8d-119">Type</span></span>   | <span data-ttu-id="69c8d-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="69c8d-120">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="69c8d-121">if-match</span><span class="sxs-lookup"><span data-stu-id="69c8d-121">if-match</span></span>      | <span data-ttu-id="69c8d-122">string</span><span class="sxs-lookup"><span data-stu-id="69c8d-122">string</span></span> | <span data-ttu-id="69c8d-123">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag (oder cTag) nicht mit dem aktuellen Tag des Elements übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben, und das Element wird nicht gelöscht.</span><span class="sxs-lookup"><span data-stu-id="69c8d-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="69c8d-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="69c8d-124">Request body</span></span>

<span data-ttu-id="69c8d-125">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="69c8d-125">In the request body, supply the values for relevant fields that should be updated.</span></span>

<span data-ttu-id="69c8d-126">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="69c8d-126">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>
<span data-ttu-id="69c8d-127">Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="69c8d-127">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="69c8d-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="69c8d-128">Property</span></span>     | <span data-ttu-id="69c8d-129">Typ</span><span class="sxs-lookup"><span data-stu-id="69c8d-129">Type</span></span>   | <span data-ttu-id="69c8d-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="69c8d-130">Description</span></span>                   |
|:-------------|:-------|:------------------------------|
| <span data-ttu-id="69c8d-131">**roles**</span><span class="sxs-lookup"><span data-stu-id="69c8d-131">**roles**</span></span>    | <span data-ttu-id="69c8d-132">String</span><span class="sxs-lookup"><span data-stu-id="69c8d-132">String</span></span> | <span data-ttu-id="69c8d-133">Ein Array von Berechtigungstypen.</span><span class="sxs-lookup"><span data-stu-id="69c8d-133">An array of permission types.</span></span> |

## <a name="response"></a><span data-ttu-id="69c8d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="69c8d-134">Response</span></span>

<span data-ttu-id="69c8d-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [permission](../resources/permission.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="69c8d-135">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69c8d-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="69c8d-136">Example</span></span>

<span data-ttu-id="69c8d-137">Dies ist ein Beispiel für die Anforderung, welche die Rolle der Freigabeberechtigung zu Schreibgeschützt ändert.</span><span class="sxs-lookup"><span data-stu-id="69c8d-137">Here is an example of the request that changes the role on the sharing permission to read-only.</span></span>

<!-- {"blockType": "request", "name": "update-permission", "@odata.type": "microsoft.graph.permission", "scopes": "files.readwrite"} -->

```http
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```

### <a name="response"></a><span data-ttu-id="69c8d-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="69c8d-138">Response</span></span>

<span data-ttu-id="69c8d-139">Bei Erfolg gibt diese Methode eine [Permission](../resources/permission.md)-Ressource im Antworttext zurück, die den aktualisierten Status der Berechtigung darstellt.</span><span class="sxs-lookup"><span data-stu-id="69c8d-139">If successful, this method returns a [Permission](../resources/permission.md) resource in the response body that represents the updated state of the permission.</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="69c8d-140">Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="69c8d-140">Error responses</span></span>

<span data-ttu-id="69c8d-141">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie im Thema [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="69c8d-141">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

[error-response]: ../../../concepts/errors.md

<!-- {
  "type": "#page.annotation",
  "description": "Update an item's sharing permissions",
  "keywords": "permission, permissions, sharing, change permissions, update permission",
  "section": "documentation",
  "tocPath": "Sharing/Update permission"
} -->
