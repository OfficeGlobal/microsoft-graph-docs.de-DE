---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Löschen eines Eintrags aus einer SharePoint-Liste
localization_priority: Normal
ms.openlocfilehash: ea4f4b7d1f0f681348bcc9802736041b81a63c3a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863980"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="da611-102">Element aus einer Liste löschen</span><span class="sxs-lookup"><span data-stu-id="da611-102">Delete an item from a list</span></span>

<span data-ttu-id="da611-103">Entfernt ein Element aus einer [Liste][].</span><span class="sxs-lookup"><span data-stu-id="da611-103">Removes an item from a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="da611-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="da611-105">Permissions</span></span>

<span data-ttu-id="da611-106">Damit ein Element gelöscht werden kann, muss der Benutzer der Anwendung Schreibzugriff auf das zu löschende Element gewährt haben.</span><span class="sxs-lookup"><span data-stu-id="da611-106">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="da611-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da611-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da611-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="da611-109">Permission type</span></span>      | <span data-ttu-id="da611-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="da611-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da611-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="da611-111">Delegated (work or school account)</span></span> | <span data-ttu-id="da611-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da611-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="da611-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="da611-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da611-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="da611-114">Not supported.</span></span>    |
|<span data-ttu-id="da611-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="da611-115">Application</span></span> | <span data-ttu-id="da611-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da611-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="da611-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="da611-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="da611-118">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="da611-118">Optional request headers</span></span>

| <span data-ttu-id="da611-119">Name</span><span class="sxs-lookup"><span data-stu-id="da611-119">Name</span></span>       | <span data-ttu-id="da611-120">Wert</span><span class="sxs-lookup"><span data-stu-id="da611-120">Value</span></span> | <span data-ttu-id="da611-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da611-121">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="da611-122">_if-match_</span><span class="sxs-lookup"><span data-stu-id="da611-122">_if-match_</span></span> | <span data-ttu-id="da611-123">etag</span><span class="sxs-lookup"><span data-stu-id="da611-123">etag</span></span>  | <span data-ttu-id="da611-124">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag nicht mit dem aktuellen Tag des Elements übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben, und das Element wird nicht gelöscht.</span><span class="sxs-lookup"><span data-stu-id="da611-124">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="da611-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="da611-125">Request body</span></span>

<span data-ttu-id="da611-126">Bei dieser Methode wird kein Anforderungstext angegeben.</span><span class="sxs-lookup"><span data-stu-id="da611-126">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="da611-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="da611-127">Example</span></span>

<!-- { "blockType": "request", "name": "delete-item-site", "scopes": "files.readwrite sites.readwrite.all" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="da611-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="da611-128">Response</span></span>

<span data-ttu-id="da611-129">Wenn die Methode erfolgreich verläuft, wird die Antwort `204 No Content` zurückgegeben, um anzugeben, dass die Ressource gelöscht wurde und keine Werte zum Zurückgeben vorhanden waren.</span><span class="sxs-lookup"><span data-stu-id="da611-129">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

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
