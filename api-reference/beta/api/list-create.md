---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Erstellen einer SharePoint-Liste
localization_priority: Normal
ms.openlocfilehash: bf1bc2afdba13878050c13cf81dcdfadf230ee3d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808274"
---
# <a name="create-a-new-list"></a><span data-ttu-id="baf90-102">Eine neue Liste erstellen</span><span class="sxs-lookup"><span data-stu-id="baf90-102">Create a new list</span></span>

> <span data-ttu-id="baf90-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="baf90-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="baf90-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="baf90-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="baf90-105">Erstellen Sie eine neue [Liste][] auf einer [Webseite][].</span><span class="sxs-lookup"><span data-stu-id="baf90-105">Create a new [list][] in a [site][].</span></span>

## <a name="permissions"></a><span data-ttu-id="baf90-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="baf90-106">Permissions</span></span>

<span data-ttu-id="baf90-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="baf90-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="baf90-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="baf90-109">Permission type</span></span>             | <span data-ttu-id="baf90-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="baf90-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="baf90-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="baf90-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="baf90-112">Sites.Manage.All</span><span class="sxs-lookup"><span data-stu-id="baf90-112">Sites.Manage.All</span></span>                            |
| <span data-ttu-id="baf90-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="baf90-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="baf90-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="baf90-114">Not supported.</span></span>                              |
| <span data-ttu-id="baf90-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="baf90-115">Application</span></span>                            | <span data-ttu-id="baf90-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="baf90-116">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="baf90-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="baf90-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="request-body"></a><span data-ttu-id="baf90-118">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="baf90-118">Request body</span></span>

<span data-ttu-id="baf90-119">Geben Sie im Anforderungstext eine JSON-Darstellung der zu erstellenden [liste][]-Ressource an.</span><span class="sxs-lookup"><span data-stu-id="baf90-119">In the request body, supply a JSON representation of the [list][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="baf90-120">Beispiel</span><span class="sxs-lookup"><span data-stu-id="baf90-120">Example</span></span>

<span data-ttu-id="baf90-121">Unten sehen Sie ein Beispiel, das die Erstellung einer neuen generischen Liste illustriert.</span><span class="sxs-lookup"><span data-stu-id="baf90-121">Here is an example of how to create a new generic list.</span></span>

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

<span data-ttu-id="baf90-122">**Hinweis:** Benutzerdefinierte Spalten sind optional.</span><span class="sxs-lookup"><span data-stu-id="baf90-122">**Note:** Custom columns are optional.</span></span>

<span data-ttu-id="baf90-123">Zusätzlich zu den hier angegebenen Spalten werden neue Listen mit der in den referenzierten Spalten definierten **Vorlage** erstellt.</span><span class="sxs-lookup"><span data-stu-id="baf90-123">In addition to any columns specified here, new lists are created with columns defined in the referenced **template**.</span></span>
<span data-ttu-id="baf90-124">Wenn das **Listen**-Facette oder die **Vorlage** nicht angegeben ist, wird für die Liste standardmäßig die `genericList`Vorlage mit der Spalte _Titel_ verwendet.</span><span class="sxs-lookup"><span data-stu-id="baf90-124">If the **list** facet or **template** is unspecified, the list defaults to the `genericList` template, which includes a _Title_ column.</span></span>

## <a name="response"></a><span data-ttu-id="baf90-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="baf90-125">Response</span></span>

<span data-ttu-id="baf90-126">Wenn die Methode erfolgreich verläuft, wird ein [liste][]-Objekt im Antworttext der neu erstellten Liste zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="baf90-126">If successful, this method returns a [list][] in the response body for the created list.</span></span>

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

<span data-ttu-id="baf90-127">**Hinweis:** Das „Response“-Objekt wurde zwecks besserer Übersichtlichkeit gekürzt.</span><span class="sxs-lookup"><span data-stu-id="baf90-127">**Note:** The response object is truncated for clarity.</span></span>
<span data-ttu-id="baf90-128">Der tatsächliche Aufruf gibt die Standardeigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="baf90-128">Default properties will be returned from the actual call.</span></span>

[list]: ../resources/list.md
[site]: ../resources/site.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "List/Create"
} -->
