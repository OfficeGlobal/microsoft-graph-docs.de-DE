---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Freigabeberechtigungen ändern
localization_priority: Normal
ms.openlocfilehash: 44f98d559ab6dc4c81a4efede2f3f60020c2f944
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859682"
---
# <a name="update-sharing-permission"></a><span data-ttu-id="db122-102">Freigabeberechtigung aktualisieren</span><span class="sxs-lookup"><span data-stu-id="db122-102">Update sharing permission</span></span>

> <span data-ttu-id="db122-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="db122-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="db122-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="db122-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="db122-105">Über diese API können Sie die Eigenschaften einer Freigabeberechtigung aktualisieren, indem Sie einen Patch auf die betreffende Berechtigungsressource anwenden.</span><span class="sxs-lookup"><span data-stu-id="db122-105">Update the properties of a sharing permission by patching the permission resource.</span></span>

<span data-ttu-id="db122-106">Nur die **roles**-Eigenschaft kann auf diese Weise geändert werden.</span><span class="sxs-lookup"><span data-stu-id="db122-106">Only the **roles** property can be modified this way.</span></span>

## <a name="permissions"></a><span data-ttu-id="db122-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="db122-107">Permissions</span></span>

<span data-ttu-id="db122-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db122-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db122-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="db122-110">Permission type</span></span>      | <span data-ttu-id="db122-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="db122-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db122-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="db122-112">Delegated (work or school account)</span></span> | <span data-ttu-id="db122-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db122-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="db122-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="db122-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db122-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db122-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="db122-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="db122-116">Application</span></span> | <span data-ttu-id="db122-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db122-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db122-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="db122-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
PATCH /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
PATCH /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="db122-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="db122-119">Optional request headers</span></span>

| <span data-ttu-id="db122-120">Name</span><span class="sxs-lookup"><span data-stu-id="db122-120">Name</span></span>          | <span data-ttu-id="db122-121">Typ</span><span class="sxs-lookup"><span data-stu-id="db122-121">Type</span></span>   | <span data-ttu-id="db122-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="db122-122">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="db122-123">if-match</span><span class="sxs-lookup"><span data-stu-id="db122-123">if-match</span></span>      | <span data-ttu-id="db122-124">string</span><span class="sxs-lookup"><span data-stu-id="db122-124">string</span></span> | <span data-ttu-id="db122-125">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag (oder cTag) nicht mit dem aktuellen Tag des Elements übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben, und das Element wird nicht gelöscht.</span><span class="sxs-lookup"><span data-stu-id="db122-125">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db122-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="db122-126">Request body</span></span>

<span data-ttu-id="db122-127">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="db122-127">In the request body, supply the values for relevant fields that should be updated.</span></span>

<span data-ttu-id="db122-128">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="db122-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="db122-129">Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="db122-129">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="db122-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="db122-130">Property</span></span>     | <span data-ttu-id="db122-131">Typ</span><span class="sxs-lookup"><span data-stu-id="db122-131">Type</span></span>   | <span data-ttu-id="db122-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="db122-132">Description</span></span>                   |
|:-------------|:-------|:------------------------------|
| <span data-ttu-id="db122-133">**roles**</span><span class="sxs-lookup"><span data-stu-id="db122-133">**roles**</span></span>    | <span data-ttu-id="db122-134">String</span><span class="sxs-lookup"><span data-stu-id="db122-134">String</span></span> | <span data-ttu-id="db122-135">Ein Array von Berechtigungstypen.</span><span class="sxs-lookup"><span data-stu-id="db122-135">An array of permission types.</span></span> |

## <a name="response"></a><span data-ttu-id="db122-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="db122-136">Response</span></span>

<span data-ttu-id="db122-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [permission](../resources/permission.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="db122-137">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db122-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="db122-138">Example</span></span>

<span data-ttu-id="db122-139">Dies ist ein Beispiel für die Anforderung, welche die Rolle der Freigabeberechtigung zu Schreibgeschützt ändert.</span><span class="sxs-lookup"><span data-stu-id="db122-139">Here is an example of the request that changes the role on the sharing permission to read-only.</span></span>

<!-- {"blockType": "request", "name": "update-permission", "@odata.type": "microsoft.graph.permission", "scopes": "files.readwrite"} -->

```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```

### <a name="response"></a><span data-ttu-id="db122-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="db122-140">Response</span></span>

<span data-ttu-id="db122-141">Bei Erfolg gibt diese Methode eine [Permission](../resources/permission.md)-Ressource im Antworttext zurück, die den aktualisierten Status der Berechtigung darstellt.</span><span class="sxs-lookup"><span data-stu-id="db122-141">If successful, this method returns a [Permission](../resources/permission.md) resource in the response body that represents the updated state of the permission.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Update an item's sharing permissions",
  "keywords": "permission, permissions, sharing, change permissions, update permission",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission"
}-->
