---
author: VinodRavichandran
ms.date: 09/10/2017
title: Audio
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b4ff9e98b3024184298da144f90665ba2f192fef
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527033"
---
# <a name="audio-facet"></a><span data-ttu-id="0e973-102">Facet „Audio“</span><span class="sxs-lookup"><span data-stu-id="0e973-102">Audio facet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e973-103">Die Ressource **Audio** führt audiobezogene Eigenschaften für ein Element in einer einzelnen Struktur zusammen.</span><span class="sxs-lookup"><span data-stu-id="0e973-103">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="0e973-p101">Wenn ein DriveItem-Element ein file-Facet ungleich Null aufweist, stellt das Element eine Audiodatei dar. Die Eigenschaften der Audio-Ressource werden durch Extrahieren von Metadaten aus der Datei aufgefüllt.</span><span class="sxs-lookup"><span data-stu-id="0e973-p101">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="0e973-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0e973-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="0e973-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0e973-107">Properties</span></span>

| <span data-ttu-id="0e973-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="0e973-108">Property name</span></span>         | <span data-ttu-id="0e973-109">Typ</span><span class="sxs-lookup"><span data-stu-id="0e973-109">Type</span></span>    | <span data-ttu-id="0e973-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e973-110">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="0e973-111">**album**</span><span class="sxs-lookup"><span data-stu-id="0e973-111">**album**</span></span>             | <span data-ttu-id="0e973-112">string</span><span class="sxs-lookup"><span data-stu-id="0e973-112">string</span></span>  | <span data-ttu-id="0e973-113">Der Titel des Albums, zu dem die Audiodatei gehört</span><span class="sxs-lookup"><span data-stu-id="0e973-113">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="0e973-114">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="0e973-114">**albumArtist**</span></span>       | <span data-ttu-id="0e973-115">string</span><span class="sxs-lookup"><span data-stu-id="0e973-115">string</span></span>  | <span data-ttu-id="0e973-116">Der Künstler, der für das Album genannt ist, zu dem die Audiodatei gehört</span><span class="sxs-lookup"><span data-stu-id="0e973-116">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="0e973-117">**artist**</span><span class="sxs-lookup"><span data-stu-id="0e973-117">**artist**</span></span>            | <span data-ttu-id="0e973-118">string</span><span class="sxs-lookup"><span data-stu-id="0e973-118">string</span></span>  | <span data-ttu-id="0e973-119">Der zur Audiodatei gehörende Künstler</span><span class="sxs-lookup"><span data-stu-id="0e973-119">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="0e973-120">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="0e973-120">**bitrate**</span></span>           | <span data-ttu-id="0e973-121">Int32</span><span class="sxs-lookup"><span data-stu-id="0e973-121">Int32</span></span>   | <span data-ttu-id="0e973-122">Die Bitrate in KBit/s</span><span class="sxs-lookup"><span data-stu-id="0e973-122">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="0e973-123">**composers**</span><span class="sxs-lookup"><span data-stu-id="0e973-123">**composers**</span></span>         | <span data-ttu-id="0e973-124">string</span><span class="sxs-lookup"><span data-stu-id="0e973-124">string</span></span>  | <span data-ttu-id="0e973-125">Der Name des Komponisten der Audiodatei</span><span class="sxs-lookup"><span data-stu-id="0e973-125">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="0e973-126">**copyright**</span><span class="sxs-lookup"><span data-stu-id="0e973-126">**copyright**</span></span>         | <span data-ttu-id="0e973-127">string</span><span class="sxs-lookup"><span data-stu-id="0e973-127">string</span></span>  | <span data-ttu-id="0e973-128">Urheberrechtsinformationen zur Audiodatei</span><span class="sxs-lookup"><span data-stu-id="0e973-128">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="0e973-129">**disc**</span><span class="sxs-lookup"><span data-stu-id="0e973-129">**disc**</span></span>              | <span data-ttu-id="0e973-130">Int32</span><span class="sxs-lookup"><span data-stu-id="0e973-130">Int32</span></span>   | <span data-ttu-id="0e973-131">Die Nummer der CD, von der die Audiodatei stammt</span><span class="sxs-lookup"><span data-stu-id="0e973-131">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="0e973-132">**discCount**</span><span class="sxs-lookup"><span data-stu-id="0e973-132">**discCount**</span></span>         | <span data-ttu-id="0e973-133">Int32</span><span class="sxs-lookup"><span data-stu-id="0e973-133">Int32</span></span>   | <span data-ttu-id="0e973-134">Die Gesamtanzahl von CDs im Album</span><span class="sxs-lookup"><span data-stu-id="0e973-134">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="0e973-135">**duration**</span><span class="sxs-lookup"><span data-stu-id="0e973-135">**duration**</span></span>          | <span data-ttu-id="0e973-136">Int64</span><span class="sxs-lookup"><span data-stu-id="0e973-136">Int64</span></span>   | <span data-ttu-id="0e973-137">Die Dauer der Audiodatei in Millisekunden</span><span class="sxs-lookup"><span data-stu-id="0e973-137">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="0e973-138">**genre**</span><span class="sxs-lookup"><span data-stu-id="0e973-138">**genre**</span></span>             | <span data-ttu-id="0e973-139">string</span><span class="sxs-lookup"><span data-stu-id="0e973-139">string</span></span>  | <span data-ttu-id="0e973-140">Das Genre der Audiodatei</span><span class="sxs-lookup"><span data-stu-id="0e973-140">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="0e973-141">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="0e973-141">**hasDrm**</span></span>            | <span data-ttu-id="0e973-142">boolean</span><span class="sxs-lookup"><span data-stu-id="0e973-142">boolean</span></span> | <span data-ttu-id="0e973-143">Angabe, ob die Datei DRM-geschützt ist (Digital Rights Management, Verwaltung digitaler Rechte)</span><span class="sxs-lookup"><span data-stu-id="0e973-143">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="0e973-144">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="0e973-144">**isVariableBitrate**</span></span> | <span data-ttu-id="0e973-145">boolean</span><span class="sxs-lookup"><span data-stu-id="0e973-145">boolean</span></span> | <span data-ttu-id="0e973-146">Angabe, ob die Datei mit variabler Bitrate codiert ist</span><span class="sxs-lookup"><span data-stu-id="0e973-146">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="0e973-147">**title**</span><span class="sxs-lookup"><span data-stu-id="0e973-147">**title**</span></span>             | <span data-ttu-id="0e973-148">string</span><span class="sxs-lookup"><span data-stu-id="0e973-148">string</span></span>  | <span data-ttu-id="0e973-149">Der Titel der Audiodatei</span><span class="sxs-lookup"><span data-stu-id="0e973-149">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="0e973-150">**track**</span><span class="sxs-lookup"><span data-stu-id="0e973-150">**track**</span></span>             | <span data-ttu-id="0e973-151">Int32</span><span class="sxs-lookup"><span data-stu-id="0e973-151">Int32</span></span>   | <span data-ttu-id="0e973-152">Die Nummer des der Audiodatei entsprechenden Titels auf der Quell-CD</span><span class="sxs-lookup"><span data-stu-id="0e973-152">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="0e973-153">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="0e973-153">**trackCount**</span></span>        | <span data-ttu-id="0e973-154">Int32</span><span class="sxs-lookup"><span data-stu-id="0e973-154">Int32</span></span>   | <span data-ttu-id="0e973-155">Die Gesamtanzahl von Audiotiteln auf der Quell-CD der Audiodatei</span><span class="sxs-lookup"><span data-stu-id="0e973-155">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="0e973-156">**year**</span><span class="sxs-lookup"><span data-stu-id="0e973-156">**year**</span></span>              | <span data-ttu-id="0e973-157">Int32</span><span class="sxs-lookup"><span data-stu-id="0e973-157">Int32</span></span>   | <span data-ttu-id="0e973-158">Das Jahr, in dem die Audiodatei aufgenommen wurde</span><span class="sxs-lookup"><span data-stu-id="0e973-158">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="0e973-159">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="0e973-159">Remarks</span></span>

<span data-ttu-id="0e973-160">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="0e973-160">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio",
  "suppressions": [
    "Error: /api-reference/beta/resources/audio.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
