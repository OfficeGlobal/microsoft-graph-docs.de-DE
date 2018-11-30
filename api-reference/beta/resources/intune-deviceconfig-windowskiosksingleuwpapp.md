---
title: Ressourcentyp windowsKioskSingleUWPApp
description: Die Klasse verwendet, um die UWP app-Informationen für die Konfiguration Kiosk identifizieren
ms.openlocfilehash: 009d53d1439894b59a89a1f269df34c4dbb09ce1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063109"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a><span data-ttu-id="455e6-103">Ressourcentyp windowsKioskSingleUWPApp</span><span class="sxs-lookup"><span data-stu-id="455e6-103">windowsKioskSingleUWPApp resource type</span></span>

> <span data-ttu-id="455e6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="455e6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="455e6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="455e6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="455e6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="455e6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="455e6-107">Die Klasse verwendet, um die UWP app-Informationen für die Konfiguration Kiosk identifizieren</span><span class="sxs-lookup"><span data-stu-id="455e6-107">The class used to identify the UWP app info for the kiosk configuration</span></span>

<span data-ttu-id="455e6-108">Erbt vom [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="455e6-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="455e6-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="455e6-109">Properties</span></span>
|<span data-ttu-id="455e6-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="455e6-110">Property</span></span>|<span data-ttu-id="455e6-111">Typ</span><span class="sxs-lookup"><span data-stu-id="455e6-111">Type</span></span>|<span data-ttu-id="455e6-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="455e6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="455e6-113">uwpApp</span><span class="sxs-lookup"><span data-stu-id="455e6-113">uwpApp</span></span>|[<span data-ttu-id="455e6-114">windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="455e6-114">windowsKioskUWPApp</span></span>](../resources/intune-deviceconfig-windowskioskuwpapp.md)|<span data-ttu-id="455e6-115">Dies ist die einzige Anwendung Benutzer Modell ID (AUMID), die Verwendung im Kioskmodus gestartet werden</span><span class="sxs-lookup"><span data-stu-id="455e6-115">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="455e6-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="455e6-116">Relationships</span></span>
<span data-ttu-id="455e6-117">Keine</span><span class="sxs-lookup"><span data-stu-id="455e6-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="455e6-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="455e6-118">JSON Representation</span></span>
<span data-ttu-id="455e6-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="455e6-119">Here is a JSON representation of the resource.</span></span>
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





