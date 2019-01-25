---
title: internetMessageHeader-Ressourcentyp
description: 'Schlüssel-Wert-Paar, die eine Internet-Nachrichtenkopfzeile darstellt, wie durch RFC5322, definiert, die bereitstellt '
localization_priority: Normal
ms.openlocfilehash: e748e6badd3e6bad6adb02a9df46a40a7241d636
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511667"
---
# <a name="internetmessageheader-resource-type"></a><span data-ttu-id="07c24-103">internetMessageHeader-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="07c24-103">internetMessageHeader resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07c24-104">Ein Schlüssel-Wert-Paar, das eine Internet-Nachrichtenkopfzeile darstellt, wie von [RFC5322](https://www.ietf.org/rfc/rfc5322.txt) definiert, die Informationen zum Netzwerkpfad einer Nachricht vom Absender bis zum Empfänger liefert.</span><span class="sxs-lookup"><span data-stu-id="07c24-104">A key-value pair that represents an Internet message header, as defined by [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), that provides details of the network path taken by a message from the sender to the recipient.</span></span> 

<span data-ttu-id="07c24-105">Beispiele für eine Internet-Nachrichtenkopfzeile finden Sie unter [Anzeigen E-Mail-Kopfzeilen](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span><span class="sxs-lookup"><span data-stu-id="07c24-105">For examples of an Internet message header, see [View e-mail message headers](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span></span>


## <a name="properties"></a><span data-ttu-id="07c24-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="07c24-106">Properties</span></span>
| <span data-ttu-id="07c24-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="07c24-107">Property</span></span>     | <span data-ttu-id="07c24-108">Typ</span><span class="sxs-lookup"><span data-stu-id="07c24-108">Type</span></span>   |<span data-ttu-id="07c24-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07c24-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07c24-110">name</span><span class="sxs-lookup"><span data-stu-id="07c24-110">name</span></span>|<span data-ttu-id="07c24-111">string</span><span class="sxs-lookup"><span data-stu-id="07c24-111">string</span></span>|<span data-ttu-id="07c24-112">Stellt den Schlüssel in einem Schlüssel-Wert-Paar dar.</span><span class="sxs-lookup"><span data-stu-id="07c24-112">Represents the key in a key-value pair.</span></span>|
|<span data-ttu-id="07c24-113">Wert</span><span class="sxs-lookup"><span data-stu-id="07c24-113">value</span></span>|<span data-ttu-id="07c24-114">string</span><span class="sxs-lookup"><span data-stu-id="07c24-114">string</span></span>|<span data-ttu-id="07c24-115">Der Wert in einem Schlüssel-Wert-Paar.</span><span class="sxs-lookup"><span data-stu-id="07c24-115">The value in a key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="07c24-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="07c24-116">JSON representation</span></span>

<span data-ttu-id="07c24-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="07c24-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.internetMessageHeader"
}-->

```json
{
  "name": "string",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "internetMessageHeader resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/internetmessageheader.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
