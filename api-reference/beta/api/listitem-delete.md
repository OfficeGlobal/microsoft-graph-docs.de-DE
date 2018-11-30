---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Löschen eines Eintrags aus einer SharePoint-Liste
ms.openlocfilehash: d0b39a7c0ca69d3bfdd0edb256ac20711dfe5efc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063714"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="c6daa-102">Element aus einer Liste löschen</span><span class="sxs-lookup"><span data-stu-id="c6daa-102">Delete an item from a list</span></span>

> <span data-ttu-id="c6daa-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c6daa-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6daa-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c6daa-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c6daa-105">Entfernt ein Element aus einer [Liste][].</span><span class="sxs-lookup"><span data-stu-id="c6daa-105">Removes an item from a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="c6daa-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c6daa-107">Permissions</span></span>

<span data-ttu-id="c6daa-108">Damit ein Element gelöscht werden kann, muss der Benutzer der Anwendung Schreibzugriff auf das zu löschende Element gewährt haben.</span><span class="sxs-lookup"><span data-stu-id="c6daa-108">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="c6daa-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6daa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6daa-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c6daa-111">Permission type</span></span>      | <span data-ttu-id="c6daa-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c6daa-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6daa-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c6daa-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c6daa-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6daa-114">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c6daa-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c6daa-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6daa-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c6daa-116">Not supported.</span></span>    |
|<span data-ttu-id="c6daa-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c6daa-117">Application</span></span> | <span data-ttu-id="c6daa-118">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6daa-118">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6daa-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c6daa-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="c6daa-120">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c6daa-120">Optional request headers</span></span>

| <span data-ttu-id="c6daa-121">Name</span><span class="sxs-lookup"><span data-stu-id="c6daa-121">Name</span></span>       | <span data-ttu-id="c6daa-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c6daa-122">Value</span></span> | <span data-ttu-id="c6daa-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c6daa-123">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="c6daa-124">_if-match_</span><span class="sxs-lookup"><span data-stu-id="c6daa-124">_if-match_</span></span> | <span data-ttu-id="c6daa-125">etag</span><span class="sxs-lookup"><span data-stu-id="c6daa-125">etag</span></span>  | <span data-ttu-id="c6daa-126">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag nicht mit dem aktuellen Tag des Elements übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben, und das Element wird nicht gelöscht.</span><span class="sxs-lookup"><span data-stu-id="c6daa-126">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="c6daa-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c6daa-127">Request body</span></span>

<span data-ttu-id="c6daa-128">Bei dieser Methode wird kein Anforderungstext angegeben.</span><span class="sxs-lookup"><span data-stu-id="c6daa-128">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="c6daa-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c6daa-129">Example</span></span>

<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="c6daa-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="c6daa-130">Response</span></span>

<span data-ttu-id="c6daa-131">Wenn die Methode erfolgreich verläuft, wird die Antwort `204 No Content` zurückgegeben, um anzugeben, dass die Ressource gelöscht wurde und keine Werte zum Zurückgeben vorhanden waren.</span><span class="sxs-lookup"><span data-stu-id="c6daa-131">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Delete"
} -->
