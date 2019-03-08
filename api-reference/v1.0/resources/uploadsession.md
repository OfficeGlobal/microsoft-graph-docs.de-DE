---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: UploadSession
localization_priority: Normal
ms.openlocfilehash: 3e97a6396f39db690be8a1cfe235bb21592da4e0
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481552"
---
# <a name="uploadsession-resource"></a><span data-ttu-id="a5630-102">UploadSession-Ressource</span><span class="sxs-lookup"><span data-stu-id="a5630-102">UploadSession resource</span></span>

<span data-ttu-id="a5630-103">Die **UploadSession**-Ressource enthält Informationen zum Hochladen von großen Dateien auf OneDrive, OneDrive for Business oder SharePoint-Dokumentbibliotheken.</span><span class="sxs-lookup"><span data-stu-id="a5630-103">The **UploadSession** resource provides information about how to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5630-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a5630-104">JSON representation</span></span>

<span data-ttu-id="a5630-105">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a5630-105">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "uploadUrl", "nextExpectedRanges" ],
  "@odata.type": "microsoft.graph.uploadSession"
}-->

```json
{
  "uploadUrl": "https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337",
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["0-"]
}
```

## <a name="properties"></a><span data-ttu-id="a5630-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a5630-106">Properties</span></span>


| <span data-ttu-id="a5630-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a5630-107">Property</span></span>       | <span data-ttu-id="a5630-108">Typ</span><span class="sxs-lookup"><span data-stu-id="a5630-108">Type</span></span>              |<span data-ttu-id="a5630-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a5630-109">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="a5630-110">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a5630-110">expirationDateTime</span></span> | <span data-ttu-id="a5630-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5630-111">DateTimeOffset</span></span>    | <span data-ttu-id="a5630-p101">Datum und Uhrzeit in UTC, wenn die Upload Sitzung abläuft. Die vollständige Datei muss hochgeladen werden, bevor dieser Ablaufzeitpunkt erreicht wird.</span><span class="sxs-lookup"><span data-stu-id="a5630-p101">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="a5630-114">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="a5630-114">nextExpectedRanges</span></span> | <span data-ttu-id="a5630-115">String collection</span><span class="sxs-lookup"><span data-stu-id="a5630-115">String collection</span></span> | <span data-ttu-id="a5630-p102">Eine Zusammenstellung von Bytebereichen, die dem Server für die Datei fehlen. Diese Bereiche sind Null indiziert und haben das Format "Anfang-Ende" (z. B. zeigt "0-26" die ersten 27 Bytes der Datei an).</span><span class="sxs-lookup"><span data-stu-id="a5630-p102">A collection of byte ranges that the server is missing for the file. These ranges are zero indexed and of the format "start-end" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span>
| <span data-ttu-id="a5630-118">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="a5630-118">uploadUrl</span></span>          | <span data-ttu-id="a5630-119">String</span><span class="sxs-lookup"><span data-stu-id="a5630-119">String</span></span>            | <span data-ttu-id="a5630-120">Der URL-Endpunkt, der PUT-Anfragen für Bytebereiche der Datei akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="a5630-120">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="a5630-121">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="a5630-121">See also</span></span>

- [<span data-ttu-id="a5630-122">Hochladen großer Dateien mit einer Uploadsitzung</span><span class="sxs-lookup"><span data-stu-id="a5630-122">Upload large files with an upload session</span></span>](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->
