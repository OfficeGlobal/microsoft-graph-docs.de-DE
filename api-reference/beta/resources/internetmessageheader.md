---
title: internetMessageHeader-Ressourcentyp
description: 'Schlüssel-Wert-Paar, die eine Internet-Nachrichtenkopfzeile darstellt, wie durch RFC5322, definiert, die bereitstellt '
ms.openlocfilehash: 420d39b6a139563e3f5f277f032f0f7a29252337
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061244"
---
# <a name="internetmessageheader-resource-type"></a><span data-ttu-id="a9206-103">internetMessageHeader-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a9206-103">internetMessageHeader resource type</span></span>

> <span data-ttu-id="a9206-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a9206-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9206-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a9206-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a9206-106">Ein Schlüssel-Wert-Paar, das eine Internet-Nachrichtenkopfzeile darstellt, wie von [RFC5322](https://www.ietf.org/rfc/rfc5322.txt) definiert, die Informationen zum Netzwerkpfad einer Nachricht vom Absender bis zum Empfänger liefert.</span><span class="sxs-lookup"><span data-stu-id="a9206-106">A key-value pair that represents an Internet message header, as defined by [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), that provides details of the network path taken by a message from the sender to the recipient.</span></span> 

<span data-ttu-id="a9206-107">Beispiele für eine Internet-Nachrichtenkopfzeile finden Sie unter [Anzeigen E-Mail-Kopfzeilen](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span><span class="sxs-lookup"><span data-stu-id="a9206-107">For examples of an Internet message header, see [View e-mail message headers](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span></span>


## <a name="properties"></a><span data-ttu-id="a9206-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a9206-108">Properties</span></span>
| <span data-ttu-id="a9206-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a9206-109">Property</span></span>     | <span data-ttu-id="a9206-110">Typ</span><span class="sxs-lookup"><span data-stu-id="a9206-110">Type</span></span>   |<span data-ttu-id="a9206-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a9206-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9206-112">name</span><span class="sxs-lookup"><span data-stu-id="a9206-112">name</span></span>|<span data-ttu-id="a9206-113">string</span><span class="sxs-lookup"><span data-stu-id="a9206-113">string</span></span>|<span data-ttu-id="a9206-114">Stellt den Schlüssel in einem Schlüssel-Wert-Paar dar.</span><span class="sxs-lookup"><span data-stu-id="a9206-114">Represents the key in a key-value pair.</span></span>|
|<span data-ttu-id="a9206-115">Wert</span><span class="sxs-lookup"><span data-stu-id="a9206-115">value</span></span>|<span data-ttu-id="a9206-116">string</span><span class="sxs-lookup"><span data-stu-id="a9206-116">string</span></span>|<span data-ttu-id="a9206-117">Der Wert in einem Schlüssel-Wert-Paar.</span><span class="sxs-lookup"><span data-stu-id="a9206-117">The value in a key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a9206-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a9206-118">JSON representation</span></span>

<span data-ttu-id="a9206-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a9206-119">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "internetMessageHeader resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->