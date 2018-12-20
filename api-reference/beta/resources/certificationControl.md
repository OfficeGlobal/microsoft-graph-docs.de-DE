---
title: " Ressourcentyp certificationControl"
description: Diese Ressource enthält Compliance Zertifizierung zugeordnete Daten secure Score-Steuerelement.
ms.openlocfilehash: 62b6627a9bb1a012d6d7e542d87abbaddb0e279a
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380945"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="eadf7-103">Ressourcentyp certificationControl</span><span class="sxs-lookup"><span data-stu-id="eadf7-103">certificationControl resource type</span></span>

<span data-ttu-id="eadf7-104">Enthält Compliance Zertifizierung zugeordnete Daten secure Score-Steuerelement.</span><span class="sxs-lookup"><span data-stu-id="eadf7-104">Contains compliance certification data associated with secure score control.</span></span>

|<span data-ttu-id="eadf7-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eadf7-105">Property</span></span> |<span data-ttu-id="eadf7-106">Typ</span><span class="sxs-lookup"><span data-stu-id="eadf7-106">Type</span></span> |<span data-ttu-id="eadf7-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eadf7-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="eadf7-108">name</span><span class="sxs-lookup"><span data-stu-id="eadf7-108">name</span></span> | <span data-ttu-id="eadf7-109">string</span><span class="sxs-lookup"><span data-stu-id="eadf7-109">string</span></span> | <span data-ttu-id="eadf7-110">Steuerelementname Zertifizierung (engl.)</span><span class="sxs-lookup"><span data-stu-id="eadf7-110">Certification control name</span></span> |
|<span data-ttu-id="eadf7-111">url</span><span class="sxs-lookup"><span data-stu-id="eadf7-111">url</span></span> | <span data-ttu-id="eadf7-112">string</span><span class="sxs-lookup"><span data-stu-id="eadf7-112">string</span></span> | <span data-ttu-id="eadf7-113">URL für den Microsoft-Dienst vertrauen Portal</span><span class="sxs-lookup"><span data-stu-id="eadf7-113">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="eadf7-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="eadf7-114">JSON representation</span></span>

<span data-ttu-id="eadf7-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="eadf7-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificationControl"
}-->

```json
{
  "name": "String",
  "url": "Collection(microsoft.graph.certificationControl)"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "certificationControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
