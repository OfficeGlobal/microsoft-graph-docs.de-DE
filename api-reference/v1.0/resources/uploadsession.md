---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: UploadSession
ms.openlocfilehash: 6c0ffebf0d973afe72ab82de9782c1f54e2342dd
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "20502123"
---
# <a name="uploadsession-resource"></a><span data-ttu-id="b3c47-102">UploadSession-Ressource</span><span class="sxs-lookup"><span data-stu-id="b3c47-102">UploadSession resource</span></span>

<span data-ttu-id="b3c47-103">Die **UploadSession**-Ressource enthält Informationen zum Hochladen von großen Dateien auf OneDrive, OneDrive for Business oder SharePoint-Dokumentbibliotheken.</span><span class="sxs-lookup"><span data-stu-id="b3c47-103">The **UploadSession** resource provides information about how to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3c47-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b3c47-104">JSON representation</span></span>

<span data-ttu-id="b3c47-105">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b3c47-105">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="b3c47-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b3c47-106">Properties</span></span>


| <span data-ttu-id="b3c47-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b3c47-107">Property</span></span>       | <span data-ttu-id="b3c47-108">Typ</span><span class="sxs-lookup"><span data-stu-id="b3c47-108">Type</span></span>              |<span data-ttu-id="b3c47-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b3c47-109">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="b3c47-110">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b3c47-110">expirationDateTime</span></span> | <span data-ttu-id="b3c47-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3c47-111">DateTimeOffset</span></span>    | <span data-ttu-id="b3c47-p101">Datum und Uhrzeit in UTC, wenn die Upload Sitzung abläuft. Die vollständige Datei muss hochgeladen werden, bevor dieser Ablaufzeitpunkt erreicht wird.</span><span class="sxs-lookup"><span data-stu-id="b3c47-p101">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="b3c47-114">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="b3c47-114">nextExpectedRanges</span></span> | <span data-ttu-id="b3c47-115">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="b3c47-115">String collection</span></span> | <span data-ttu-id="b3c47-p102">Eine Zusammenstellung von Bytebereichen, die dem Server für die Datei fehlen. Diese Bereiche sind Null indiziert und haben das Format "Anfang-Ende" (z. B. zeigt "0-26" die ersten 27 Bytes der Datei an).</span><span class="sxs-lookup"><span data-stu-id="b3c47-p102">A collection of byte ranges that the server is missing for the file. These ranges are zero indexed and of the format "start-end" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span>
| <span data-ttu-id="b3c47-118">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="b3c47-118">uploadUrl</span></span>          | <span data-ttu-id="b3c47-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b3c47-119">String</span></span>            | <span data-ttu-id="b3c47-120">Der URL-Endpunkt, der PUT-Anfragen für Bytebereiche der Datei akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="b3c47-120">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="b3c47-121">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="b3c47-121">See also</span></span>

- [<span data-ttu-id="b3c47-122">Hochladen großer Dateien mit einer Uploadsitzung</span><span class="sxs-lookup"><span data-stu-id="b3c47-122">Upload large files with an upload session</span></span>](../api/driveitem_createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->
