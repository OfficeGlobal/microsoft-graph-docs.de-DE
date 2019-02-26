---
title: macOSLobChildApp-Ressourcentyp
description: Enthält Eigenschaften der MacOS-Branchen-app in einem Bundle-Paket
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f4bf8a8715bb681d1737a2fb1b39e5bac61fb9d7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146998"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="1a566-103">macOSLobChildApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1a566-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="1a566-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1a566-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a566-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1a566-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a566-106">Enthält Eigenschaften der MacOS-Branchen-app in einem Bundle-Paket</span><span class="sxs-lookup"><span data-stu-id="1a566-106">Contains properties the MacOS LOB App in a bundle package</span></span>

## <a name="properties"></a><span data-ttu-id="1a566-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1a566-107">Properties</span></span>
|<span data-ttu-id="1a566-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1a566-108">Property</span></span>|<span data-ttu-id="1a566-109">Typ</span><span class="sxs-lookup"><span data-stu-id="1a566-109">Type</span></span>|<span data-ttu-id="1a566-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1a566-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a566-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="1a566-111">bundleId</span></span>|<span data-ttu-id="1a566-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a566-112">String</span></span>|<span data-ttu-id="1a566-113">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="1a566-113">The Identity Name.</span></span>|
|<span data-ttu-id="1a566-114">buildNumber</span><span class="sxs-lookup"><span data-stu-id="1a566-114">buildNumber</span></span>|<span data-ttu-id="1a566-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a566-115">String</span></span>|<span data-ttu-id="1a566-116">Die Buildnummer der MacOS-app.</span><span class="sxs-lookup"><span data-stu-id="1a566-116">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="1a566-117">versionNumber</span><span class="sxs-lookup"><span data-stu-id="1a566-117">versionNumber</span></span>|<span data-ttu-id="1a566-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a566-118">String</span></span>|<span data-ttu-id="1a566-119">Die Versionsnummer der MacOS-app.</span><span class="sxs-lookup"><span data-stu-id="1a566-119">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a566-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1a566-120">Relationships</span></span>
<span data-ttu-id="1a566-121">Keine</span><span class="sxs-lookup"><span data-stu-id="1a566-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a566-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1a566-122">JSON Representation</span></span>
<span data-ttu-id="1a566-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1a566-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLobChildApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLobChildApp",
  "bundleId": "String",
  "buildNumber": "String",
  "versionNumber": "String"
}
```




