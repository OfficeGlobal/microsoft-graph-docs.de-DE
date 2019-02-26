---
title: iosHomeScreenApp-Ressourcentyp
description: Gibt das Symbol einer App auf der Startseite an.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: faaa2bfa7ac0d4a25eeb4452349250ceb3d80524
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163175"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="a60c5-103">iosHomeScreenApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a60c5-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="a60c5-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a60c5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a60c5-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a60c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a60c5-106">Gibt das Symbol einer App auf der Startseite an.</span><span class="sxs-lookup"><span data-stu-id="a60c5-106">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="a60c5-107">Erbt von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="a60c5-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a60c5-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a60c5-108">Properties</span></span>
|<span data-ttu-id="a60c5-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a60c5-109">Property</span></span>|<span data-ttu-id="a60c5-110">Typ</span><span class="sxs-lookup"><span data-stu-id="a60c5-110">Type</span></span>|<span data-ttu-id="a60c5-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a60c5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a60c5-112">displayName</span><span class="sxs-lookup"><span data-stu-id="a60c5-112">displayName</span></span>|<span data-ttu-id="a60c5-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a60c5-113">String</span></span>|<span data-ttu-id="a60c5-114">Name der von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) geerbten App</span><span class="sxs-lookup"><span data-stu-id="a60c5-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="a60c5-115">bundleID</span><span class="sxs-lookup"><span data-stu-id="a60c5-115">bundleID</span></span>|<span data-ttu-id="a60c5-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a60c5-116">String</span></span>|<span data-ttu-id="a60c5-117">Paket-ID der App</span><span class="sxs-lookup"><span data-stu-id="a60c5-117">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="a60c5-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a60c5-118">Relationships</span></span>
<span data-ttu-id="a60c5-119">Keine</span><span class="sxs-lookup"><span data-stu-id="a60c5-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a60c5-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a60c5-120">JSON Representation</span></span>
<span data-ttu-id="a60c5-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a60c5-121">Here is a JSON representation of the resource.</span></span>
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




