---
author: rahmit
ms.author: rahmit
ms.date: 05/07/2018
title: Löschen einer Seite aus einer SharePoint-Website
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f855942288556fdf07e2b3af78408976c34eb052
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513025"
---
# <a name="delete-page-from-the-site-pages-list-of-a-site"></a><span data-ttu-id="61239-102">Löschen der Seite aus der Liste Website Seiten einer Website</span><span class="sxs-lookup"><span data-stu-id="61239-102">Delete page from the site pages list of a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61239-103">Entfernt eine [SitePage][] aus der Website-Seiten- [Liste][] in einer [Website][].</span><span class="sxs-lookup"><span data-stu-id="61239-103">Removes a [sitePage][] from the site pages [list][] in a [site][].</span></span>

[sitePage]: ../resources/sitepage.md
[list]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="61239-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="61239-107">Permissions</span></span>

<span data-ttu-id="61239-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61239-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="61239-110">**Hinweis:** Um ein Element zu löschen, muss der Benutzer die Anwendung Schreibzugriff auf das Element, das gelöscht werden erteilt haben.</span><span class="sxs-lookup"><span data-stu-id="61239-110">**Note:** To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

|<span data-ttu-id="61239-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="61239-111">Permission type</span></span>      | <span data-ttu-id="61239-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="61239-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61239-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="61239-113">Delegated (work or school account)</span></span> | <span data-ttu-id="61239-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61239-114">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="61239-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="61239-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61239-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="61239-116">Not supported.</span></span>    |
|<span data-ttu-id="61239-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="61239-117">Application</span></span> | <span data-ttu-id="61239-118">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61239-118">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="61239-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="61239-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/pages/{page-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="61239-120">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="61239-120">Optional request headers</span></span>

| <span data-ttu-id="61239-121">Name</span><span class="sxs-lookup"><span data-stu-id="61239-121">Name</span></span>       | <span data-ttu-id="61239-122">Wert</span><span class="sxs-lookup"><span data-stu-id="61239-122">Value</span></span> | <span data-ttu-id="61239-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61239-123">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="61239-124">_if-match_</span><span class="sxs-lookup"><span data-stu-id="61239-124">_if-match_</span></span> | <span data-ttu-id="61239-125">etag</span><span class="sxs-lookup"><span data-stu-id="61239-125">etag</span></span>  | <span data-ttu-id="61239-126">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag nicht mit dem aktuellen Tag des Elements übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben, und das Element wird nicht gelöscht.</span><span class="sxs-lookup"><span data-stu-id="61239-126">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="61239-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="61239-127">Request body</span></span>

<span data-ttu-id="61239-128">Bei dieser Methode wird kein Anforderungstext angegeben.</span><span class="sxs-lookup"><span data-stu-id="61239-128">Do not supply a request body with this method.</span></span>
<!-- TODO: should we provide a URL to recover/undelete the file, if one exists? -->

## <a name="response"></a><span data-ttu-id="61239-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="61239-129">Response</span></span>

<span data-ttu-id="61239-130">Wenn erfolgreich ist, dieses Anrufs gibt eine `204 No Content` Antwort, um anzugeben, dass die Ressource wurde gelöscht, und es nothing wurde zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="61239-130">If successful, this call returns a `204 No Content` response to indicate that the resource was deleted and there was nothing to return.</span></span>

## <a name="example"></a><span data-ttu-id="61239-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="61239-131">Example</span></span>

<!-- { "blockType": "request", "name": "delete-page", "scopes": "files.readwrite sites.readwrite.all" } -->

##### <a name="request"></a><span data-ttu-id="61239-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="61239-132">Request</span></span>

```http
DELETE /sites/{site-id}/pages/{page-id}
```
##### <a name="response"></a><span data-ttu-id="61239-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="61239-133">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Delete a page in the SitePages list in a site.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Pages/Delete",
  "suppressions": [
    "Error: /api-reference/beta/api/sitepage-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
