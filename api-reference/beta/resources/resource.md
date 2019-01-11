---
title: resource-Ressourcentyp
description: 'Ein Bild oder eine andere Dateiressource auf einer OneNote-Seite. '
localization_priority: Normal
ms.openlocfilehash: a8ba7b2afb5b083e4fe5250ef499043029a1195b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879520"
---
# <a name="resource-resource-type"></a><span data-ttu-id="cde99-103">resource-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="cde99-103">resource resource type</span></span>

> <span data-ttu-id="cde99-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cde99-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cde99-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cde99-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cde99-106">Ein Bild oder eine andere Dateiressource auf einer OneNote-Seite.</span><span class="sxs-lookup"><span data-stu-id="cde99-106">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="cde99-107">Sie können die Binärdaten einer Ressource abrufen, der Abruf einer JSON-Darstellung eines Ressourcenobjekts oder einer Ressourcensammlung wird jedoch nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cde99-107">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

<span data-ttu-id="cde99-108">Rufen Sie die Binärdaten einer bestimmten Ressource ab, indem Sie eine GET-Anforderung an den Endpunkt `content` der Ressourcen senden:</span><span class="sxs-lookup"><span data-stu-id="cde99-108">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="cde99-109">Der Ressourcen-URI der Datei wird zurückgegeben, wenn Sie den HTML-Inhalt einer Seite mit der folgenden Anforderung abrufen:</span><span class="sxs-lookup"><span data-stu-id="cde99-109">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="cde99-110">Im HTML-Code der Seite schließt ein `img`-Tag Endpunkte für die ursprüngliche Bildressource in das Attribut `data-fullres-src` und das optimierte Bild in das Attribut `src` ein:</span><span class="sxs-lookup"><span data-stu-id="cde99-110">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="cde99-111">Ein `object`-Tag (das Dateien wie PDF, DOCX und PNG darstellt) schließt den Endpunkt für die Dateiressource in das Attribut `data` ein:</span><span class="sxs-lookup"><span data-stu-id="cde99-111">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="cde99-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cde99-112">Properties</span></span>
<span data-ttu-id="cde99-113">Keine.</span><span class="sxs-lookup"><span data-stu-id="cde99-113">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="cde99-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="cde99-114">Relationships</span></span>
<span data-ttu-id="cde99-115">Keine.</span><span class="sxs-lookup"><span data-stu-id="cde99-115">None.</span></span>


## <a name="methods"></a><span data-ttu-id="cde99-116">Methoden</span><span class="sxs-lookup"><span data-stu-id="cde99-116">Methods</span></span>
| <span data-ttu-id="cde99-117">Methode</span><span class="sxs-lookup"><span data-stu-id="cde99-117">Method</span></span>           | <span data-ttu-id="cde99-118">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="cde99-118">Return Type</span></span>    |<span data-ttu-id="cde99-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cde99-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cde99-120">Binärdaten von Ressource abrufen</span><span class="sxs-lookup"><span data-stu-id="cde99-120">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="cde99-121">Stream</span><span class="sxs-lookup"><span data-stu-id="cde99-121">Stream</span></span> |<span data-ttu-id="cde99-122">Dient zum Abrufen der Binärdaten einer Datei- oder Bildressource.</span><span class="sxs-lookup"><span data-stu-id="cde99-122">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
