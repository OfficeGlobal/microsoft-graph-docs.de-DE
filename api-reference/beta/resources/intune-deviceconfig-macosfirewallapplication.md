---
title: Ressourcentyp macOSFirewallApplication
description: Stellt eine app in der Liste der Mac OS-Firewall-Anwendung
ms.openlocfilehash: 6e016f2191fd9b366bbdf5dbaef5562284a6b5ae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059826"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="3c0bb-103">Ressourcentyp macOSFirewallApplication</span><span class="sxs-lookup"><span data-stu-id="3c0bb-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="3c0bb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3c0bb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c0bb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c0bb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3c0bb-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3c0bb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c0bb-107">Stellt eine app in der Liste der Mac OS-Firewall-Anwendung</span><span class="sxs-lookup"><span data-stu-id="3c0bb-107">Represents an app in the list of macOS firewall applications</span></span>
## <a name="properties"></a><span data-ttu-id="3c0bb-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3c0bb-108">Properties</span></span>
|<span data-ttu-id="3c0bb-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3c0bb-109">Property</span></span>|<span data-ttu-id="3c0bb-110">Typ</span><span class="sxs-lookup"><span data-stu-id="3c0bb-110">Type</span></span>|<span data-ttu-id="3c0bb-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3c0bb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c0bb-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="3c0bb-112">bundleId</span></span>|<span data-ttu-id="3c0bb-113">String</span><span class="sxs-lookup"><span data-stu-id="3c0bb-113">String</span></span>|<span data-ttu-id="3c0bb-114">Bundlekennung der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="3c0bb-114">BundleId of the application.</span></span>|
|<span data-ttu-id="3c0bb-115">allowsIncomingConnections</span><span class="sxs-lookup"><span data-stu-id="3c0bb-115">allowsIncomingConnections</span></span>|<span data-ttu-id="3c0bb-116">Boolesch</span><span class="sxs-lookup"><span data-stu-id="3c0bb-116">Boolean</span></span>|<span data-ttu-id="3c0bb-117">Unabhängig davon, ob eingehende Verbindungen zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="3c0bb-117">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c0bb-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3c0bb-118">Relationships</span></span>
<span data-ttu-id="3c0bb-119">Keine</span><span class="sxs-lookup"><span data-stu-id="3c0bb-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3c0bb-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3c0bb-120">JSON Representation</span></span>
<span data-ttu-id="3c0bb-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3c0bb-121">Here is a JSON representation of the resource.</span></span>
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





