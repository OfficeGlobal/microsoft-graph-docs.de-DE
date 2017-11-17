---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Aktualisieren eines Eintrags in einer SharePoint-Liste
ms.openlocfilehash: ca1c3dcb96ba347b457253b3843114402dba8ba3
ms.sourcegitcommit: 339070a20730bc4d363da7eb346d5f3c1e1d6c3e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/18/2017
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="9a677-102">Element in einer Liste aktualisieren</span><span class="sxs-lookup"><span data-stu-id="9a677-102">Update an item in a list</span></span>

<span data-ttu-id="9a677-103">Aktualisieren Sie die Eigenschaften in einem **[listItem][]**.</span><span class="sxs-lookup"><span data-stu-id="9a677-103">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a677-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9a677-104">Permissions</span></span>

<span data-ttu-id="9a677-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9a677-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9a677-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9a677-107">Permission type</span></span>      | <span data-ttu-id="9a677-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9a677-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a677-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9a677-109">Delegated (work or school account)</span></span> | <span data-ttu-id="9a677-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a677-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="9a677-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9a677-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a677-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9a677-112">Not supported.</span></span>    |
|<span data-ttu-id="9a677-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9a677-113">Application</span></span> | <span data-ttu-id="9a677-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a677-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a677-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9a677-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="9a677-116">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9a677-116">Optional request headers</span></span>

| <span data-ttu-id="9a677-117">Name</span><span class="sxs-lookup"><span data-stu-id="9a677-117">Name</span></span>       | <span data-ttu-id="9a677-118">Wert</span><span class="sxs-lookup"><span data-stu-id="9a677-118">Value</span></span> | <span data-ttu-id="9a677-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9a677-119">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="9a677-120">_if-match_</span><span class="sxs-lookup"><span data-stu-id="9a677-120">_if-match_</span></span> | <span data-ttu-id="9a677-121">etag</span><span class="sxs-lookup"><span data-stu-id="9a677-121">etag</span></span>  | <span data-ttu-id="9a677-122">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag nicht mit dem aktuellen Tag des Elements übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben, und das Element wird nicht aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="9a677-122">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>


## <a name="request-body"></a><span data-ttu-id="9a677-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9a677-123">Request body</span></span>

<span data-ttu-id="9a677-124">Geben Sie im Textbereich eine JSON-Darstellung von einem [FieldValueSet][] an, um die Felder für die Aktualisierung anzugeben.</span><span class="sxs-lookup"><span data-stu-id="9a677-124">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="9a677-125">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9a677-125">Example</span></span>

<span data-ttu-id="9a677-126">Dies ist ein Beispiel für die Aktualisierung der Felder Farbe und Menge Felder des Listenelements mit neuen Werten.</span><span class="sxs-lookup"><span data-stu-id="9a677-126">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="9a677-127">Alle anderen Werte des listItem bleiben unberührt.</span><span class="sxs-lookup"><span data-stu-id="9a677-127">All other values on the listItem are left alone.</span></span> 

<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```

## <a name="response"></a><span data-ttu-id="9a677-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="9a677-128">Response</span></span>

<span data-ttu-id="9a677-129">Wenn die Methode erfolgreich verläuft, wird ein [fieldValueSet][]-Objekt im Antworttext des aktualisierten Listenelements zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9a677-129">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "Name": "Widget",
  "Color": "Fuchsia",
  "Quantity": 934
}
```

[fieldValueSet]: ../resources/fieldValueSet.md
[listItem]: ../resources/listItem.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Update"
} -->
