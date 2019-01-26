---
author: VinodRavichandran
ms.date: 09/10/2017
title: Audio
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cd1f1af0e1ddcd1d56853c708da7ba03be740812
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573634"
---
# <a name="audio-facet"></a><span data-ttu-id="6994f-102">Facet „Audio“</span><span class="sxs-lookup"><span data-stu-id="6994f-102">Audio facet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6994f-103">Die Ressource **Audio** führt audiobezogene Eigenschaften für ein Element in einer einzelnen Struktur zusammen.</span><span class="sxs-lookup"><span data-stu-id="6994f-103">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="6994f-p101">Wenn ein [**DriveItem**](driveitem.md)-Element ein **file**-Facet ungleich Null aufweist, stellt das Element eine Audiodatei dar. Die Eigenschaften der **Audio**-Ressource werden durch Extrahieren von Metadaten aus der Datei aufgefüllt.</span><span class="sxs-lookup"><span data-stu-id="6994f-p101">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="6994f-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6994f-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="6994f-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6994f-107">Properties</span></span>

| <span data-ttu-id="6994f-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="6994f-108">Property name</span></span>         | <span data-ttu-id="6994f-109">Typ</span><span class="sxs-lookup"><span data-stu-id="6994f-109">Type</span></span>    | <span data-ttu-id="6994f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6994f-110">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="6994f-111">**album**</span><span class="sxs-lookup"><span data-stu-id="6994f-111">**album**</span></span>             | <span data-ttu-id="6994f-112">string</span><span class="sxs-lookup"><span data-stu-id="6994f-112">string</span></span>  | <span data-ttu-id="6994f-113">Der Titel des Albums, zu dem die Audiodatei gehört</span><span class="sxs-lookup"><span data-stu-id="6994f-113">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="6994f-114">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="6994f-114">**albumArtist**</span></span>       | <span data-ttu-id="6994f-115">string</span><span class="sxs-lookup"><span data-stu-id="6994f-115">string</span></span>  | <span data-ttu-id="6994f-116">Der Künstler, der für das Album genannt ist, zu dem die Audiodatei gehört</span><span class="sxs-lookup"><span data-stu-id="6994f-116">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="6994f-117">**artist**</span><span class="sxs-lookup"><span data-stu-id="6994f-117">**artist**</span></span>            | <span data-ttu-id="6994f-118">string</span><span class="sxs-lookup"><span data-stu-id="6994f-118">string</span></span>  | <span data-ttu-id="6994f-119">Der zur Audiodatei gehörende Künstler</span><span class="sxs-lookup"><span data-stu-id="6994f-119">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="6994f-120">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="6994f-120">**bitrate**</span></span>           | <span data-ttu-id="6994f-121">Int64</span><span class="sxs-lookup"><span data-stu-id="6994f-121">Int64</span></span>   | <span data-ttu-id="6994f-122">Die Bitrate in KBit/s</span><span class="sxs-lookup"><span data-stu-id="6994f-122">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="6994f-123">**composers**</span><span class="sxs-lookup"><span data-stu-id="6994f-123">**composers**</span></span>         | <span data-ttu-id="6994f-124">string</span><span class="sxs-lookup"><span data-stu-id="6994f-124">string</span></span>  | <span data-ttu-id="6994f-125">Der Name des Komponisten der Audiodatei</span><span class="sxs-lookup"><span data-stu-id="6994f-125">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="6994f-126">**copyright**</span><span class="sxs-lookup"><span data-stu-id="6994f-126">**copyright**</span></span>         | <span data-ttu-id="6994f-127">string</span><span class="sxs-lookup"><span data-stu-id="6994f-127">string</span></span>  | <span data-ttu-id="6994f-128">Urheberrechtsinformationen zur Audiodatei</span><span class="sxs-lookup"><span data-stu-id="6994f-128">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="6994f-129">**disc**</span><span class="sxs-lookup"><span data-stu-id="6994f-129">**disc**</span></span>              | <span data-ttu-id="6994f-130">Int16</span><span class="sxs-lookup"><span data-stu-id="6994f-130">Int16</span></span>   | <span data-ttu-id="6994f-131">Die Nummer der CD, von der die Audiodatei stammt</span><span class="sxs-lookup"><span data-stu-id="6994f-131">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="6994f-132">**discCount**</span><span class="sxs-lookup"><span data-stu-id="6994f-132">**discCount**</span></span>         | <span data-ttu-id="6994f-133">Int16</span><span class="sxs-lookup"><span data-stu-id="6994f-133">Int16</span></span>   | <span data-ttu-id="6994f-134">Die Gesamtanzahl von CDs im Album</span><span class="sxs-lookup"><span data-stu-id="6994f-134">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="6994f-135">**duration**</span><span class="sxs-lookup"><span data-stu-id="6994f-135">**duration**</span></span>          | <span data-ttu-id="6994f-136">Int64</span><span class="sxs-lookup"><span data-stu-id="6994f-136">Int64</span></span>   | <span data-ttu-id="6994f-137">Die Dauer der Audiodatei in Millisekunden</span><span class="sxs-lookup"><span data-stu-id="6994f-137">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="6994f-138">**genre**</span><span class="sxs-lookup"><span data-stu-id="6994f-138">**genre**</span></span>             | <span data-ttu-id="6994f-139">string</span><span class="sxs-lookup"><span data-stu-id="6994f-139">string</span></span>  | <span data-ttu-id="6994f-140">Das Genre der Audiodatei</span><span class="sxs-lookup"><span data-stu-id="6994f-140">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="6994f-141">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="6994f-141">**hasDrm**</span></span>            | <span data-ttu-id="6994f-142">boolean</span><span class="sxs-lookup"><span data-stu-id="6994f-142">boolean</span></span> | <span data-ttu-id="6994f-143">Angabe, ob die Datei DRM-geschützt ist (Digital Rights Management, Verwaltung digitaler Rechte)</span><span class="sxs-lookup"><span data-stu-id="6994f-143">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="6994f-144">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="6994f-144">**isVariableBitrate**</span></span> | <span data-ttu-id="6994f-145">boolean</span><span class="sxs-lookup"><span data-stu-id="6994f-145">boolean</span></span> | <span data-ttu-id="6994f-146">Angabe, ob die Datei mit variabler Bitrate codiert ist</span><span class="sxs-lookup"><span data-stu-id="6994f-146">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="6994f-147">**title**</span><span class="sxs-lookup"><span data-stu-id="6994f-147">**title**</span></span>             | <span data-ttu-id="6994f-148">string</span><span class="sxs-lookup"><span data-stu-id="6994f-148">string</span></span>  | <span data-ttu-id="6994f-149">Der Titel der Audiodatei</span><span class="sxs-lookup"><span data-stu-id="6994f-149">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="6994f-150">**track**</span><span class="sxs-lookup"><span data-stu-id="6994f-150">**track**</span></span>             | <span data-ttu-id="6994f-151">Int32</span><span class="sxs-lookup"><span data-stu-id="6994f-151">Int32</span></span>   | <span data-ttu-id="6994f-152">Die Nummer des der Audiodatei entsprechenden Titels auf der Quell-CD</span><span class="sxs-lookup"><span data-stu-id="6994f-152">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="6994f-153">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="6994f-153">**trackCount**</span></span>        | <span data-ttu-id="6994f-154">Int32</span><span class="sxs-lookup"><span data-stu-id="6994f-154">Int32</span></span>   | <span data-ttu-id="6994f-155">Die Gesamtanzahl von Audiotiteln auf der Quell-CD der Audiodatei</span><span class="sxs-lookup"><span data-stu-id="6994f-155">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="6994f-156">**year**</span><span class="sxs-lookup"><span data-stu-id="6994f-156">**year**</span></span>              | <span data-ttu-id="6994f-157">Int32</span><span class="sxs-lookup"><span data-stu-id="6994f-157">Int32</span></span>   | <span data-ttu-id="6994f-158">Das Jahr, in dem die Audiodatei aufgenommen wurde</span><span class="sxs-lookup"><span data-stu-id="6994f-158">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="6994f-159">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="6994f-159">Remarks</span></span>

<span data-ttu-id="6994f-160">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="6994f-160">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

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
