---
title: iPv6Range-Ressourcentyp
description: IPV6-Bereich
author: tfitzmac
ms.openlocfilehash: b5a2ad772d45b4be5fa3a8f4da04b28bc965195d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337548"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="b5573-103">iPv6Range-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b5573-103">iPv6Range resource type</span></span>

> <span data-ttu-id="b5573-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b5573-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5573-105">IPV6-Bereich</span><span class="sxs-lookup"><span data-stu-id="b5573-105">IP V6 range</span></span>

<span data-ttu-id="b5573-106">Erbt von [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="b5573-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b5573-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b5573-107">Properties</span></span>
|<span data-ttu-id="b5573-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b5573-108">Property</span></span>|<span data-ttu-id="b5573-109">Typ</span><span class="sxs-lookup"><span data-stu-id="b5573-109">Type</span></span>|<span data-ttu-id="b5573-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5573-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5573-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="b5573-111">lowerAddress</span></span>|<span data-ttu-id="b5573-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b5573-112">String</span></span>|<span data-ttu-id="b5573-113">Untere IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="b5573-113">Lower IP Address</span></span>|
|<span data-ttu-id="b5573-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="b5573-114">upperAddress</span></span>|<span data-ttu-id="b5573-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b5573-115">String</span></span>|<span data-ttu-id="b5573-116">Obere IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="b5573-116">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5573-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b5573-117">Relationships</span></span>
<span data-ttu-id="b5573-118">Keine</span><span class="sxs-lookup"><span data-stu-id="b5573-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b5573-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b5573-119">JSON Representation</span></span>
<span data-ttu-id="b5573-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b5573-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv6Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv6Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



