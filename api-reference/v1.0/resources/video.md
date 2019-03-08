---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Video
localization_priority: Normal
ms.openlocfilehash: deba8cccb5f0ab80ca03395ef9f798719d542b8d
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480803"
---
# <a name="video-resource-type"></a><span data-ttu-id="bc309-102">Video-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bc309-102">Video resource type</span></span>

<span data-ttu-id="bc309-103">Die **Video**-Ressource gruppiert videobezogene Datenelemente in einer einzelnen Struktur.</span><span class="sxs-lookup"><span data-stu-id="bc309-103">The **Video** resource groups video-related data items into a single structure.</span></span>

<span data-ttu-id="bc309-p101">Wenn ein [**DriveItem**](driveitem.md) ein **video**-Facet ungleich Null aufweist, stellt das Element eine Videodatei dar. Die Eigenschaften der **Video**-Ressource werden durch Extrahieren von Metadaten aus der Datei aufgefüllt.</span><span class="sxs-lookup"><span data-stu-id="bc309-p101">If a [**DriveItem**](driveitem.md) has a non-null **video** facet, the item represents a video file. The properties of the **Video** resource are populated by extracting metadata from the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc309-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bc309-106">JSON representation</span></span>

<span data-ttu-id="bc309-107">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bc309-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="bc309-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bc309-108">Properties</span></span>

| <span data-ttu-id="bc309-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="bc309-109">Property name</span></span>             | <span data-ttu-id="bc309-110">Typ</span><span class="sxs-lookup"><span data-stu-id="bc309-110">Type</span></span>   | <span data-ttu-id="bc309-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc309-111">Description</span></span>
|:--------------------------|:-------|:----------------------------------------
| <span data-ttu-id="bc309-112">**audioBitsPerSample**</span><span class="sxs-lookup"><span data-stu-id="bc309-112">**audioBitsPerSample**</span></span>    | <span data-ttu-id="bc309-113">Int32</span><span class="sxs-lookup"><span data-stu-id="bc309-113">Int32</span></span>  | <span data-ttu-id="bc309-114">Anzahl von Audiobits pro Sample.</span><span class="sxs-lookup"><span data-stu-id="bc309-114">Number of audio bits per sample.</span></span>
| <span data-ttu-id="bc309-115">**audioChannels**</span><span class="sxs-lookup"><span data-stu-id="bc309-115">**audioChannels**</span></span>         | <span data-ttu-id="bc309-116">Int32</span><span class="sxs-lookup"><span data-stu-id="bc309-116">Int32</span></span>  | <span data-ttu-id="bc309-117">Anzahl der Audiokanäle.</span><span class="sxs-lookup"><span data-stu-id="bc309-117">Number of audio channels.</span></span>
| <span data-ttu-id="bc309-118">**audioFormat**</span><span class="sxs-lookup"><span data-stu-id="bc309-118">**audioFormat**</span></span>           | <span data-ttu-id="bc309-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bc309-119">string</span></span> | <span data-ttu-id="bc309-120">Name des Audioformats (AAC, MP3 usw.).</span><span class="sxs-lookup"><span data-stu-id="bc309-120">Name of the audio format (AAC, MP3, etc.).</span></span>
| <span data-ttu-id="bc309-121">**audioSamplesPerSecond**</span><span class="sxs-lookup"><span data-stu-id="bc309-121">**audioSamplesPerSecond**</span></span> | <span data-ttu-id="bc309-122">Int32</span><span class="sxs-lookup"><span data-stu-id="bc309-122">Int32</span></span>  | <span data-ttu-id="bc309-123">Anzahl der Audiosamples pro Sekunde.</span><span class="sxs-lookup"><span data-stu-id="bc309-123">Number of audio samples per second.</span></span>
| <span data-ttu-id="bc309-124">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="bc309-124">**bitrate**</span></span>               | <span data-ttu-id="bc309-125">Int32</span><span class="sxs-lookup"><span data-stu-id="bc309-125">Int32</span></span>  | <span data-ttu-id="bc309-126">Bitrate des Videos in Bits pro Sekunde.</span><span class="sxs-lookup"><span data-stu-id="bc309-126">Bit rate of the video in bits per second.</span></span>
| <span data-ttu-id="bc309-127">**duration**</span><span class="sxs-lookup"><span data-stu-id="bc309-127">**duration**</span></span>              | <span data-ttu-id="bc309-128">Int64</span><span class="sxs-lookup"><span data-stu-id="bc309-128">Int64</span></span>  | <span data-ttu-id="bc309-129">Dauer der Datei in Millisekunden.</span><span class="sxs-lookup"><span data-stu-id="bc309-129">Duration of the file in milliseconds.</span></span>
| <span data-ttu-id="bc309-130">**fourCC**</span><span class="sxs-lookup"><span data-stu-id="bc309-130">**fourCC**</span></span>                | <span data-ttu-id="bc309-131">string</span><span class="sxs-lookup"><span data-stu-id="bc309-131">string</span></span> | <span data-ttu-id="bc309-132">„Vier Zeichencode“-Name des Videoformats.</span><span class="sxs-lookup"><span data-stu-id="bc309-132">"Four character code" name of the video format.</span></span>
| <span data-ttu-id="bc309-133">**frameRate**</span><span class="sxs-lookup"><span data-stu-id="bc309-133">**frameRate**</span></span>             | <span data-ttu-id="bc309-134">double</span><span class="sxs-lookup"><span data-stu-id="bc309-134">double</span></span> | <span data-ttu-id="bc309-135">Framerate des Videos.</span><span class="sxs-lookup"><span data-stu-id="bc309-135">Frame rate of the video.</span></span>
| <span data-ttu-id="bc309-136">**height**</span><span class="sxs-lookup"><span data-stu-id="bc309-136">**height**</span></span>                | <span data-ttu-id="bc309-137">Int32</span><span class="sxs-lookup"><span data-stu-id="bc309-137">Int32</span></span>  | <span data-ttu-id="bc309-138">Die Höhe des Videos in Pixel.</span><span class="sxs-lookup"><span data-stu-id="bc309-138">Height of the video, in pixels.</span></span>
| <span data-ttu-id="bc309-139">**width**</span><span class="sxs-lookup"><span data-stu-id="bc309-139">**width**</span></span>                 | <span data-ttu-id="bc309-140">Int32</span><span class="sxs-lookup"><span data-stu-id="bc309-140">Int32</span></span>  | <span data-ttu-id="bc309-141">Die Breite des Videos in Pixel.</span><span class="sxs-lookup"><span data-stu-id="bc309-141">Width of the video, in pixels.</span></span>

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="bc309-142">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="bc309-142">Remarks</span></span>

<span data-ttu-id="bc309-143">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="bc309-143">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": "Facets/Video"
} -->
