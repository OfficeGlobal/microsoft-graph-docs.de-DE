---
title: vppLicensingType-Ressourcentyp
description: Enthält Eigenschaften für den iOS-Volume-Purchased Programm (Vpp)-Lizenzierungstyp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 42bb678077781309b9e06c339112537bc2e48bde
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399675"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="a1c4c-103">vppLicensingType-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a1c4c-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="a1c4c-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="a1c4c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a1c4c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a1c4c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a1c4c-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a1c4c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1c4c-107">Enthält Eigenschaften für den iOS-Volume-Purchased Programm (Vpp)-Lizenzierungstyp.</span><span class="sxs-lookup"><span data-stu-id="a1c4c-107">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="a1c4c-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a1c4c-108">Properties</span></span>
|<span data-ttu-id="a1c4c-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a1c4c-109">Property</span></span>|<span data-ttu-id="a1c4c-110">Typ</span><span class="sxs-lookup"><span data-stu-id="a1c4c-110">Type</span></span>|<span data-ttu-id="a1c4c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a1c4c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1c4c-112">supportUserLicensing</span><span class="sxs-lookup"><span data-stu-id="a1c4c-112">supportUserLicensing</span></span>|<span data-ttu-id="a1c4c-113">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a1c4c-113">Boolean</span></span>|<span data-ttu-id="a1c4c-114">Gibt an, ob das Programm den Benutzerlizenzierungstyp unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a1c4c-114">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="a1c4c-115">supportDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="a1c4c-115">supportDeviceLicensing</span></span>|<span data-ttu-id="a1c4c-116">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a1c4c-116">Boolean</span></span>|<span data-ttu-id="a1c4c-117">Gibt an, ob das Programm den Gerätelizenzierungstyp unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a1c4c-117">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="a1c4c-118">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="a1c4c-118">supportsUserLicensing</span></span>|<span data-ttu-id="a1c4c-119">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a1c4c-119">Boolean</span></span>|<span data-ttu-id="a1c4c-120">Gibt an, ob das Programm den Benutzerlizenzierungstyp unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a1c4c-120">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="a1c4c-121">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="a1c4c-121">supportsDeviceLicensing</span></span>|<span data-ttu-id="a1c4c-122">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a1c4c-122">Boolean</span></span>|<span data-ttu-id="a1c4c-123">Gibt an, ob das Programm den Gerätelizenzierungstyp unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a1c4c-123">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1c4c-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a1c4c-124">Relationships</span></span>
<span data-ttu-id="a1c4c-125">Keine</span><span class="sxs-lookup"><span data-stu-id="a1c4c-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a1c4c-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a1c4c-126">JSON Representation</span></span>
<span data-ttu-id="a1c4c-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a1c4c-127">Here is a JSON representation of the resource.</span></span>
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




