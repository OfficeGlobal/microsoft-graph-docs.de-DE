---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Erstellen eines neuen Eintrags in einer SharePoint-Liste
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1af6162fd12c9c3dfc470b97e42a25d0cad8ebea
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482413"
---
# <a name="create-a-new-item-in-a-list"></a><span data-ttu-id="97f91-102">Neues Element in einer Liste erstellen</span><span class="sxs-lookup"><span data-stu-id="97f91-102">Create a new item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97f91-103">Erstellen Sie ein neues [listItem][] in einer [Liste][].</span><span class="sxs-lookup"><span data-stu-id="97f91-103">Create a new [listItem][] in a [list][].</span></span>

## <a name="permissions"></a><span data-ttu-id="97f91-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="97f91-104">Permissions</span></span>

<span data-ttu-id="97f91-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97f91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97f91-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="97f91-107">Permission type</span></span>      | <span data-ttu-id="97f91-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="97f91-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97f91-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="97f91-109">Delegated (work or school account)</span></span> | <span data-ttu-id="97f91-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97f91-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="97f91-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="97f91-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97f91-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97f91-112">Not supported.</span></span>    |
|<span data-ttu-id="97f91-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="97f91-113">Application</span></span> | <span data-ttu-id="97f91-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97f91-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="97f91-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="97f91-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
```

## <a name="request-body"></a><span data-ttu-id="97f91-116">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="97f91-116">Request body</span></span>

<span data-ttu-id="97f91-117">Geben Sie im Anforderungstext eine JSON-Darstellung der zu erstellenden [listItem][]-Ressource an.</span><span class="sxs-lookup"><span data-stu-id="97f91-117">In the request body, supply a JSON representation of the [listItem][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="97f91-118">Beispiel</span><span class="sxs-lookup"><span data-stu-id="97f91-118">Example</span></span>

<span data-ttu-id="97f91-119">Unten sehen Sie ein Beispiel, das die Erstellung eines neuen generischen Listenelements illustriert.</span><span class="sxs-lookup"><span data-stu-id="97f91-119">Here is an example of how to create a new generic list item.</span></span>

<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
POST https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
Content-Type: application/json

{
  "fields": {
    "Title": "Widget",
    "Color": "Purple",
    "Weight": 32
  }
}
```

## <a name="response"></a><span data-ttu-id="97f91-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="97f91-120">Response</span></span>

<span data-ttu-id="97f91-121">Wenn die Methode erfolgreich verläuft, wird ein [listItem][]-Objekt im Antworttext des neu erstellten Listenelements zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="97f91-121">If successful, this method returns a [listItem][] in the response body for the created list item.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "20",
  "createdDateTime": "2016-08-30T08:26:00Z",
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

<span data-ttu-id="97f91-122">**Hinweis:** Das „Response“-Objekt wurde zwecks besserer Übersichtlichkeit gekürzt.</span><span class="sxs-lookup"><span data-stu-id="97f91-122">**Note:** The response object is truncated for clarity.</span></span> <span data-ttu-id="97f91-123">Der tatsächliche Aufruf gibt die Standardeigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="97f91-123">Default properties will be returned from the actual call.</span></span>

[Liste]: ../resources/list.md
[list]: ../resources/list.md
[listItem]: ../resources/listitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Add a new item to a SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Create",
  "suppressions": [
    "Error: /api-reference/beta/api/listitem-create.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
