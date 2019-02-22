---
title: omaSetting-Ressourcentyp
description: Definition der OMA-Einstellungen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fab80ad06fb5654578f29b92e3b0f3aa9c09abdb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143848"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="60bd5-103">omaSetting-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="60bd5-103">omaSetting resource type</span></span>

> <span data-ttu-id="60bd5-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="60bd5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60bd5-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="60bd5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60bd5-106">Definition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="60bd5-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="60bd5-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="60bd5-107">Properties</span></span>
|<span data-ttu-id="60bd5-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="60bd5-108">Property</span></span>|<span data-ttu-id="60bd5-109">Typ</span><span class="sxs-lookup"><span data-stu-id="60bd5-109">Type</span></span>|<span data-ttu-id="60bd5-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="60bd5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60bd5-111">displayName</span><span class="sxs-lookup"><span data-stu-id="60bd5-111">displayName</span></span>|<span data-ttu-id="60bd5-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="60bd5-112">String</span></span>|<span data-ttu-id="60bd5-113">Anzeigename.</span><span class="sxs-lookup"><span data-stu-id="60bd5-113">Display Name.</span></span>|
|<span data-ttu-id="60bd5-114">description</span><span class="sxs-lookup"><span data-stu-id="60bd5-114">description</span></span>|<span data-ttu-id="60bd5-115">String</span><span class="sxs-lookup"><span data-stu-id="60bd5-115">String</span></span>|<span data-ttu-id="60bd5-116">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="60bd5-116">Description.</span></span>|
|<span data-ttu-id="60bd5-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="60bd5-117">omaUri</span></span>|<span data-ttu-id="60bd5-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="60bd5-118">String</span></span>|<span data-ttu-id="60bd5-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="60bd5-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60bd5-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="60bd5-120">Relationships</span></span>
<span data-ttu-id="60bd5-121">Keine</span><span class="sxs-lookup"><span data-stu-id="60bd5-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="60bd5-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="60bd5-122">JSON Representation</span></span>
<span data-ttu-id="60bd5-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="60bd5-123">Here is a JSON representation of the resource.</span></span>
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




