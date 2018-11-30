---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Video
ms.openlocfilehash: a9bf228d814526d089fb102444e6952558b07e1c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064941"
---
# <a name="video-resource-type"></a><span data-ttu-id="91225-102">Video-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="91225-102">Video resource type</span></span>

> <span data-ttu-id="91225-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="91225-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91225-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="91225-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="91225-105">Die **Video**-Ressource gruppiert videobezogene Datenelemente in einer einzelnen Struktur.</span><span class="sxs-lookup"><span data-stu-id="91225-105">The **Video** resource groups video-related data items into a single structure.</span></span>

<span data-ttu-id="91225-p102">Wenn ein [**DriveItem**](driveitem.md) ein **video**-Facet ungleich Null aufweist, stellt das Element eine Videodatei dar. Die Eigenschaften der **Video**-Ressource werden durch Extrahieren von Metadaten aus der Datei aufgefüllt.</span><span class="sxs-lookup"><span data-stu-id="91225-p102">If a [**DriveItem**](driveitem.md) has a non-null **video** facet, the item represents a video file. The properties of the **Video** resource are populated by extracting metadata from the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="91225-108">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="91225-108">JSON representation</span></span>

<span data-ttu-id="91225-109">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="91225-109">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.video"
}-->

```json
{
  "audioBitsPerSample": 16,
  "audioChannels": 1,
  "audioFormat": "AAC",
  "audioSamplesPerSecond": 44100,
  "bitrate": 39101896,
  "duration": 8053,
  "fourCC": "H264",
  "frameRate": 239.877,
  "height": 1280,
  "width": 720
}
```

## <a name="properties"></a><span data-ttu-id="91225-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="91225-110">Properties</span></span>

| <span data-ttu-id="91225-111">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="91225-111">Property name</span></span>             | <span data-ttu-id="91225-112">Typ</span><span class="sxs-lookup"><span data-stu-id="91225-112">Type</span></span>   | <span data-ttu-id="91225-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91225-113">Description</span></span>
|:--------------------------|:-------|:----------------------------------------
| <span data-ttu-id="91225-114">**audioBitsPerSample**</span><span class="sxs-lookup"><span data-stu-id="91225-114">**audioBitsPerSample**</span></span>    | <span data-ttu-id="91225-115">Int32</span><span class="sxs-lookup"><span data-stu-id="91225-115">Int32</span></span>  | <span data-ttu-id="91225-116">Anzahl von Audiobits pro Sample.</span><span class="sxs-lookup"><span data-stu-id="91225-116">Number of audio bits per sample.</span></span>
| <span data-ttu-id="91225-117">**audioChannels**</span><span class="sxs-lookup"><span data-stu-id="91225-117">**audioChannels**</span></span>         | <span data-ttu-id="91225-118">Int32</span><span class="sxs-lookup"><span data-stu-id="91225-118">Int32</span></span>  | <span data-ttu-id="91225-119">Anzahl der Audiokanäle.</span><span class="sxs-lookup"><span data-stu-id="91225-119">Number of audio channels.</span></span>
| <span data-ttu-id="91225-120">**audioFormat**</span><span class="sxs-lookup"><span data-stu-id="91225-120">**audioFormat**</span></span>           | <span data-ttu-id="91225-121">string</span><span class="sxs-lookup"><span data-stu-id="91225-121">string</span></span> | <span data-ttu-id="91225-122">Name des Audioformats (AAC, MP3 usw.).</span><span class="sxs-lookup"><span data-stu-id="91225-122">Name of the audio format (AAC, MP3, etc.).</span></span>
| <span data-ttu-id="91225-123">**audioSamplesPerSecond**</span><span class="sxs-lookup"><span data-stu-id="91225-123">**audioSamplesPerSecond**</span></span> | <span data-ttu-id="91225-124">Int32</span><span class="sxs-lookup"><span data-stu-id="91225-124">Int32</span></span>  | <span data-ttu-id="91225-125">Anzahl der Audiosamples pro Sekunde.</span><span class="sxs-lookup"><span data-stu-id="91225-125">Number of audio samples per second.</span></span>
| <span data-ttu-id="91225-126">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="91225-126">**bitrate**</span></span>               | <span data-ttu-id="91225-127">Int32</span><span class="sxs-lookup"><span data-stu-id="91225-127">Int32</span></span>  | <span data-ttu-id="91225-128">Bitrate des Videos in Bits pro Sekunde.</span><span class="sxs-lookup"><span data-stu-id="91225-128">Bit rate of the video in bits per second.</span></span>
| <span data-ttu-id="91225-129">**duration**</span><span class="sxs-lookup"><span data-stu-id="91225-129">**duration**</span></span>              | <span data-ttu-id="91225-130">Int64</span><span class="sxs-lookup"><span data-stu-id="91225-130">Int64</span></span>  | <span data-ttu-id="91225-131">Dauer der Datei in Millisekunden.</span><span class="sxs-lookup"><span data-stu-id="91225-131">Duration of the file in milliseconds.</span></span>
| <span data-ttu-id="91225-132">**fourCC**</span><span class="sxs-lookup"><span data-stu-id="91225-132">**fourCC**</span></span>                | <span data-ttu-id="91225-133">string</span><span class="sxs-lookup"><span data-stu-id="91225-133">string</span></span> | <span data-ttu-id="91225-134">„Vier Zeichencode“-Name des Videoformats.</span><span class="sxs-lookup"><span data-stu-id="91225-134">"Four character code" name of the video format.</span></span>
| <span data-ttu-id="91225-135">**framerate**</span><span class="sxs-lookup"><span data-stu-id="91225-135">**framerate**</span></span>             | <span data-ttu-id="91225-136">double</span><span class="sxs-lookup"><span data-stu-id="91225-136">double</span></span> | <span data-ttu-id="91225-137">Framerate des Videos.</span><span class="sxs-lookup"><span data-stu-id="91225-137">Frame rate of the video.</span></span>
| <span data-ttu-id="91225-138">**height**</span><span class="sxs-lookup"><span data-stu-id="91225-138">**height**</span></span>                | <span data-ttu-id="91225-139">Int32</span><span class="sxs-lookup"><span data-stu-id="91225-139">Int32</span></span>  | <span data-ttu-id="91225-140">Die Höhe des Videos in Pixel.</span><span class="sxs-lookup"><span data-stu-id="91225-140">Height of the video, in pixels.</span></span>
| <span data-ttu-id="91225-141">**width**</span><span class="sxs-lookup"><span data-stu-id="91225-141">**width**</span></span>                 | <span data-ttu-id="91225-142">Int32</span><span class="sxs-lookup"><span data-stu-id="91225-142">Int32</span></span>  | <span data-ttu-id="91225-143">Die Breite des Videos in Pixel.</span><span class="sxs-lookup"><span data-stu-id="91225-143">Width of the video, in pixels.</span></span>

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="91225-144">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="91225-144">Remarks</span></span>

<span data-ttu-id="91225-145">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="91225-145">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>





<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": ""
}-->
