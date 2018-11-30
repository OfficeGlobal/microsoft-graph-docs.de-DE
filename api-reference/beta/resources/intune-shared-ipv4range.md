---
title: iPv4Range-Ressourcentyp
description: IP-V4-Bereich
ms.openlocfilehash: 9147bb45380ec8d207bf8b4f332efe5a370f3c07
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059223"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="ac6e6-103">iPv4Range-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ac6e6-103">iPv4Range resource type</span></span>

> <span data-ttu-id="ac6e6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ac6e6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ac6e6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ac6e6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ac6e6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ac6e6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ac6e6-107">IP-V4-Bereich</span><span class="sxs-lookup"><span data-stu-id="ac6e6-107">IP V4 range</span></span>

<span data-ttu-id="ac6e6-108">Erbt von [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="ac6e6-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ac6e6-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ac6e6-109">Properties</span></span>
|<span data-ttu-id="ac6e6-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ac6e6-110">Property</span></span>|<span data-ttu-id="ac6e6-111">Typ</span><span class="sxs-lookup"><span data-stu-id="ac6e6-111">Type</span></span>|<span data-ttu-id="ac6e6-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ac6e6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac6e6-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="ac6e6-113">lowerAddress</span></span>|<span data-ttu-id="ac6e6-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ac6e6-114">String</span></span>|<span data-ttu-id="ac6e6-115">Untere IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="ac6e6-115">Lower IP Address</span></span>|
|<span data-ttu-id="ac6e6-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="ac6e6-116">upperAddress</span></span>|<span data-ttu-id="ac6e6-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ac6e6-117">String</span></span>|<span data-ttu-id="ac6e6-118">Obere IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="ac6e6-118">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac6e6-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ac6e6-119">Relationships</span></span>
<span data-ttu-id="ac6e6-120">Keine</span><span class="sxs-lookup"><span data-stu-id="ac6e6-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac6e6-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ac6e6-121">JSON Representation</span></span>
<span data-ttu-id="ac6e6-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ac6e6-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iPv4Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv4Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



