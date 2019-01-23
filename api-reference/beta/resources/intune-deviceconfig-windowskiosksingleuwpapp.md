---
title: Ressourcentyp windowsKioskSingleUWPApp
description: Die Klasse verwendet, um die UWP app-Informationen für die Konfiguration Kiosk identifizieren
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e62dc6393cc2dc6a9133732a42527abdfadbd91e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409377"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a><span data-ttu-id="23699-103">Ressourcentyp windowsKioskSingleUWPApp</span><span class="sxs-lookup"><span data-stu-id="23699-103">windowsKioskSingleUWPApp resource type</span></span>

> <span data-ttu-id="23699-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="23699-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="23699-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="23699-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23699-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="23699-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23699-107">Die Klasse verwendet, um die UWP app-Informationen für die Konfiguration Kiosk identifizieren</span><span class="sxs-lookup"><span data-stu-id="23699-107">The class used to identify the UWP app info for the kiosk configuration</span></span>


<span data-ttu-id="23699-108">Erbt vom [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23699-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="23699-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="23699-109">Properties</span></span>
|<span data-ttu-id="23699-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="23699-110">Property</span></span>|<span data-ttu-id="23699-111">Typ</span><span class="sxs-lookup"><span data-stu-id="23699-111">Type</span></span>|<span data-ttu-id="23699-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="23699-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23699-113">uwpApp</span><span class="sxs-lookup"><span data-stu-id="23699-113">uwpApp</span></span>|[<span data-ttu-id="23699-114">windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="23699-114">windowsKioskUWPApp</span></span>](../resources/intune-deviceconfig-windowskioskuwpapp.md)|<span data-ttu-id="23699-115">Dies ist die einzige Anwendung Benutzer Modell ID (AUMID), die Verwendung im Kioskmodus gestartet werden</span><span class="sxs-lookup"><span data-stu-id="23699-115">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="23699-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="23699-116">Relationships</span></span>
<span data-ttu-id="23699-117">Keine</span><span class="sxs-lookup"><span data-stu-id="23699-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23699-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="23699-118">JSON Representation</span></span>
<span data-ttu-id="23699-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="23699-119">Here is a JSON representation of the resource.</span></span>
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




