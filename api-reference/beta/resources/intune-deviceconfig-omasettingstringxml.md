---
title: omaSettingStringXml-Ressourcentyp
description: Zeichenfolgen-XML-Definition der OMA-Einstellungen
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 846ed1c9bb17065b82f2663e7f4276b34442f9bd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164533"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="892b0-103">omaSettingStringXml-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="892b0-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="892b0-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="892b0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="892b0-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="892b0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="892b0-106">Zeichenfolgen-XML-Definition der OMA-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="892b0-106">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="892b0-107">Erbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="892b0-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="892b0-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="892b0-108">Properties</span></span>
|<span data-ttu-id="892b0-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="892b0-109">Property</span></span>|<span data-ttu-id="892b0-110">Typ</span><span class="sxs-lookup"><span data-stu-id="892b0-110">Type</span></span>|<span data-ttu-id="892b0-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="892b0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="892b0-112">displayName</span><span class="sxs-lookup"><span data-stu-id="892b0-112">displayName</span></span>|<span data-ttu-id="892b0-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="892b0-113">String</span></span>|<span data-ttu-id="892b0-114">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="892b0-114">Display Name.</span></span> <span data-ttu-id="892b0-115">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="892b0-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="892b0-116">description</span><span class="sxs-lookup"><span data-stu-id="892b0-116">description</span></span>|<span data-ttu-id="892b0-117">String</span><span class="sxs-lookup"><span data-stu-id="892b0-117">String</span></span>|<span data-ttu-id="892b0-118">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="892b0-118">Description.</span></span> <span data-ttu-id="892b0-119">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md).</span><span class="sxs-lookup"><span data-stu-id="892b0-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="892b0-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="892b0-120">omaUri</span></span>|<span data-ttu-id="892b0-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="892b0-121">String</span></span>|<span data-ttu-id="892b0-122">OMA</span><span class="sxs-lookup"><span data-stu-id="892b0-122">OMA.</span></span> <span data-ttu-id="892b0-123">Vererbt von [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="892b0-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="892b0-124">fileName</span><span class="sxs-lookup"><span data-stu-id="892b0-124">fileName</span></span>|<span data-ttu-id="892b0-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="892b0-125">String</span></span>|<span data-ttu-id="892b0-126">Die dem Dateinamen zugeordnete Werteigenschaft (\*.xml).</span><span class="sxs-lookup"><span data-stu-id="892b0-126">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="892b0-127">value</span><span class="sxs-lookup"><span data-stu-id="892b0-127">value</span></span>|<span data-ttu-id="892b0-128">Binär</span><span class="sxs-lookup"><span data-stu-id="892b0-128">Binary</span></span>|<span data-ttu-id="892b0-129">Wert</span><span class="sxs-lookup"><span data-stu-id="892b0-129">Value.</span></span> <span data-ttu-id="892b0-130">(UTF8-codiertes Bytearray)</span><span class="sxs-lookup"><span data-stu-id="892b0-130">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="892b0-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="892b0-131">Relationships</span></span>
<span data-ttu-id="892b0-132">Keine</span><span class="sxs-lookup"><span data-stu-id="892b0-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="892b0-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="892b0-133">JSON Representation</span></span>
<span data-ttu-id="892b0-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="892b0-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingStringXml"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingStringXml",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "binary"
}
```




