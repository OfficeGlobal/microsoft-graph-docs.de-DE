---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Erstellen einer SharePoint-Liste
ms.openlocfilehash: 223c324c132e1e6baf7fb23e57212e0b5fa63b56
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017789"
---
# <a name="create-a-new-list"></a><span data-ttu-id="90dd9-102">Eine neue Liste erstellen</span><span class="sxs-lookup"><span data-stu-id="90dd9-102">Create a new list</span></span>

<span data-ttu-id="90dd9-103">Erstellen Sie eine neue [Liste][] auf einer [Webseite][].</span><span class="sxs-lookup"><span data-stu-id="90dd9-103">Create a new [list][] in a [site][].</span></span>

## <a name="permissions"></a><span data-ttu-id="90dd9-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="90dd9-104">Permissions</span></span>

<span data-ttu-id="90dd9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90dd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="90dd9-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="90dd9-107">Permission type</span></span>             | <span data-ttu-id="90dd9-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="90dd9-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="90dd9-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="90dd9-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="90dd9-110">Sites.Manage.All</span><span class="sxs-lookup"><span data-stu-id="90dd9-110">Sites.Manage.All</span></span>                            |
| <span data-ttu-id="90dd9-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="90dd9-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90dd9-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="90dd9-112">Not supported.</span></span>                              |
| <span data-ttu-id="90dd9-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="90dd9-113">Application</span></span>                            | <span data-ttu-id="90dd9-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90dd9-114">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="90dd9-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="90dd9-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

## <a name="request-body"></a><span data-ttu-id="90dd9-116">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="90dd9-116">Request body</span></span>

<span data-ttu-id="90dd9-117">Geben Sie im Anforderungstext eine JSON-Darstellung der zu erstellenden [liste][]-Ressource an.</span><span class="sxs-lookup"><span data-stu-id="90dd9-117">In the request body, supply a JSON representation of the [list][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="90dd9-118">Beispiel</span><span class="sxs-lookup"><span data-stu-id="90dd9-118">Example</span></span>

<span data-ttu-id="90dd9-119">Unten sehen Sie ein Beispiel, das die Erstellung einer neuen generischen Liste illustriert.</span><span class="sxs-lookup"><span data-stu-id="90dd9-119">Here is an example of how to create a new generic list.</span></span>

<!-- { "blockType": "request", "name": "create-list", "scopes": "sites.readwrite.all" } -->

```http
POST /sites/{site-id}/lists
Content-Type: application/json

{
  "name": "Books",
  "columns": [
    {
      "name": "Author",
      "text": { }
    },
    {
      "name": "PageCount",
      "number": { }
    }
  ],
  "list": {
    "template": "genericList"
  }
}
```

<span data-ttu-id="90dd9-120">**Hinweis:** Benutzerdefinierte Spalten sind optional.</span><span class="sxs-lookup"><span data-stu-id="90dd9-120">**Note:** Custom columns are optional.</span></span>

<span data-ttu-id="90dd9-121">Zusätzlich zu den hier angegebenen Spalten werden neue Listen mit der in den referenzierten Spalten definierten **Vorlage** erstellt.</span><span class="sxs-lookup"><span data-stu-id="90dd9-121">In addition to any columns specified here, new lists are created with columns defined in the referenced **template**.</span></span>
<span data-ttu-id="90dd9-122">Wenn das **Listen**-Facette oder die **Vorlage** nicht angegeben ist, wird für die Liste standardmäßig die `genericList`Vorlage mit der Spalte _Titel_ verwendet.</span><span class="sxs-lookup"><span data-stu-id="90dd9-122">If the **list** facet or **template** is unspecified, the list defaults to the `genericList` template, which includes a _Title_ column.</span></span>

## <a name="response"></a><span data-ttu-id="90dd9-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="90dd9-123">Response</span></span>

<span data-ttu-id="90dd9-124">Wenn die Methode erfolgreich verläuft, wird ein [liste][]-Objekt im Antworttext der neu erstellten Liste zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="90dd9-124">If successful, this method returns a [list][] in the response body for the created list.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.list", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "22e03ef3-6ef4-424d-a1d3-92a337807c30",
  "createdDateTime": "2017-04-30T01:21:00Z",
  "createdBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  },
  "lastModifiedDateTime": "2016-08-30T08:26:00Z",
  "lastModifiedBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  }
}
```

<span data-ttu-id="90dd9-125">**Hinweis:** Das „Response“-Objekt wurde zwecks besserer Übersichtlichkeit gekürzt.</span><span class="sxs-lookup"><span data-stu-id="90dd9-125">**Note:** The response object is truncated for clarity.</span></span>
<span data-ttu-id="90dd9-126">Der tatsächliche Aufruf gibt die Standardeigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="90dd9-126">Default properties will be returned from the actual call.</span></span>

[list]: ../resources/list.md
[site]: ../resources/site.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "List/Create"
} -->
