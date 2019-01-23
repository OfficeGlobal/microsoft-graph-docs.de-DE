---
title: Ressourcentyp macOSFirewallApplication
description: Stellt eine app in der Liste der Mac OS-Firewall-Anwendung
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fe3bbd83c3101420ec011fda85304fabce06daf0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404211"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="9eebf-103">Ressourcentyp macOSFirewallApplication</span><span class="sxs-lookup"><span data-stu-id="9eebf-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="9eebf-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="9eebf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9eebf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9eebf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9eebf-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9eebf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9eebf-107">Stellt eine app in der Liste der Mac OS-Firewall-Anwendung</span><span class="sxs-lookup"><span data-stu-id="9eebf-107">Represents an app in the list of macOS firewall applications</span></span>

## <a name="properties"></a><span data-ttu-id="9eebf-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9eebf-108">Properties</span></span>
|<span data-ttu-id="9eebf-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9eebf-109">Property</span></span>|<span data-ttu-id="9eebf-110">Typ</span><span class="sxs-lookup"><span data-stu-id="9eebf-110">Type</span></span>|<span data-ttu-id="9eebf-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9eebf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9eebf-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="9eebf-112">bundleId</span></span>|<span data-ttu-id="9eebf-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9eebf-113">String</span></span>|<span data-ttu-id="9eebf-114">Bundlekennung der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="9eebf-114">BundleId of the application.</span></span>|
|<span data-ttu-id="9eebf-115">allowsIncomingConnections</span><span class="sxs-lookup"><span data-stu-id="9eebf-115">allowsIncomingConnections</span></span>|<span data-ttu-id="9eebf-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="9eebf-116">Boolean</span></span>|<span data-ttu-id="9eebf-117">Unabhängig davon, ob eingehende Verbindungen zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="9eebf-117">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9eebf-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9eebf-118">Relationships</span></span>
<span data-ttu-id="9eebf-119">Keine</span><span class="sxs-lookup"><span data-stu-id="9eebf-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9eebf-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9eebf-120">JSON Representation</span></span>
<span data-ttu-id="9eebf-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9eebf-121">Here is a JSON representation of the resource.</span></span>
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




