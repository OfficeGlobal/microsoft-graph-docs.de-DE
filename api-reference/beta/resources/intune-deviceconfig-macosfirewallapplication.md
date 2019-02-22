---
title: macOSFirewallApplication-Ressourcentyp
description: Stellt eine app in der Liste der macOS-Firewall-Anwendungen dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 477911dba492bdda09eb815aba968bb7f63955bf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145402"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="3e2e6-103">macOSFirewallApplication-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3e2e6-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="3e2e6-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3e2e6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e2e6-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3e2e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e2e6-106">Stellt eine app in der Liste der macOS-Firewall-Anwendungen dar.</span><span class="sxs-lookup"><span data-stu-id="3e2e6-106">Represents an app in the list of macOS firewall applications</span></span>

## <a name="properties"></a><span data-ttu-id="3e2e6-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3e2e6-107">Properties</span></span>
|<span data-ttu-id="3e2e6-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3e2e6-108">Property</span></span>|<span data-ttu-id="3e2e6-109">Typ</span><span class="sxs-lookup"><span data-stu-id="3e2e6-109">Type</span></span>|<span data-ttu-id="3e2e6-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3e2e6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e2e6-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="3e2e6-111">bundleId</span></span>|<span data-ttu-id="3e2e6-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3e2e6-112">String</span></span>|<span data-ttu-id="3e2e6-113">Bündeln der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="3e2e6-113">BundleId of the application.</span></span>|
|<span data-ttu-id="3e2e6-114">allowsIncomingConnections</span><span class="sxs-lookup"><span data-stu-id="3e2e6-114">allowsIncomingConnections</span></span>|<span data-ttu-id="3e2e6-115">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3e2e6-115">Boolean</span></span>|<span data-ttu-id="3e2e6-116">Gibt an, ob eingehende Verbindungen zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="3e2e6-116">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e2e6-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3e2e6-117">Relationships</span></span>
<span data-ttu-id="3e2e6-118">Keine</span><span class="sxs-lookup"><span data-stu-id="3e2e6-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e2e6-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3e2e6-119">JSON Representation</span></span>
<span data-ttu-id="3e2e6-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3e2e6-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSFirewallApplication"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSFirewallApplication",
  "bundleId": "String",
  "allowsIncomingConnections": true
}
```




