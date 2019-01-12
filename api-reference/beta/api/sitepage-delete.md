---
author: rahmit
ms.author: rahmit
ms.date: 05/07/2018
title: Löschen einer Seite aus einer SharePoint-Website
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b4ac336999484f6af97e41d08caa926fae4c055f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950025"
---
# <a name="delete-page-from-the-site-pages-list-of-a-site"></a><span data-ttu-id="98418-102">Löschen der Seite aus der Liste Website Seiten einer Website</span><span class="sxs-lookup"><span data-stu-id="98418-102">Delete page from the site pages list of a site</span></span>

> <span data-ttu-id="98418-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="98418-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="98418-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="98418-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="98418-105">Entfernt eine [SitePage][] aus der Website-Seiten- [Liste][] in einer [Website][].</span><span class="sxs-lookup"><span data-stu-id="98418-105">Removes a [sitePage][] from the site pages [list][] in a [site][].</span></span>

[sitePage]: ../resources/sitepage.md
[list]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="98418-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="98418-109">Permissions</span></span>

<span data-ttu-id="98418-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98418-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="98418-112">**Hinweis:** Um ein Element zu löschen, muss der Benutzer die Anwendung Schreibzugriff auf das Element, das gelöscht werden erteilt haben.</span><span class="sxs-lookup"><span data-stu-id="98418-112">**Note:** To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

|<span data-ttu-id="98418-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="98418-113">Permission type</span></span>      | <span data-ttu-id="98418-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="98418-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98418-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="98418-115">Delegated (work or school account)</span></span> | <span data-ttu-id="98418-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98418-116">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="98418-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="98418-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98418-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="98418-118">Not supported.</span></span>    |
|<span data-ttu-id="98418-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="98418-119">Application</span></span> | <span data-ttu-id="98418-120">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98418-120">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="98418-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="98418-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/pages/{page-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="98418-122">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="98418-122">Optional request headers</span></span>

| <span data-ttu-id="98418-123">Name</span><span class="sxs-lookup"><span data-stu-id="98418-123">Name</span></span>       | <span data-ttu-id="98418-124">Wert</span><span class="sxs-lookup"><span data-stu-id="98418-124">Value</span></span> | <span data-ttu-id="98418-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="98418-125">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="98418-126">_if-match_</span><span class="sxs-lookup"><span data-stu-id="98418-126">_if-match_</span></span> | <span data-ttu-id="98418-127">etag</span><span class="sxs-lookup"><span data-stu-id="98418-127">etag</span></span>  | <span data-ttu-id="98418-128">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag nicht mit dem aktuellen Tag des Elements übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben, und das Element wird nicht gelöscht.</span><span class="sxs-lookup"><span data-stu-id="98418-128">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="98418-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="98418-129">Request body</span></span>

<span data-ttu-id="98418-130">Bei dieser Methode wird kein Anforderungstext angegeben.</span><span class="sxs-lookup"><span data-stu-id="98418-130">Do not supply a request body with this method.</span></span>
<!-- TODO: should we provide a URL to recover/undelete the file, if one exists? -->

## <a name="response"></a><span data-ttu-id="98418-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="98418-131">Response</span></span>

<span data-ttu-id="98418-132">Wenn erfolgreich ist, dieses Anrufs gibt eine `204 No Content` Antwort, um anzugeben, dass die Ressource wurde gelöscht, und es nothing wurde zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="98418-132">If successful, this call returns a `204 No Content` response to indicate that the resource was deleted and there was nothing to return.</span></span>

## <a name="example"></a><span data-ttu-id="98418-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="98418-133">Example</span></span>

<!-- { "blockType": "request", "name": "delete-page", "scopes": "files.readwrite sites.readwrite.all" } -->

##### <a name="request"></a><span data-ttu-id="98418-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="98418-134">Request</span></span>

```http
DELETE /sites/{site-id}/pages/{page-id}
```
##### <a name="response"></a><span data-ttu-id="98418-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="98418-135">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Delete a page in the SitePages list in a site.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Pages/Delete"
} -->
