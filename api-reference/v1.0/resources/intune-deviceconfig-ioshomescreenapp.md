---
title: iosHomeScreenApp-Ressourcentyp
description: Gibt das Symbol einer App auf der Startseite an.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 67c11096414db0dccad2ccf56ec184a4e3f30397
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260935"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="dff88-103">iosHomeScreenApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="dff88-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="dff88-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="dff88-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dff88-105">Gibt das Symbol einer App auf der Startseite an.</span><span class="sxs-lookup"><span data-stu-id="dff88-105">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="dff88-106">Erbt von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="dff88-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dff88-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dff88-107">Properties</span></span>
|<span data-ttu-id="dff88-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dff88-108">Property</span></span>|<span data-ttu-id="dff88-109">Typ</span><span class="sxs-lookup"><span data-stu-id="dff88-109">Type</span></span>|<span data-ttu-id="dff88-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dff88-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dff88-111">displayName</span><span class="sxs-lookup"><span data-stu-id="dff88-111">displayName</span></span>|<span data-ttu-id="dff88-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dff88-112">String</span></span>|<span data-ttu-id="dff88-113">Name der von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) geerbten App</span><span class="sxs-lookup"><span data-stu-id="dff88-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="dff88-114">bundleID</span><span class="sxs-lookup"><span data-stu-id="dff88-114">bundleID</span></span>|<span data-ttu-id="dff88-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dff88-115">String</span></span>|<span data-ttu-id="dff88-116">Paket-ID der App</span><span class="sxs-lookup"><span data-stu-id="dff88-116">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="dff88-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="dff88-117">Relationships</span></span>
<span data-ttu-id="dff88-118">Keine</span><span class="sxs-lookup"><span data-stu-id="dff88-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dff88-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dff88-119">JSON Representation</span></span>
<span data-ttu-id="dff88-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="dff88-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String"
}
```



