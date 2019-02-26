---
title: windowsKioskLocalUser-Ressourcentyp
description: Die Klasse, die zum Identifizieren eines lokalen Kontos für die Kiosk Konfiguration verwendet wird.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 94b2397a8bb1a3825af97c5d22f273f622500359
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173199"
---
# <a name="windowskiosklocaluser-resource-type"></a><span data-ttu-id="1ed57-103">windowsKioskLocalUser-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1ed57-103">windowsKioskLocalUser resource type</span></span>

> <span data-ttu-id="1ed57-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1ed57-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ed57-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1ed57-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ed57-106">Die Klasse, die zum Identifizieren eines lokalen Kontos für die Kiosk Konfiguration verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="1ed57-106">The class used to identify a local account for the kiosk configuration</span></span>


<span data-ttu-id="1ed57-107">Erbt von [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="1ed57-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1ed57-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1ed57-108">Properties</span></span>
|<span data-ttu-id="1ed57-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1ed57-109">Property</span></span>|<span data-ttu-id="1ed57-110">Typ</span><span class="sxs-lookup"><span data-stu-id="1ed57-110">Type</span></span>|<span data-ttu-id="1ed57-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1ed57-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ed57-112">userName</span><span class="sxs-lookup"><span data-stu-id="1ed57-112">userName</span></span>|<span data-ttu-id="1ed57-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1ed57-113">String</span></span>|<span data-ttu-id="1ed57-114">Der lokale Benutzer, der für diese Kiosk Konfiguration gesperrt wird</span><span class="sxs-lookup"><span data-stu-id="1ed57-114">The local user that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ed57-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1ed57-115">Relationships</span></span>
<span data-ttu-id="1ed57-116">Keine</span><span class="sxs-lookup"><span data-stu-id="1ed57-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ed57-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1ed57-117">JSON Representation</span></span>
<span data-ttu-id="1ed57-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1ed57-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskLocalUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskLocalUser",
  "userName": "String"
}
```




