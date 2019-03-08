---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Löschen eines Eintrags aus einer SharePoint-Liste
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 83a14c237b59c66c24bab2705520c84f3f0e090e
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481930"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="51bb0-102">Element aus einer Liste löschen</span><span class="sxs-lookup"><span data-stu-id="51bb0-102">Delete an item from a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51bb0-103">Entfernt ein Element aus einer [Liste][].</span><span class="sxs-lookup"><span data-stu-id="51bb0-103">Removes an item from a [list][].</span></span>

[Liste]: ../resources/list.md
[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="51bb0-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="51bb0-105">Permissions</span></span>

<span data-ttu-id="51bb0-106">Damit ein Element gelöscht werden kann, muss der Benutzer der Anwendung Schreibzugriff auf das zu löschende Element gewährt haben.</span><span class="sxs-lookup"><span data-stu-id="51bb0-106">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="51bb0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51bb0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51bb0-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="51bb0-109">Permission type</span></span>      | <span data-ttu-id="51bb0-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="51bb0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51bb0-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="51bb0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="51bb0-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51bb0-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="51bb0-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="51bb0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51bb0-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="51bb0-114">Not supported.</span></span>    |
|<span data-ttu-id="51bb0-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="51bb0-115">Application</span></span> | <span data-ttu-id="51bb0-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51bb0-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="51bb0-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="51bb0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="51bb0-118">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="51bb0-118">Optional request headers</span></span>

| <span data-ttu-id="51bb0-119">Name</span><span class="sxs-lookup"><span data-stu-id="51bb0-119">Name</span></span>       | <span data-ttu-id="51bb0-120">Wert</span><span class="sxs-lookup"><span data-stu-id="51bb0-120">Value</span></span> | <span data-ttu-id="51bb0-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="51bb0-121">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="51bb0-122">_if-match_</span><span class="sxs-lookup"><span data-stu-id="51bb0-122">_if-match_</span></span> | <span data-ttu-id="51bb0-123">etag</span><span class="sxs-lookup"><span data-stu-id="51bb0-123">etag</span></span>  | <span data-ttu-id="51bb0-124">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag nicht mit dem aktuellen Tag des Elements übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben, und das Element wird nicht gelöscht.</span><span class="sxs-lookup"><span data-stu-id="51bb0-124">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="51bb0-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="51bb0-125">Request body</span></span>

<span data-ttu-id="51bb0-126">Bei dieser Methode wird kein Anforderungstext angegeben.</span><span class="sxs-lookup"><span data-stu-id="51bb0-126">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="51bb0-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="51bb0-127">Example</span></span>

<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="51bb0-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="51bb0-128">Response</span></span>

<span data-ttu-id="51bb0-129">Wenn die Methode erfolgreich verläuft, wird die Antwort `204 No Content` zurückgegeben, um anzugeben, dass die Ressource gelöscht wurde und keine Werte zum Zurückgeben vorhanden waren.</span><span class="sxs-lookup"><span data-stu-id="51bb0-129">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Delete",
  "suppressions": [
    "Error: /api-reference/beta/api/listitem-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
