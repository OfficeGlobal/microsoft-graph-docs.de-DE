---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Aktualisieren eines Eintrags in einer SharePoint-Liste
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: f80f2607e953ba760893170366179f6751d9665d
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481993"
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="e80bc-102">Element in einer Liste aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e80bc-102">Update an item in a list</span></span>

<span data-ttu-id="e80bc-103">Aktualisieren Sie die Eigenschaften in einem **[listItem][]**.</span><span class="sxs-lookup"><span data-stu-id="e80bc-103">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="e80bc-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e80bc-104">Permissions</span></span>

<span data-ttu-id="e80bc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e80bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e80bc-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e80bc-107">Permission type</span></span>      | <span data-ttu-id="e80bc-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e80bc-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e80bc-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e80bc-109">Delegated (work or school account)</span></span> | <span data-ttu-id="e80bc-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e80bc-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e80bc-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e80bc-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e80bc-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e80bc-112">Not supported.</span></span>    |
|<span data-ttu-id="e80bc-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e80bc-113">Application</span></span> | <span data-ttu-id="e80bc-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e80bc-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e80bc-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e80bc-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="e80bc-116">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e80bc-116">Optional request headers</span></span>

| <span data-ttu-id="e80bc-117">Name</span><span class="sxs-lookup"><span data-stu-id="e80bc-117">Name</span></span>       | <span data-ttu-id="e80bc-118">Wert</span><span class="sxs-lookup"><span data-stu-id="e80bc-118">Value</span></span> | <span data-ttu-id="e80bc-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e80bc-119">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="e80bc-120">_if-match_</span><span class="sxs-lookup"><span data-stu-id="e80bc-120">_if-match_</span></span> | <span data-ttu-id="e80bc-121">etag</span><span class="sxs-lookup"><span data-stu-id="e80bc-121">etag</span></span>  | <span data-ttu-id="e80bc-122">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag nicht mit dem aktuellen Tag des Elements übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben, und das Element wird nicht aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="e80bc-122">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>


## <a name="request-body"></a><span data-ttu-id="e80bc-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e80bc-123">Request body</span></span>

<span data-ttu-id="e80bc-124">Geben Sie im Textbereich eine JSON-Darstellung von einem [FieldValueSet][] an, um die Felder für die Aktualisierung anzugeben.</span><span class="sxs-lookup"><span data-stu-id="e80bc-124">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="e80bc-125">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e80bc-125">Example</span></span>

<span data-ttu-id="e80bc-126">Dies ist ein Beispiel für die Aktualisierung der Felder Farbe und Menge Felder des Listenelements mit neuen Werten.</span><span class="sxs-lookup"><span data-stu-id="e80bc-126">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="e80bc-127">Alle anderen Werte des listItem bleiben unberührt.</span><span class="sxs-lookup"><span data-stu-id="e80bc-127">All other values on the listItem are left alone.</span></span> 

<!-- { "blockType": "request", "name": "update-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```

## <a name="response"></a><span data-ttu-id="e80bc-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="e80bc-128">Response</span></span>

<span data-ttu-id="e80bc-129">Wenn die Methode erfolgreich verläuft, wird ein [fieldValueSet][]-Objekt im Antworttext des aktualisierten Listenelements zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e80bc-129">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.fieldValueSet", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "Name": "Widget",
  "Color": "Fuchsia",
  "Quantity": 934
}
```

[fieldValueSet]: ../resources/fieldvalueset.md
[listItem]: ../resources/listitem.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Update"
} -->
