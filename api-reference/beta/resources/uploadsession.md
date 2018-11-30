---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: UploadSession
ms.openlocfilehash: 27e3b448b54df0a5d35e2992391a554b73fd2c42
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066075"
---
# <a name="uploadsession-resource"></a><span data-ttu-id="7bcc1-102">UploadSession-Ressource</span><span class="sxs-lookup"><span data-stu-id="7bcc1-102">UploadSession resource</span></span>

> <span data-ttu-id="7bcc1-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7bcc1-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7bcc1-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7bcc1-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7bcc1-105">Die **UploadSession**-Ressource enthält Informationen zum Hochladen von großen Dateien auf OneDrive, OneDrive for Business oder SharePoint-Dokumentbibliotheken.</span><span class="sxs-lookup"><span data-stu-id="7bcc1-105">The **UploadSession** resource provides information about how to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7bcc1-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7bcc1-106">JSON representation</span></span>

<span data-ttu-id="7bcc1-107">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7bcc1-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="7bcc1-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7bcc1-108">Properties</span></span>


| <span data-ttu-id="7bcc1-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7bcc1-109">Property</span></span>       | <span data-ttu-id="7bcc1-110">Typ</span><span class="sxs-lookup"><span data-stu-id="7bcc1-110">Type</span></span>              |<span data-ttu-id="7bcc1-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7bcc1-111">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="7bcc1-112">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7bcc1-112">expirationDateTime</span></span> | <span data-ttu-id="7bcc1-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bcc1-113">DateTimeOffset</span></span>    | <span data-ttu-id="7bcc1-p102">Datum und Uhrzeit in UTC, wenn die Upload Sitzung abläuft. Die vollständige Datei muss hochgeladen werden, bevor dieser Ablaufzeitpunkt erreicht wird.</span><span class="sxs-lookup"><span data-stu-id="7bcc1-p102">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="7bcc1-116">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="7bcc1-116">nextExpectedRanges</span></span> | <span data-ttu-id="7bcc1-117">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="7bcc1-117">String collection</span></span> | <span data-ttu-id="7bcc1-p103">Eine Zusammenstellung von Bytebereichen, die dem Server für die Datei fehlen. Diese Bereiche sind Null indiziert und haben das Format "Anfang-Ende" (z. B. zeigt "0-26" die ersten 27 Bytes der Datei an).</span><span class="sxs-lookup"><span data-stu-id="7bcc1-p103">A collection of byte ranges that the server is missing for the file. These ranges are zero indexed and of the format "start-end" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span>
| <span data-ttu-id="7bcc1-120">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="7bcc1-120">uploadUrl</span></span>          | <span data-ttu-id="7bcc1-121">String</span><span class="sxs-lookup"><span data-stu-id="7bcc1-121">String</span></span>            | <span data-ttu-id="7bcc1-122">Der URL-Endpunkt, der PUT-Anfragen für Bytebereiche der Datei akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="7bcc1-122">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="7bcc1-123">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="7bcc1-123">See also</span></span>

- [<span data-ttu-id="7bcc1-124">Hochladen großer Dateien mit einer Uploadsitzung</span><span class="sxs-lookup"><span data-stu-id="7bcc1-124">Upload large files with an upload session</span></span>](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->
