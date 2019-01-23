---
title: iPv4Range-Ressourcentyp
description: Beschreibt die iPv4Range Ressource die Microsoft Graph-API für Intune, die mehrere Workflows unterstützt.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9ac2656b7c79cceba70879fe478aec65a5bd7250
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425225"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="8278c-103">iPv4Range-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8278c-103">iPv4Range resource type</span></span>

> <span data-ttu-id="8278c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8278c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8278c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8278c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8278c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8278c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8278c-107">IP-V4-Bereich</span><span class="sxs-lookup"><span data-stu-id="8278c-107">IP V4 range</span></span>

<span data-ttu-id="8278c-108">Erbt von [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="8278c-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8278c-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8278c-109">Properties</span></span>
|<span data-ttu-id="8278c-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8278c-110">Property</span></span>|<span data-ttu-id="8278c-111">Typ</span><span class="sxs-lookup"><span data-stu-id="8278c-111">Type</span></span>|<span data-ttu-id="8278c-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8278c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8278c-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="8278c-113">lowerAddress</span></span>|<span data-ttu-id="8278c-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8278c-114">String</span></span>|<span data-ttu-id="8278c-115">Untere IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="8278c-115">Lower IP Address</span></span>|
|<span data-ttu-id="8278c-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="8278c-116">upperAddress</span></span>|<span data-ttu-id="8278c-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8278c-117">String</span></span>|<span data-ttu-id="8278c-118">Obere IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="8278c-118">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="8278c-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8278c-119">Relationships</span></span>
<span data-ttu-id="8278c-120">Keine</span><span class="sxs-lookup"><span data-stu-id="8278c-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8278c-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8278c-121">JSON Representation</span></span>
<span data-ttu-id="8278c-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8278c-122">Here is a JSON representation of the resource.</span></span>
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



