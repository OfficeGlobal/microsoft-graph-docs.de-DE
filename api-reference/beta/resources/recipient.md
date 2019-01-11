---
title: recipient-Ressourcentyp
description: 'Stellt Informationen zu einem Benutzer am sendenden oder empfangenden Ende eines Ereignisses, einer Nachricht oder einer Gruppenveröffentlichung dar. '
localization_priority: Normal
ms.openlocfilehash: b234cac0526ee66a59a19f7059dbebdc8a1bdcb3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848377"
---
# <a name="recipient-resource-type"></a><span data-ttu-id="59bcc-103">recipient-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="59bcc-103">recipient resource type</span></span>

> <span data-ttu-id="59bcc-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="59bcc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="59bcc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="59bcc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="59bcc-106">Stellt Informationen zu einem Benutzer am sendenden oder empfangenden Ende eines Ereignisses, einer Nachricht oder einer Gruppenveröffentlichung dar.</span><span class="sxs-lookup"><span data-stu-id="59bcc-106">Represents information about a user in the sending or receiving end of an event, message or group post.</span></span> 

## <a name="properties"></a><span data-ttu-id="59bcc-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="59bcc-107">Properties</span></span>
| <span data-ttu-id="59bcc-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="59bcc-108">Property</span></span>     | <span data-ttu-id="59bcc-109">Typ</span><span class="sxs-lookup"><span data-stu-id="59bcc-109">Type</span></span>   |<span data-ttu-id="59bcc-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="59bcc-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59bcc-111">emailAddress</span><span class="sxs-lookup"><span data-stu-id="59bcc-111">emailAddress</span></span>|[<span data-ttu-id="59bcc-112">EmailAddress</span><span class="sxs-lookup"><span data-stu-id="59bcc-112">EmailAddress</span></span>](emailaddress.md)|<span data-ttu-id="59bcc-113">Die E-Mail-Adresse des Empfängers.</span><span class="sxs-lookup"><span data-stu-id="59bcc-113">The recipient's email address.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="59bcc-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="59bcc-114">JSON representation</span></span>

<span data-ttu-id="59bcc-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="59bcc-115">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recipient"
}-->

```json
{
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
