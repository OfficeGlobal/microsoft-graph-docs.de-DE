---
title: windowsKioskSingleUWPApp-Ressourcentyp
description: Die Klasse, die zum Identifizieren der UWP-app-Informationen für die Kiosk Konfiguration verwendet wird.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d0a3b56c7bc9856b98708b63c247479e6ccf9c9b
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571158"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a><span data-ttu-id="cfc46-103">windowsKioskSingleUWPApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="cfc46-103">windowsKioskSingleUWPApp resource type</span></span>

> <span data-ttu-id="cfc46-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cfc46-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cfc46-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="cfc46-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfc46-106">Die Klasse, die zum Identifizieren der UWP-app-Informationen für die Kiosk Konfiguration verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="cfc46-106">The class used to identify the UWP app info for the kiosk configuration</span></span>


<span data-ttu-id="cfc46-107">Erbt von [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cfc46-107">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cfc46-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cfc46-108">Properties</span></span>
|<span data-ttu-id="cfc46-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cfc46-109">Property</span></span>|<span data-ttu-id="cfc46-110">Typ</span><span class="sxs-lookup"><span data-stu-id="cfc46-110">Type</span></span>|<span data-ttu-id="cfc46-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cfc46-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfc46-112">uwpApp</span><span class="sxs-lookup"><span data-stu-id="cfc46-112">uwpApp</span></span>|[<span data-ttu-id="cfc46-113">windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="cfc46-113">windowsKioskUWPApp</span></span>](../resources/intune-deviceconfig-windowskioskuwpapp.md)|<span data-ttu-id="cfc46-114">Dies ist die einzige Anwendungsbenutzer Modell-ID (AUMID), die im Kiosk-Modus verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="cfc46-114">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="cfc46-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="cfc46-115">Relationships</span></span>
<span data-ttu-id="cfc46-116">Keine</span><span class="sxs-lookup"><span data-stu-id="cfc46-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cfc46-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cfc46-117">JSON Representation</span></span>
<span data-ttu-id="cfc46-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cfc46-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskSingleUWPApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskSingleUWPApp",
  "uwpApp": {
    "@odata.type": "microsoft.graph.windowsKioskUWPApp",
    "startLayoutTileSize": "String",
    "name": "String",
    "appType": "String",
    "autoLaunch": true,
    "appUserModelId": "String",
    "appId": "String",
    "containedAppId": "String"
  }
}
```




