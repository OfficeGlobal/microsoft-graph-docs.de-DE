---
title: iPv6Range-Ressourcentyp
description: IPV6-Bereich
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 84d925cc7885dab4b3e87dbd62060894e741f52c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845746"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="5497b-103">iPv6Range-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5497b-103">iPv6Range resource type</span></span>

> <span data-ttu-id="5497b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5497b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5497b-105">IPV6-Bereich</span><span class="sxs-lookup"><span data-stu-id="5497b-105">IP V6 range</span></span>

<span data-ttu-id="5497b-106">Erbt von [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="5497b-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5497b-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5497b-107">Properties</span></span>
|<span data-ttu-id="5497b-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5497b-108">Property</span></span>|<span data-ttu-id="5497b-109">Typ</span><span class="sxs-lookup"><span data-stu-id="5497b-109">Type</span></span>|<span data-ttu-id="5497b-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5497b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5497b-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="5497b-111">lowerAddress</span></span>|<span data-ttu-id="5497b-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5497b-112">String</span></span>|<span data-ttu-id="5497b-113">Untere IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="5497b-113">Lower IP Address</span></span>|
|<span data-ttu-id="5497b-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="5497b-114">upperAddress</span></span>|<span data-ttu-id="5497b-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5497b-115">String</span></span>|<span data-ttu-id="5497b-116">Obere IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="5497b-116">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="5497b-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5497b-117">Relationships</span></span>
<span data-ttu-id="5497b-118">Keine</span><span class="sxs-lookup"><span data-stu-id="5497b-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5497b-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5497b-119">JSON Representation</span></span>
<span data-ttu-id="5497b-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5497b-120">Here is a JSON representation of the resource.</span></span>
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



