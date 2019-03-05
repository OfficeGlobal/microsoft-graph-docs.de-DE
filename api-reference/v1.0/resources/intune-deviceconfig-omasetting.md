---
title: omaSetting-Ressourcentyp
description: Definition der OMA-Einstellungen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6d0a69c10f1f0075caee48276bdbc37f6d616f22
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253379"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="5b550-103">omaSetting-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5b550-103">omaSetting resource type</span></span>

> <span data-ttu-id="5b550-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5b550-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b550-105">Definition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="5b550-105">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="5b550-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5b550-106">Properties</span></span>
|<span data-ttu-id="5b550-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5b550-107">Property</span></span>|<span data-ttu-id="5b550-108">Typ</span><span class="sxs-lookup"><span data-stu-id="5b550-108">Type</span></span>|<span data-ttu-id="5b550-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5b550-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b550-110">displayName</span><span class="sxs-lookup"><span data-stu-id="5b550-110">displayName</span></span>|<span data-ttu-id="5b550-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5b550-111">String</span></span>|<span data-ttu-id="5b550-112">Anzeigename.</span><span class="sxs-lookup"><span data-stu-id="5b550-112">Display Name.</span></span>|
|<span data-ttu-id="5b550-113">description</span><span class="sxs-lookup"><span data-stu-id="5b550-113">description</span></span>|<span data-ttu-id="5b550-114">String</span><span class="sxs-lookup"><span data-stu-id="5b550-114">String</span></span>|<span data-ttu-id="5b550-115">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="5b550-115">Description.</span></span>|
|<span data-ttu-id="5b550-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="5b550-116">omaUri</span></span>|<span data-ttu-id="5b550-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5b550-117">String</span></span>|<span data-ttu-id="5b550-118">OMA.</span><span class="sxs-lookup"><span data-stu-id="5b550-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b550-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5b550-119">Relationships</span></span>
<span data-ttu-id="5b550-120">Keine</span><span class="sxs-lookup"><span data-stu-id="5b550-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b550-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5b550-121">JSON Representation</span></span>
<span data-ttu-id="5b550-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5b550-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```



