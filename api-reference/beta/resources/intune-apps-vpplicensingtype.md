---
title: vppLicensingType-Ressourcentyp
description: Enthält Eigenschaften für den iOS-Volume-Purchased Programm (Vpp)-Lizenzierungstyp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f09ca9a8f891b90563ebad2cff74775f4c6fb7c2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168397"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="c89bb-103">vppLicensingType-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c89bb-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="c89bb-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c89bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c89bb-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c89bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c89bb-106">Enthält Eigenschaften für den iOS-Volume-Purchased Programm (Vpp)-Lizenzierungstyp.</span><span class="sxs-lookup"><span data-stu-id="c89bb-106">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="c89bb-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c89bb-107">Properties</span></span>
|<span data-ttu-id="c89bb-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c89bb-108">Property</span></span>|<span data-ttu-id="c89bb-109">Typ</span><span class="sxs-lookup"><span data-stu-id="c89bb-109">Type</span></span>|<span data-ttu-id="c89bb-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c89bb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c89bb-111">supportUserLicensing</span><span class="sxs-lookup"><span data-stu-id="c89bb-111">supportUserLicensing</span></span>|<span data-ttu-id="c89bb-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c89bb-112">Boolean</span></span>|<span data-ttu-id="c89bb-113">Gibt an, ob das Programm den Benutzerlizenzierungstyp unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c89bb-113">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="c89bb-114">supportDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="c89bb-114">supportDeviceLicensing</span></span>|<span data-ttu-id="c89bb-115">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c89bb-115">Boolean</span></span>|<span data-ttu-id="c89bb-116">Gibt an, ob das Programm den Gerätelizenzierungstyp unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c89bb-116">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="c89bb-117">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="c89bb-117">supportsUserLicensing</span></span>|<span data-ttu-id="c89bb-118">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c89bb-118">Boolean</span></span>|<span data-ttu-id="c89bb-119">Gibt an, ob das Programm den Benutzerlizenzierungstyp unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c89bb-119">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="c89bb-120">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="c89bb-120">supportsDeviceLicensing</span></span>|<span data-ttu-id="c89bb-121">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c89bb-121">Boolean</span></span>|<span data-ttu-id="c89bb-122">Gibt an, ob das Programm den Gerätelizenzierungstyp unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c89bb-122">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c89bb-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c89bb-123">Relationships</span></span>
<span data-ttu-id="c89bb-124">Keine</span><span class="sxs-lookup"><span data-stu-id="c89bb-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c89bb-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c89bb-125">JSON Representation</span></span>
<span data-ttu-id="c89bb-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c89bb-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportUserLicensing": true,
  "supportDeviceLicensing": true,
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```




