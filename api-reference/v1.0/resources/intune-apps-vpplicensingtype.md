---
title: vppLicensingType-Ressourcentyp
description: Enthält Eigenschaften für den iOS-Volume-Purchased Programm (Vpp)-Lizenzierungstyp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 73b46c9bcd8680ffbd78c1cfc85cc6dec85126e6
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256119"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="06de1-103">vppLicensingType-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="06de1-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="06de1-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="06de1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06de1-105">Enthält Eigenschaften für den iOS-Volume-Purchased Programm (Vpp)-Lizenzierungstyp.</span><span class="sxs-lookup"><span data-stu-id="06de1-105">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="06de1-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="06de1-106">Properties</span></span>
|<span data-ttu-id="06de1-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="06de1-107">Property</span></span>|<span data-ttu-id="06de1-108">Typ</span><span class="sxs-lookup"><span data-stu-id="06de1-108">Type</span></span>|<span data-ttu-id="06de1-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06de1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06de1-110">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="06de1-110">supportsUserLicensing</span></span>|<span data-ttu-id="06de1-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="06de1-111">Boolean</span></span>|<span data-ttu-id="06de1-112">Gibt an, ob das Programm den Benutzerlizenzierungstyp unterstützt.</span><span class="sxs-lookup"><span data-stu-id="06de1-112">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="06de1-113">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="06de1-113">supportsDeviceLicensing</span></span>|<span data-ttu-id="06de1-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="06de1-114">Boolean</span></span>|<span data-ttu-id="06de1-115">Gibt an, ob das Programm den Gerätelizenzierungstyp unterstützt.</span><span class="sxs-lookup"><span data-stu-id="06de1-115">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06de1-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="06de1-116">Relationships</span></span>
<span data-ttu-id="06de1-117">Keine</span><span class="sxs-lookup"><span data-stu-id="06de1-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="06de1-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="06de1-118">JSON Representation</span></span>
<span data-ttu-id="06de1-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="06de1-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```



