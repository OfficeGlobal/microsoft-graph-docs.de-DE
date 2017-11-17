---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: UploadSession
ms.openlocfilehash: d84b588c28791ab8f1cf6cef1be6af767fa18e47
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="uploadsession-resource"></a><span data-ttu-id="ccb0c-102">UploadSession-Ressource</span><span class="sxs-lookup"><span data-stu-id="ccb0c-102">UploadSession resource</span></span>

<span data-ttu-id="ccb0c-103">Die **UploadSession**-Ressource enthält Informationen zum Hochladen von großen Dateien auf OneDrive, OneDrive for Business oder SharePoint-Dokumentbibliotheken.</span><span class="sxs-lookup"><span data-stu-id="ccb0c-103">The **UploadSession** resource provides information about how to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ccb0c-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ccb0c-104">JSON representation</span></span>

<span data-ttu-id="ccb0c-105">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ccb0c-105">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="ccb0c-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ccb0c-106">Properties</span></span>


| <span data-ttu-id="ccb0c-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ccb0c-107">Property</span></span>       | <span data-ttu-id="ccb0c-108">Typ</span><span class="sxs-lookup"><span data-stu-id="ccb0c-108">Type</span></span>              |<span data-ttu-id="ccb0c-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ccb0c-109">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="ccb0c-110">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ccb0c-110">expirationDateTime</span></span> | <span data-ttu-id="ccb0c-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccb0c-111">DateTimeOffset</span></span>    | <span data-ttu-id="ccb0c-p101">Datum und Uhrzeit in UTC, wenn die Upload Sitzung abläuft. Die vollständige Datei muss hochgeladen werden, bevor dieser Ablaufzeitpunkt erreicht wird.</span><span class="sxs-lookup"><span data-stu-id="ccb0c-p101">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="ccb0c-114">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="ccb0c-114">nextExpectedRanges</span></span> | <span data-ttu-id="ccb0c-115">String collection</span><span class="sxs-lookup"><span data-stu-id="ccb0c-115">String collection</span></span> | <span data-ttu-id="ccb0c-p102">Eine Zusammenstellung von Bytebereichen, die dem Server für die Datei fehlen. Diese Bereiche sind Null indiziert und haben das Format "Anfang-Ende" (z. B. zeigt "0-26" die ersten 27 Bytes der Datei an).</span><span class="sxs-lookup"><span data-stu-id="ccb0c-p102">A collection of byte ranges that the server is missing for the file. These ranges are zero indexed and of the format "start-end" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span>
| <span data-ttu-id="ccb0c-118">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="ccb0c-118">uploadUrl</span></span>          | <span data-ttu-id="ccb0c-119">String</span><span class="sxs-lookup"><span data-stu-id="ccb0c-119">String</span></span>            | <span data-ttu-id="ccb0c-120">Der URL-Endpunkt, der PUT-Anfragen für Bytebereiche der Datei akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="ccb0c-120">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="additional-resources"></a><span data-ttu-id="ccb0c-121">Zusätzliche Ressourcen</span><span class="sxs-lookup"><span data-stu-id="ccb0c-121">Additional Resources</span></span>

<span data-ttu-id="ccb0c-122">Unter [Hochladen große Dateien mit einer Upload-Sitzung](../api/driveitem_createuploadsession.md) finden Sie Details zum Hochladen von Dateien mit einer Sitzung.</span><span class="sxs-lookup"><span data-stu-id="ccb0c-122">See [Upload large files with an upload session](../api/driveitem_createuploadsession.md) for details on how to upload files using an upload session.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->
