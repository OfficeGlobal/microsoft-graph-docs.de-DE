---
title: vppLicensingType-Ressourcentyp
description: Enthält Eigenschaften für den iOS-Volume-Purchased Programm (Vpp)-Lizenzierungstyp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5d4b7983d20f22be5f8cce24a5c362926d00de55
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851597"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="12f00-103">vppLicensingType-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="12f00-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="12f00-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="12f00-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12f00-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="12f00-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="12f00-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="12f00-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12f00-107">Enthält Eigenschaften für den iOS-Volume-Purchased Programm (Vpp)-Lizenzierungstyp.</span><span class="sxs-lookup"><span data-stu-id="12f00-107">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>
## <a name="properties"></a><span data-ttu-id="12f00-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="12f00-108">Properties</span></span>
|<span data-ttu-id="12f00-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="12f00-109">Property</span></span>|<span data-ttu-id="12f00-110">Typ</span><span class="sxs-lookup"><span data-stu-id="12f00-110">Type</span></span>|<span data-ttu-id="12f00-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="12f00-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12f00-112">supportUserLicensing</span><span class="sxs-lookup"><span data-stu-id="12f00-112">supportUserLicensing</span></span>|<span data-ttu-id="12f00-113">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="12f00-113">Boolean</span></span>|<span data-ttu-id="12f00-114">Gibt an, ob das Programm den Benutzerlizenzierungstyp unterstützt.</span><span class="sxs-lookup"><span data-stu-id="12f00-114">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="12f00-115">supportDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="12f00-115">supportDeviceLicensing</span></span>|<span data-ttu-id="12f00-116">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="12f00-116">Boolean</span></span>|<span data-ttu-id="12f00-117">Gibt an, ob das Programm den Gerätelizenzierungstyp unterstützt.</span><span class="sxs-lookup"><span data-stu-id="12f00-117">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="12f00-118">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="12f00-118">supportsUserLicensing</span></span>|<span data-ttu-id="12f00-119">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="12f00-119">Boolean</span></span>|<span data-ttu-id="12f00-120">Gibt an, ob das Programm den Benutzerlizenzierungstyp unterstützt.</span><span class="sxs-lookup"><span data-stu-id="12f00-120">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="12f00-121">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="12f00-121">supportsDeviceLicensing</span></span>|<span data-ttu-id="12f00-122">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="12f00-122">Boolean</span></span>|<span data-ttu-id="12f00-123">Gibt an, ob das Programm den Gerätelizenzierungstyp unterstützt.</span><span class="sxs-lookup"><span data-stu-id="12f00-123">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12f00-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="12f00-124">Relationships</span></span>
<span data-ttu-id="12f00-125">Keine</span><span class="sxs-lookup"><span data-stu-id="12f00-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="12f00-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="12f00-126">JSON Representation</span></span>
<span data-ttu-id="12f00-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="12f00-127">Here is a JSON representation of the resource.</span></span>
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





