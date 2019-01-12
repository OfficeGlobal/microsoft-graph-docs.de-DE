---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Löschen eines Eintrags aus einer SharePoint-Liste
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1b61c9359ca349a7f7882a204e8e474aba00444b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968463"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="0a24c-102">Element aus einer Liste löschen</span><span class="sxs-lookup"><span data-stu-id="0a24c-102">Delete an item from a list</span></span>

> <span data-ttu-id="0a24c-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0a24c-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a24c-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0a24c-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0a24c-105">Entfernt ein Element aus einer [Liste][].</span><span class="sxs-lookup"><span data-stu-id="0a24c-105">Removes an item from a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="0a24c-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0a24c-107">Permissions</span></span>

<span data-ttu-id="0a24c-108">Damit ein Element gelöscht werden kann, muss der Benutzer der Anwendung Schreibzugriff auf das zu löschende Element gewährt haben.</span><span class="sxs-lookup"><span data-stu-id="0a24c-108">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="0a24c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a24c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a24c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0a24c-111">Permission type</span></span>      | <span data-ttu-id="0a24c-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0a24c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a24c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0a24c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0a24c-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a24c-114">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="0a24c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0a24c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a24c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0a24c-116">Not supported.</span></span>    |
|<span data-ttu-id="0a24c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0a24c-117">Application</span></span> | <span data-ttu-id="0a24c-118">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a24c-118">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a24c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0a24c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="0a24c-120">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0a24c-120">Optional request headers</span></span>

| <span data-ttu-id="0a24c-121">Name</span><span class="sxs-lookup"><span data-stu-id="0a24c-121">Name</span></span>       | <span data-ttu-id="0a24c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0a24c-122">Value</span></span> | <span data-ttu-id="0a24c-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a24c-123">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="0a24c-124">_if-match_</span><span class="sxs-lookup"><span data-stu-id="0a24c-124">_if-match_</span></span> | <span data-ttu-id="0a24c-125">etag</span><span class="sxs-lookup"><span data-stu-id="0a24c-125">etag</span></span>  | <span data-ttu-id="0a24c-126">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag nicht mit dem aktuellen Tag des Elements übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben, und das Element wird nicht gelöscht.</span><span class="sxs-lookup"><span data-stu-id="0a24c-126">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="0a24c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0a24c-127">Request body</span></span>

<span data-ttu-id="0a24c-128">Bei dieser Methode wird kein Anforderungstext angegeben.</span><span class="sxs-lookup"><span data-stu-id="0a24c-128">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="0a24c-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0a24c-129">Example</span></span>

<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="0a24c-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="0a24c-130">Response</span></span>

<span data-ttu-id="0a24c-131">Wenn die Methode erfolgreich verläuft, wird die Antwort `204 No Content` zurückgegeben, um anzugeben, dass die Ressource gelöscht wurde und keine Werte zum Zurückgeben vorhanden waren.</span><span class="sxs-lookup"><span data-stu-id="0a24c-131">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

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
