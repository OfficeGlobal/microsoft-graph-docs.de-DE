---
title: iosLobAppAssignmentSettings-Ressourcentyp
description: Enthält Eigenschaften zum Zuweisen einer mobilen iOS-Branchen-App zu einer Gruppe.
ms.openlocfilehash: 5c4380103c7d06032d3605d944fe8d420258d070
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059183"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="81a7f-103">iosLobAppAssignmentSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="81a7f-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="81a7f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="81a7f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81a7f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="81a7f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="81a7f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="81a7f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81a7f-107">Enthält Eigenschaften zum Zuweisen einer mobilen iOS-Branchen-App zu einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="81a7f-107">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>

<span data-ttu-id="81a7f-108">Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="81a7f-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="81a7f-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="81a7f-109">Properties</span></span>
|<span data-ttu-id="81a7f-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="81a7f-110">Property</span></span>|<span data-ttu-id="81a7f-111">Typ</span><span class="sxs-lookup"><span data-stu-id="81a7f-111">Type</span></span>|<span data-ttu-id="81a7f-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="81a7f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81a7f-113">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="81a7f-113">vpnConfigurationId</span></span>|<span data-ttu-id="81a7f-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="81a7f-114">String</span></span>|<span data-ttu-id="81a7f-115">Die VPN-Konfigurations-ID, die für diese App verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="81a7f-115">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81a7f-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="81a7f-116">Relationships</span></span>
<span data-ttu-id="81a7f-117">Keine</span><span class="sxs-lookup"><span data-stu-id="81a7f-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="81a7f-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="81a7f-118">JSON Representation</span></span>
<span data-ttu-id="81a7f-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="81a7f-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppAssignmentSettings",
  "vpnConfigurationId": "String"
}
```





