---
author: VinodRavichandran
ms.date: 09/10/2017
title: Audio
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b88fbbcd11a4cbeff56c870225d7b0bef4b32346
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985375"
---
# <a name="audio-facet"></a><span data-ttu-id="0ae58-102">Facet „Audio“</span><span class="sxs-lookup"><span data-stu-id="0ae58-102">Audio facet</span></span>

> <span data-ttu-id="0ae58-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0ae58-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ae58-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0ae58-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0ae58-105">Die Ressource **Audio** führt audiobezogene Eigenschaften für ein Element in einer einzelnen Struktur zusammen.</span><span class="sxs-lookup"><span data-stu-id="0ae58-105">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="0ae58-p102">Wenn ein [**DriveItem**](driveitem.md)-Element ein **file**-Facet ungleich Null aufweist, stellt das Element eine Audiodatei dar. Die Eigenschaften der **Audio**-Ressource werden durch Extrahieren von Metadaten aus der Datei aufgefüllt.</span><span class="sxs-lookup"><span data-stu-id="0ae58-p102">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="0ae58-108">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0ae58-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="0ae58-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0ae58-109">Properties</span></span>

| <span data-ttu-id="0ae58-110">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="0ae58-110">Property name</span></span>         | <span data-ttu-id="0ae58-111">Typ</span><span class="sxs-lookup"><span data-stu-id="0ae58-111">Type</span></span>    | <span data-ttu-id="0ae58-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0ae58-112">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="0ae58-113">**album**</span><span class="sxs-lookup"><span data-stu-id="0ae58-113">**album**</span></span>             | <span data-ttu-id="0ae58-114">string</span><span class="sxs-lookup"><span data-stu-id="0ae58-114">string</span></span>  | <span data-ttu-id="0ae58-115">Der Titel des Albums, zu dem die Audiodatei gehört</span><span class="sxs-lookup"><span data-stu-id="0ae58-115">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="0ae58-116">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="0ae58-116">**albumArtist**</span></span>       | <span data-ttu-id="0ae58-117">string</span><span class="sxs-lookup"><span data-stu-id="0ae58-117">string</span></span>  | <span data-ttu-id="0ae58-118">Der Künstler, der für das Album genannt ist, zu dem die Audiodatei gehört</span><span class="sxs-lookup"><span data-stu-id="0ae58-118">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="0ae58-119">**artist**</span><span class="sxs-lookup"><span data-stu-id="0ae58-119">**artist**</span></span>            | <span data-ttu-id="0ae58-120">string</span><span class="sxs-lookup"><span data-stu-id="0ae58-120">string</span></span>  | <span data-ttu-id="0ae58-121">Der zur Audiodatei gehörende Künstler</span><span class="sxs-lookup"><span data-stu-id="0ae58-121">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="0ae58-122">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="0ae58-122">**bitrate**</span></span>           | <span data-ttu-id="0ae58-123">Int32</span><span class="sxs-lookup"><span data-stu-id="0ae58-123">Int32</span></span>   | <span data-ttu-id="0ae58-124">Die Bitrate in KBit/s</span><span class="sxs-lookup"><span data-stu-id="0ae58-124">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="0ae58-125">**composers**</span><span class="sxs-lookup"><span data-stu-id="0ae58-125">**composers**</span></span>         | <span data-ttu-id="0ae58-126">string</span><span class="sxs-lookup"><span data-stu-id="0ae58-126">string</span></span>  | <span data-ttu-id="0ae58-127">Der Name des Komponisten der Audiodatei</span><span class="sxs-lookup"><span data-stu-id="0ae58-127">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="0ae58-128">**copyright**</span><span class="sxs-lookup"><span data-stu-id="0ae58-128">**copyright**</span></span>         | <span data-ttu-id="0ae58-129">string</span><span class="sxs-lookup"><span data-stu-id="0ae58-129">string</span></span>  | <span data-ttu-id="0ae58-130">Urheberrechtsinformationen zur Audiodatei</span><span class="sxs-lookup"><span data-stu-id="0ae58-130">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="0ae58-131">**disc**</span><span class="sxs-lookup"><span data-stu-id="0ae58-131">**disc**</span></span>              | <span data-ttu-id="0ae58-132">Int32</span><span class="sxs-lookup"><span data-stu-id="0ae58-132">Int32</span></span>   | <span data-ttu-id="0ae58-133">Die Nummer der CD, von der die Audiodatei stammt</span><span class="sxs-lookup"><span data-stu-id="0ae58-133">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="0ae58-134">**discCount**</span><span class="sxs-lookup"><span data-stu-id="0ae58-134">**discCount**</span></span>         | <span data-ttu-id="0ae58-135">Int32</span><span class="sxs-lookup"><span data-stu-id="0ae58-135">Int32</span></span>   | <span data-ttu-id="0ae58-136">Die Gesamtanzahl von CDs im Album</span><span class="sxs-lookup"><span data-stu-id="0ae58-136">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="0ae58-137">**duration**</span><span class="sxs-lookup"><span data-stu-id="0ae58-137">**duration**</span></span>          | <span data-ttu-id="0ae58-138">Int64</span><span class="sxs-lookup"><span data-stu-id="0ae58-138">Int64</span></span>   | <span data-ttu-id="0ae58-139">Die Dauer der Audiodatei in Millisekunden</span><span class="sxs-lookup"><span data-stu-id="0ae58-139">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="0ae58-140">**genre**</span><span class="sxs-lookup"><span data-stu-id="0ae58-140">**genre**</span></span>             | <span data-ttu-id="0ae58-141">string</span><span class="sxs-lookup"><span data-stu-id="0ae58-141">string</span></span>  | <span data-ttu-id="0ae58-142">Das Genre der Audiodatei</span><span class="sxs-lookup"><span data-stu-id="0ae58-142">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="0ae58-143">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="0ae58-143">**hasDrm**</span></span>            | <span data-ttu-id="0ae58-144">boolean</span><span class="sxs-lookup"><span data-stu-id="0ae58-144">boolean</span></span> | <span data-ttu-id="0ae58-145">Angabe, ob die Datei DRM-geschützt ist (Digital Rights Management, Verwaltung digitaler Rechte)</span><span class="sxs-lookup"><span data-stu-id="0ae58-145">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="0ae58-146">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="0ae58-146">**isVariableBitrate**</span></span> | <span data-ttu-id="0ae58-147">boolean</span><span class="sxs-lookup"><span data-stu-id="0ae58-147">boolean</span></span> | <span data-ttu-id="0ae58-148">Angabe, ob die Datei mit variabler Bitrate codiert ist</span><span class="sxs-lookup"><span data-stu-id="0ae58-148">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="0ae58-149">**title**</span><span class="sxs-lookup"><span data-stu-id="0ae58-149">**title**</span></span>             | <span data-ttu-id="0ae58-150">string</span><span class="sxs-lookup"><span data-stu-id="0ae58-150">string</span></span>  | <span data-ttu-id="0ae58-151">Der Titel der Audiodatei</span><span class="sxs-lookup"><span data-stu-id="0ae58-151">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="0ae58-152">**track**</span><span class="sxs-lookup"><span data-stu-id="0ae58-152">**track**</span></span>             | <span data-ttu-id="0ae58-153">Int32</span><span class="sxs-lookup"><span data-stu-id="0ae58-153">Int32</span></span>   | <span data-ttu-id="0ae58-154">Die Nummer des der Audiodatei entsprechenden Titels auf der Quell-CD</span><span class="sxs-lookup"><span data-stu-id="0ae58-154">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="0ae58-155">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="0ae58-155">**trackCount**</span></span>        | <span data-ttu-id="0ae58-156">Int32</span><span class="sxs-lookup"><span data-stu-id="0ae58-156">Int32</span></span>   | <span data-ttu-id="0ae58-157">Die Gesamtanzahl von Audiotiteln auf der Quell-CD der Audiodatei</span><span class="sxs-lookup"><span data-stu-id="0ae58-157">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="0ae58-158">**year**</span><span class="sxs-lookup"><span data-stu-id="0ae58-158">**year**</span></span>              | <span data-ttu-id="0ae58-159">Int32</span><span class="sxs-lookup"><span data-stu-id="0ae58-159">Int32</span></span>   | <span data-ttu-id="0ae58-160">Das Jahr, in dem die Audiodatei aufgenommen wurde</span><span class="sxs-lookup"><span data-stu-id="0ae58-160">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="0ae58-161">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="0ae58-161">Remarks</span></span>

<span data-ttu-id="0ae58-162">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="0ae58-162">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio"
} -->
