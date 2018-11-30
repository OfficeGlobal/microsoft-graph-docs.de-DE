---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Audio
ms.openlocfilehash: 43b9999ecfb472a82e00a12ca820fdf8548eec64
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="audio-facet"></a><span data-ttu-id="e09e9-102">Audio-Facet</span><span class="sxs-lookup"><span data-stu-id="e09e9-102">Audio facet</span></span>

<span data-ttu-id="e09e9-103">Die Ressource **Audio** führt audiobezogene Eigenschaften für ein Element in einer einzelnen Struktur zusammen.</span><span class="sxs-lookup"><span data-stu-id="e09e9-103">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="e09e9-104">Wenn ein [**DriveItem**](driveitem.md)-Element ein **audio**-Facet ungleich Null aufweist, stellt das Element eine Audiodatei dar.</span><span class="sxs-lookup"><span data-stu-id="e09e9-104">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the Audio resource are populated by extracting metadata from the file.</span></span>
<span data-ttu-id="e09e9-105">Die Eigenschaften der **Audio**-Ressource werden durch Extrahieren von Metadaten aus der Datei aufgefüllt.</span><span class="sxs-lookup"><span data-stu-id="e09e9-105">If a DriveItem has a non-null audio facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="e09e9-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e09e9-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.audio" } -->
```json
{
  "album": "string",
  "albumArtist": "string",
  "artist": "string",
  "bitrate": 128,
  "composers": "string",
  "copyright": "string",
  "disc": 0,
  "discCount": 0,
  "duration": 567,
  "genre": "string",
  "hasDrm": false,
  "isVariableBitrate": false,
  "title": "string",
  "track": 1,
  "trackCount": 16,
  "year": 2014
}
```

## <a name="properties"></a><span data-ttu-id="e09e9-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e09e9-107">Properties</span></span>

| <span data-ttu-id="e09e9-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="e09e9-108">Property name</span></span>         | <span data-ttu-id="e09e9-109">Typ</span><span class="sxs-lookup"><span data-stu-id="e09e9-109">Type</span></span>    | <span data-ttu-id="e09e9-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e09e9-110">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="e09e9-111">**album**</span><span class="sxs-lookup"><span data-stu-id="e09e9-111">**album**</span></span>             | <span data-ttu-id="e09e9-112">string</span><span class="sxs-lookup"><span data-stu-id="e09e9-112">string</span></span>  | <span data-ttu-id="e09e9-113">Der Titel des Albums, zu dem die Audiodatei gehört</span><span class="sxs-lookup"><span data-stu-id="e09e9-113">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="e09e9-114">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="e09e9-114">**albumArtist**</span></span>       | <span data-ttu-id="e09e9-115">string</span><span class="sxs-lookup"><span data-stu-id="e09e9-115">string</span></span>  | <span data-ttu-id="e09e9-116">Der Künstler, der für das Album genannt ist, zu dem die Audiodatei gehört</span><span class="sxs-lookup"><span data-stu-id="e09e9-116">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="e09e9-117">**artist**</span><span class="sxs-lookup"><span data-stu-id="e09e9-117">**artist**</span></span>            | <span data-ttu-id="e09e9-118">string</span><span class="sxs-lookup"><span data-stu-id="e09e9-118">string</span></span>  | <span data-ttu-id="e09e9-119">Der zur Audiodatei gehörende Künstler</span><span class="sxs-lookup"><span data-stu-id="e09e9-119">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="e09e9-120">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="e09e9-120">**bitrate**</span></span>           | <span data-ttu-id="e09e9-121">Int32</span><span class="sxs-lookup"><span data-stu-id="e09e9-121">Int32</span></span>   | <span data-ttu-id="e09e9-122">Die Bitrate in KBit/s</span><span class="sxs-lookup"><span data-stu-id="e09e9-122">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="e09e9-123">**composers**</span><span class="sxs-lookup"><span data-stu-id="e09e9-123">**composers**</span></span>         | <span data-ttu-id="e09e9-124">string</span><span class="sxs-lookup"><span data-stu-id="e09e9-124">string</span></span>  | <span data-ttu-id="e09e9-125">Der Name des Komponisten der Audiodatei</span><span class="sxs-lookup"><span data-stu-id="e09e9-125">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="e09e9-126">**copyright**</span><span class="sxs-lookup"><span data-stu-id="e09e9-126">**copyright**</span></span>         | <span data-ttu-id="e09e9-127">string</span><span class="sxs-lookup"><span data-stu-id="e09e9-127">string</span></span>  | <span data-ttu-id="e09e9-128">Urheberrechtsinformationen zur Audiodatei</span><span class="sxs-lookup"><span data-stu-id="e09e9-128">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="e09e9-129">**disc**</span><span class="sxs-lookup"><span data-stu-id="e09e9-129">**disc**</span></span>              | <span data-ttu-id="e09e9-130">Int32</span><span class="sxs-lookup"><span data-stu-id="e09e9-130">Int32</span></span>   | <span data-ttu-id="e09e9-131">Die Nummer der CD, von der die Audiodatei stammt</span><span class="sxs-lookup"><span data-stu-id="e09e9-131">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="e09e9-132">**discCount**</span><span class="sxs-lookup"><span data-stu-id="e09e9-132">**discCount**</span></span>         | <span data-ttu-id="e09e9-133">Int32</span><span class="sxs-lookup"><span data-stu-id="e09e9-133">Int32</span></span>   | <span data-ttu-id="e09e9-134">Die Gesamtanzahl von CDs im Album</span><span class="sxs-lookup"><span data-stu-id="e09e9-134">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="e09e9-135">**duration**</span><span class="sxs-lookup"><span data-stu-id="e09e9-135">**duration**</span></span>          | <span data-ttu-id="e09e9-136">Int64</span><span class="sxs-lookup"><span data-stu-id="e09e9-136">Int64</span></span>   | <span data-ttu-id="e09e9-137">Die Dauer der Audiodatei in Millisekunden</span><span class="sxs-lookup"><span data-stu-id="e09e9-137">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="e09e9-138">**genre**</span><span class="sxs-lookup"><span data-stu-id="e09e9-138">**genre**</span></span>             | <span data-ttu-id="e09e9-139">string</span><span class="sxs-lookup"><span data-stu-id="e09e9-139">string</span></span>  | <span data-ttu-id="e09e9-140">Das Genre der Audiodatei</span><span class="sxs-lookup"><span data-stu-id="e09e9-140">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="e09e9-141">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="e09e9-141">**hasDrm**</span></span>            | <span data-ttu-id="e09e9-142">boolean</span><span class="sxs-lookup"><span data-stu-id="e09e9-142">boolean</span></span> | <span data-ttu-id="e09e9-143">Angabe, ob die Datei DRM-geschützt ist (Digital Rights Management, Verwaltung digitaler Rechte)</span><span class="sxs-lookup"><span data-stu-id="e09e9-143">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="e09e9-144">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="e09e9-144">**isVariableBitrate**</span></span> | <span data-ttu-id="e09e9-145">boolean</span><span class="sxs-lookup"><span data-stu-id="e09e9-145">boolean</span></span> | <span data-ttu-id="e09e9-146">Angabe, ob die Datei mit variabler Bitrate codiert ist</span><span class="sxs-lookup"><span data-stu-id="e09e9-146">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="e09e9-147">**title**</span><span class="sxs-lookup"><span data-stu-id="e09e9-147">**title**</span></span>             | <span data-ttu-id="e09e9-148">string</span><span class="sxs-lookup"><span data-stu-id="e09e9-148">string</span></span>  | <span data-ttu-id="e09e9-149">Der Titel der Audiodatei</span><span class="sxs-lookup"><span data-stu-id="e09e9-149">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="e09e9-150">**track**</span><span class="sxs-lookup"><span data-stu-id="e09e9-150">**track**</span></span>             | <span data-ttu-id="e09e9-151">Int32</span><span class="sxs-lookup"><span data-stu-id="e09e9-151">Int32</span></span>   | <span data-ttu-id="e09e9-152">Die Nummer des der Audiodatei entsprechenden Titels auf der Quell-CD</span><span class="sxs-lookup"><span data-stu-id="e09e9-152">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="e09e9-153">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="e09e9-153">**trackCount**</span></span>        | <span data-ttu-id="e09e9-154">Int32</span><span class="sxs-lookup"><span data-stu-id="e09e9-154">Int32</span></span>   | <span data-ttu-id="e09e9-155">Die Gesamtanzahl von Audiotiteln auf der Quell-CD der Audiodatei</span><span class="sxs-lookup"><span data-stu-id="e09e9-155">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="e09e9-156">**year**</span><span class="sxs-lookup"><span data-stu-id="e09e9-156">**year**</span></span>              | <span data-ttu-id="e09e9-157">Int32</span><span class="sxs-lookup"><span data-stu-id="e09e9-157">Int32</span></span>   | <span data-ttu-id="e09e9-158">Das Jahr, in dem die Audiodatei aufgenommen wurde</span><span class="sxs-lookup"><span data-stu-id="e09e9-158">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="e09e9-159">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="e09e9-159">Remarks</span></span>

<span data-ttu-id="e09e9-160">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="e09e9-160">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio"
} -->
