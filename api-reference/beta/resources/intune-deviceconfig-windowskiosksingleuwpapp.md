---
title: Ressourcentyp windowsKioskSingleUWPApp
description: Die Klasse verwendet, um die UWP app-Informationen für die Konfiguration Kiosk identifizieren
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c11469784e2c450b151c9a81a07f6c1568cf3a3a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818144"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a><span data-ttu-id="7664b-103">Ressourcentyp windowsKioskSingleUWPApp</span><span class="sxs-lookup"><span data-stu-id="7664b-103">windowsKioskSingleUWPApp resource type</span></span>

> <span data-ttu-id="7664b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7664b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7664b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7664b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7664b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7664b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7664b-107">Die Klasse verwendet, um die UWP app-Informationen für die Konfiguration Kiosk identifizieren</span><span class="sxs-lookup"><span data-stu-id="7664b-107">The class used to identify the UWP app info for the kiosk configuration</span></span>

<span data-ttu-id="7664b-108">Erbt vom [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7664b-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7664b-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7664b-109">Properties</span></span>
|<span data-ttu-id="7664b-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7664b-110">Property</span></span>|<span data-ttu-id="7664b-111">Typ</span><span class="sxs-lookup"><span data-stu-id="7664b-111">Type</span></span>|<span data-ttu-id="7664b-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7664b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7664b-113">uwpApp</span><span class="sxs-lookup"><span data-stu-id="7664b-113">uwpApp</span></span>|[<span data-ttu-id="7664b-114">windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="7664b-114">windowsKioskUWPApp</span></span>](../resources/intune-deviceconfig-windowskioskuwpapp.md)|<span data-ttu-id="7664b-115">Dies ist die einzige Anwendung Benutzer Modell ID (AUMID), die Verwendung im Kioskmodus gestartet werden</span><span class="sxs-lookup"><span data-stu-id="7664b-115">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="7664b-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7664b-116">Relationships</span></span>
<span data-ttu-id="7664b-117">Keine</span><span class="sxs-lookup"><span data-stu-id="7664b-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7664b-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7664b-118">JSON Representation</span></span>
<span data-ttu-id="7664b-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7664b-119">Here is a JSON representation of the resource.</span></span>
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
    "appUserModelId": "String",
    "appId": "String",
    "containedAppId": "String"
  }
}
```





