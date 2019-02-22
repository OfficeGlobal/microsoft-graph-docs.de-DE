---
title: windowsKioskSingleUWPApp-Ressourcentyp
description: Die Klasse, die zum Identifizieren der UWP-app-Informationen für die Kiosk Konfiguration verwendet wird.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 804dd2f34416eecb956b322a0f178daaf39b2418
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142042"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a><span data-ttu-id="98889-103">windowsKioskSingleUWPApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="98889-103">windowsKioskSingleUWPApp resource type</span></span>

> <span data-ttu-id="98889-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="98889-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98889-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="98889-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98889-106">Die Klasse, die zum Identifizieren der UWP-app-Informationen für die Kiosk Konfiguration verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="98889-106">The class used to identify the UWP app info for the kiosk configuration</span></span>


<span data-ttu-id="98889-107">Erbt von [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98889-107">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="98889-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="98889-108">Properties</span></span>
|<span data-ttu-id="98889-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="98889-109">Property</span></span>|<span data-ttu-id="98889-110">Typ</span><span class="sxs-lookup"><span data-stu-id="98889-110">Type</span></span>|<span data-ttu-id="98889-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="98889-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98889-112">uwpApp</span><span class="sxs-lookup"><span data-stu-id="98889-112">uwpApp</span></span>|[<span data-ttu-id="98889-113">windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="98889-113">windowsKioskUWPApp</span></span>](../resources/intune-deviceconfig-windowskioskuwpapp.md)|<span data-ttu-id="98889-114">Dies ist die einzige Anwendungsbenutzer Modell-ID (AUMID), die im Kiosk-Modus verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="98889-114">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="98889-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="98889-115">Relationships</span></span>
<span data-ttu-id="98889-116">Keine</span><span class="sxs-lookup"><span data-stu-id="98889-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="98889-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="98889-117">JSON Representation</span></span>
<span data-ttu-id="98889-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="98889-118">Here is a JSON representation of the resource.</span></span>
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
    "appUserModelId": "String",
    "appId": "String",
    "containedAppId": "String"
  }
}
```




