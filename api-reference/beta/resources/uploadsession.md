---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: UploadSession
localization_priority: Normal
ms.openlocfilehash: c5d15c380908f09ef292b7c5794046bad6e95ac8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507950"
---
# <a name="uploadsession-resource"></a><span data-ttu-id="182cc-102">UploadSession-Ressource</span><span class="sxs-lookup"><span data-stu-id="182cc-102">UploadSession resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="182cc-103">Die **UploadSession**-Ressource enthält Informationen zum Hochladen von großen Dateien auf OneDrive, OneDrive for Business oder SharePoint-Dokumentbibliotheken.</span><span class="sxs-lookup"><span data-stu-id="182cc-103">The **UploadSession** resource provides information about how to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries.</span></span>

## <a name="json-representation"></a><span data-ttu-id="182cc-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="182cc-104">JSON representation</span></span>

<span data-ttu-id="182cc-105">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="182cc-105">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="182cc-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="182cc-106">Properties</span></span>


| <span data-ttu-id="182cc-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="182cc-107">Property</span></span>       | <span data-ttu-id="182cc-108">Typ</span><span class="sxs-lookup"><span data-stu-id="182cc-108">Type</span></span>              |<span data-ttu-id="182cc-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="182cc-109">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="182cc-110">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="182cc-110">expirationDateTime</span></span> | <span data-ttu-id="182cc-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="182cc-111">DateTimeOffset</span></span>    | <span data-ttu-id="182cc-p101">Datum und Uhrzeit in UTC, wenn die Upload Sitzung abläuft. Die vollständige Datei muss hochgeladen werden, bevor dieser Ablaufzeitpunkt erreicht wird.</span><span class="sxs-lookup"><span data-stu-id="182cc-p101">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="182cc-114">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="182cc-114">nextExpectedRanges</span></span> | <span data-ttu-id="182cc-115">String collection</span><span class="sxs-lookup"><span data-stu-id="182cc-115">String collection</span></span> | <span data-ttu-id="182cc-p102">Eine Zusammenstellung von Bytebereichen, die dem Server für die Datei fehlen. Diese Bereiche sind Null indiziert und haben das Format "Anfang-Ende" (z. B. zeigt "0-26" die ersten 27 Bytes der Datei an).</span><span class="sxs-lookup"><span data-stu-id="182cc-p102">A collection of byte ranges that the server is missing for the file. These ranges are zero indexed and of the format "start-end" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span>
| <span data-ttu-id="182cc-118">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="182cc-118">uploadUrl</span></span>          | <span data-ttu-id="182cc-119">String</span><span class="sxs-lookup"><span data-stu-id="182cc-119">String</span></span>            | <span data-ttu-id="182cc-120">Der URL-Endpunkt, der PUT-Anfragen für Bytebereiche der Datei akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="182cc-120">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="182cc-121">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="182cc-121">See also</span></span>

- <span data-ttu-id="182cc-122">Hochladen großer Dateien mit einer Uploadsitzung</span><span class="sxs-lookup"><span data-stu-id="182cc-122">[Upload large files with an upload session](../api/driveitem-createuploadsession.md)</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession",
  "suppressions": [
    "Error: /api-reference/beta/resources/uploadsession.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
