---
title: resourceAction-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d229a6d4d8b514cbf092efb224ff09dfb0c78ad4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157624"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="a3e04-103">resourceAction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a3e04-103">resourceAction resource type</span></span>

> <span data-ttu-id="a3e04-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a3e04-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3e04-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a3e04-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3e04-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="a3e04-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="a3e04-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a3e04-107">Properties</span></span>
|<span data-ttu-id="a3e04-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a3e04-108">Property</span></span>|<span data-ttu-id="a3e04-109">Typ</span><span class="sxs-lookup"><span data-stu-id="a3e04-109">Type</span></span>|<span data-ttu-id="a3e04-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a3e04-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3e04-111">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="a3e04-111">allowedResourceActions</span></span>|<span data-ttu-id="a3e04-112">String collection</span><span class="sxs-lookup"><span data-stu-id="a3e04-112">String collection</span></span>|<span data-ttu-id="a3e04-113">Zulässige Aktionen</span><span class="sxs-lookup"><span data-stu-id="a3e04-113">Allowed Actions</span></span>|
|<span data-ttu-id="a3e04-114">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="a3e04-114">notAllowedResourceActions</span></span>|<span data-ttu-id="a3e04-115">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="a3e04-115">String collection</span></span>|<span data-ttu-id="a3e04-116">Nicht zulässige Aktionen</span><span class="sxs-lookup"><span data-stu-id="a3e04-116">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3e04-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a3e04-117">Relationships</span></span>
<span data-ttu-id="a3e04-118">Keine</span><span class="sxs-lookup"><span data-stu-id="a3e04-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3e04-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a3e04-119">JSON Representation</span></span>
<span data-ttu-id="a3e04-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a3e04-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```




