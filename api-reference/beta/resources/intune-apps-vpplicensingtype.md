---
title: vppLicensingType-Ressourcentyp
description: Enthält Eigenschaften für den iOS-Volume-Purchased Programm (Vpp)-Lizenzierungstyp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 47ee634c8fa488bb27c6c0a4beb7728fc7e427cb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948681"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="20db3-103">vppLicensingType-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="20db3-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="20db3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="20db3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="20db3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="20db3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="20db3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="20db3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20db3-107">Enthält Eigenschaften für den iOS-Volume-Purchased Programm (Vpp)-Lizenzierungstyp.</span><span class="sxs-lookup"><span data-stu-id="20db3-107">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>
## <a name="properties"></a><span data-ttu-id="20db3-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="20db3-108">Properties</span></span>
|<span data-ttu-id="20db3-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="20db3-109">Property</span></span>|<span data-ttu-id="20db3-110">Typ</span><span class="sxs-lookup"><span data-stu-id="20db3-110">Type</span></span>|<span data-ttu-id="20db3-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="20db3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20db3-112">supportUserLicensing</span><span class="sxs-lookup"><span data-stu-id="20db3-112">supportUserLicensing</span></span>|<span data-ttu-id="20db3-113">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="20db3-113">Boolean</span></span>|<span data-ttu-id="20db3-114">Gibt an, ob das Programm den Benutzerlizenzierungstyp unterstützt.</span><span class="sxs-lookup"><span data-stu-id="20db3-114">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="20db3-115">supportDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="20db3-115">supportDeviceLicensing</span></span>|<span data-ttu-id="20db3-116">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="20db3-116">Boolean</span></span>|<span data-ttu-id="20db3-117">Gibt an, ob das Programm den Gerätelizenzierungstyp unterstützt.</span><span class="sxs-lookup"><span data-stu-id="20db3-117">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="20db3-118">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="20db3-118">supportsUserLicensing</span></span>|<span data-ttu-id="20db3-119">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="20db3-119">Boolean</span></span>|<span data-ttu-id="20db3-120">Gibt an, ob das Programm den Benutzerlizenzierungstyp unterstützt.</span><span class="sxs-lookup"><span data-stu-id="20db3-120">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="20db3-121">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="20db3-121">supportsDeviceLicensing</span></span>|<span data-ttu-id="20db3-122">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="20db3-122">Boolean</span></span>|<span data-ttu-id="20db3-123">Gibt an, ob das Programm den Gerätelizenzierungstyp unterstützt.</span><span class="sxs-lookup"><span data-stu-id="20db3-123">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="20db3-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="20db3-124">Relationships</span></span>
<span data-ttu-id="20db3-125">Keine</span><span class="sxs-lookup"><span data-stu-id="20db3-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="20db3-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="20db3-126">JSON Representation</span></span>
<span data-ttu-id="20db3-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="20db3-127">Here is a JSON representation of the resource.</span></span>
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





