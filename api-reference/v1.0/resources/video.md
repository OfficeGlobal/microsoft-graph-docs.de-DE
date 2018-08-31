---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Video
ms.openlocfilehash: cb9e28c1b26aa60fe7d854796df8bff34ca8e5df
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23265848"
---
# <a name="video-resource-type"></a><span data-ttu-id="3060e-102">Video-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3060e-102">Video resource type</span></span>

<span data-ttu-id="3060e-103">Die **Video**-Ressource gruppiert videobezogene Datenelemente in einer einzelnen Struktur.</span><span class="sxs-lookup"><span data-stu-id="3060e-103">The **Video** resource groups video-related data items into a single structure.</span></span>

<span data-ttu-id="3060e-p101">Wenn ein [**DriveItem**](driveitem.md) ein **video**-Facet ungleich Null aufweist, stellt das Element eine Videodatei dar. Die Eigenschaften der **Video**-Ressource werden durch Extrahieren von Metadaten aus der Datei aufgefüllt.</span><span class="sxs-lookup"><span data-stu-id="3060e-p101">If a [**DriveItem**](driveitem.md) has a non-null **video** facet, the item represents a video file. The properties of the **Video** resource are populated by extracting metadata from the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3060e-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3060e-106">JSON representation</span></span>

<span data-ttu-id="3060e-107">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3060e-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="3060e-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3060e-108">Properties</span></span>

| <span data-ttu-id="3060e-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="3060e-109">Property name</span></span>             | <span data-ttu-id="3060e-110">Typ</span><span class="sxs-lookup"><span data-stu-id="3060e-110">Type</span></span>   | <span data-ttu-id="3060e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3060e-111">Description</span></span>
|:--------------------------|:-------|:----------------------------------------
| <span data-ttu-id="3060e-112">**audioBitsPerSample**</span><span class="sxs-lookup"><span data-stu-id="3060e-112">**audioBitsPerSample**</span></span>    | <span data-ttu-id="3060e-113">Int32</span><span class="sxs-lookup"><span data-stu-id="3060e-113">Int32</span></span>  | <span data-ttu-id="3060e-114">Anzahl von Audiobits pro Sample.</span><span class="sxs-lookup"><span data-stu-id="3060e-114">Number of audio bits per sample.</span></span>
| <span data-ttu-id="3060e-115">**audioChannels**</span><span class="sxs-lookup"><span data-stu-id="3060e-115">**audioChannels**</span></span>         | <span data-ttu-id="3060e-116">Int32</span><span class="sxs-lookup"><span data-stu-id="3060e-116">Int32</span></span>  | <span data-ttu-id="3060e-117">Anzahl der Audiokanäle.</span><span class="sxs-lookup"><span data-stu-id="3060e-117">Number of audio channels.</span></span>
| <span data-ttu-id="3060e-118">**audioFormat**</span><span class="sxs-lookup"><span data-stu-id="3060e-118">**audioFormat**</span></span>           | <span data-ttu-id="3060e-119">string</span><span class="sxs-lookup"><span data-stu-id="3060e-119">string</span></span> | <span data-ttu-id="3060e-120">Name des Audioformats (AAC, MP3 usw.).</span><span class="sxs-lookup"><span data-stu-id="3060e-120">Name of the audio format (AAC, MP3, etc.).</span></span>
| <span data-ttu-id="3060e-121">**audioSamplesPerSecond**</span><span class="sxs-lookup"><span data-stu-id="3060e-121">**audioSamplesPerSecond**</span></span> | <span data-ttu-id="3060e-122">Int32</span><span class="sxs-lookup"><span data-stu-id="3060e-122">Int32</span></span>  | <span data-ttu-id="3060e-123">Anzahl der Audiosamples pro Sekunde.</span><span class="sxs-lookup"><span data-stu-id="3060e-123">Number of audio samples per second.</span></span>
| <span data-ttu-id="3060e-124">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="3060e-124">**bitrate**</span></span>               | <span data-ttu-id="3060e-125">Int32</span><span class="sxs-lookup"><span data-stu-id="3060e-125">Int32</span></span>  | <span data-ttu-id="3060e-126">Bitrate des Videos in Bits pro Sekunde.</span><span class="sxs-lookup"><span data-stu-id="3060e-126">Bit rate of the video in bits per second.</span></span>
| <span data-ttu-id="3060e-127">**duration**</span><span class="sxs-lookup"><span data-stu-id="3060e-127">**duration**</span></span>              | <span data-ttu-id="3060e-128">Int64</span><span class="sxs-lookup"><span data-stu-id="3060e-128">Int64</span></span>  | <span data-ttu-id="3060e-129">Dauer der Datei in Millisekunden.</span><span class="sxs-lookup"><span data-stu-id="3060e-129">Duration of the file in milliseconds.</span></span>
| <span data-ttu-id="3060e-130">**fourCC**</span><span class="sxs-lookup"><span data-stu-id="3060e-130">**fourCC**</span></span>                | <span data-ttu-id="3060e-131">string</span><span class="sxs-lookup"><span data-stu-id="3060e-131">string</span></span> | <span data-ttu-id="3060e-132">„Vier Zeichencode“-Name des Videoformats.</span><span class="sxs-lookup"><span data-stu-id="3060e-132">"Four character code" name of the video format.</span></span>
| <span data-ttu-id="3060e-133">**frameRate**</span><span class="sxs-lookup"><span data-stu-id="3060e-133">**framerate**</span></span>             | <span data-ttu-id="3060e-134">double</span><span class="sxs-lookup"><span data-stu-id="3060e-134">double</span></span> | <span data-ttu-id="3060e-135">Framerate des Videos.</span><span class="sxs-lookup"><span data-stu-id="3060e-135">Frame rate of the video.</span></span>
| <span data-ttu-id="3060e-136">**height**</span><span class="sxs-lookup"><span data-stu-id="3060e-136">**height**</span></span>                | <span data-ttu-id="3060e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="3060e-137">Int32</span></span>  | <span data-ttu-id="3060e-138">Die Höhe des Videos in Pixel.</span><span class="sxs-lookup"><span data-stu-id="3060e-138">Height of the video, in pixels.</span></span>
| <span data-ttu-id="3060e-139">**width**</span><span class="sxs-lookup"><span data-stu-id="3060e-139">**width**</span></span>                 | <span data-ttu-id="3060e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="3060e-140">Int32</span></span>  | <span data-ttu-id="3060e-141">Die Breite des Videos in Pixel.</span><span class="sxs-lookup"><span data-stu-id="3060e-141">Width of the video, in pixels.</span></span>

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="3060e-142">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="3060e-142">Remarks</span></span>

<span data-ttu-id="3060e-143">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="3060e-143">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": "Facets/Video"
} -->
