---
title: Ressourcentyp OneNoteResource
description: 'Ein Bild oder eine andere Dateiressource auf einer OneNote-Seite. '
ms.openlocfilehash: a5be2602e2a015b278ed7c3e01c573a543c7c6a1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017616"
---
# <a name="onenoteresource-resource-type"></a><span data-ttu-id="da40b-103">Ressourcentyp OneNoteResource</span><span class="sxs-lookup"><span data-stu-id="da40b-103">OneNoteResource resource type</span></span>

<span data-ttu-id="da40b-104">Ein Bild oder eine andere Dateiressource auf einer OneNote-Seite.</span><span class="sxs-lookup"><span data-stu-id="da40b-104">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="da40b-105">Sie können die Binärdaten einer Ressource abrufen, der Abruf einer JSON-Darstellung eines Ressourcenobjekts oder einer Ressourcensammlung wird jedoch nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="da40b-105">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityBaseModel",
  "optionalProperties": [],
  "isMediaEntity": true,
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "contentUrl": "string (url)"
}
```

<span data-ttu-id="da40b-106">Rufen Sie die Binärdaten einer bestimmten Ressource ab, indem Sie eine GET-Anforderung an den Endpunkt `content` der Ressourcen senden:</span><span class="sxs-lookup"><span data-stu-id="da40b-106">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="da40b-107">Der Ressourcen-URI der Datei wird zurückgegeben, wenn Sie den HTML-Inhalt einer Seite mit der folgenden Anforderung abrufen:</span><span class="sxs-lookup"><span data-stu-id="da40b-107">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="da40b-108">Im HTML-Code der Seite schließt ein `img`-Tag Endpunkte für die ursprüngliche Bildressource in das Attribut `data-fullres-src` und das optimierte Bild in das Attribut `src` ein:</span><span class="sxs-lookup"><span data-stu-id="da40b-108">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="da40b-109">Ein `object`-Tag (das Dateien wie PDF, DOCX und PNG darstellt) schließt den Endpunkt für die Dateiressource in das Attribut `data` ein:</span><span class="sxs-lookup"><span data-stu-id="da40b-109">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="da40b-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="da40b-110">Properties</span></span>

| <span data-ttu-id="da40b-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="da40b-111">Property</span></span>             | <span data-ttu-id="da40b-112">Typ</span><span class="sxs-lookup"><span data-stu-id="da40b-112">Type</span></span>            | <span data-ttu-id="da40b-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da40b-113">Description</span></span>
|:---------------------|:----------------|:---------------------------------
| <span data-ttu-id="da40b-114">Inhalt</span><span class="sxs-lookup"><span data-stu-id="da40b-114">content</span></span>              | <span data-ttu-id="da40b-115">Stream</span><span class="sxs-lookup"><span data-stu-id="da40b-115">Stream</span></span>          | <span data-ttu-id="da40b-116">Der Inhaltsstream</span><span class="sxs-lookup"><span data-stu-id="da40b-116">The content stream</span></span>
| <span data-ttu-id="da40b-117">contentUrl</span><span class="sxs-lookup"><span data-stu-id="da40b-117">contentUrl</span></span>           | <span data-ttu-id="da40b-118">Zeichenfolge (Url)</span><span class="sxs-lookup"><span data-stu-id="da40b-118">String (url)</span></span>    | <span data-ttu-id="da40b-119">Die URL für das Herunterladen von Inhalt</span><span class="sxs-lookup"><span data-stu-id="da40b-119">The URL for downloading the content</span></span>

## <a name="relationships"></a><span data-ttu-id="da40b-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="da40b-120">Relationships</span></span>
<span data-ttu-id="da40b-121">Keine.</span><span class="sxs-lookup"><span data-stu-id="da40b-121">None.</span></span>


## <a name="methods"></a><span data-ttu-id="da40b-122">Methoden</span><span class="sxs-lookup"><span data-stu-id="da40b-122">Methods</span></span>
| <span data-ttu-id="da40b-123">Methode</span><span class="sxs-lookup"><span data-stu-id="da40b-123">Method</span></span>           | <span data-ttu-id="da40b-124">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="da40b-124">Return Type</span></span>    |<span data-ttu-id="da40b-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da40b-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="da40b-126">Binärdaten von Ressource abrufen</span><span class="sxs-lookup"><span data-stu-id="da40b-126">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="da40b-127">Stream</span><span class="sxs-lookup"><span data-stu-id="da40b-127">Stream</span></span> |<span data-ttu-id="da40b-128">Dient zum Abrufen der Binärdaten einer Datei- oder Bildressource.</span><span class="sxs-lookup"><span data-stu-id="da40b-128">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->