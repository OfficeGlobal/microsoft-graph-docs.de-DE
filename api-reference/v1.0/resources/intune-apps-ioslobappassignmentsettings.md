---
title: iosLobAppAssignmentSettings-Ressourcentyp
description: Enthält Eigenschaften zum Zuweisen einer mobilen iOS-Branchen-App zu einer Gruppe.
author: tfitzmac
ms.openlocfilehash: 78de511bdbdf2e4a8b16d9ce32a790329d2eb3c9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306090"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="c7999-103">iosLobAppAssignmentSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c7999-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="c7999-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c7999-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7999-105">Enthält Eigenschaften zum Zuweisen einer mobilen iOS-Branchen-App zu einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="c7999-105">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>

<span data-ttu-id="c7999-106">Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="c7999-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c7999-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c7999-107">Properties</span></span>
|<span data-ttu-id="c7999-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c7999-108">Property</span></span>|<span data-ttu-id="c7999-109">Typ</span><span class="sxs-lookup"><span data-stu-id="c7999-109">Type</span></span>|<span data-ttu-id="c7999-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c7999-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7999-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="c7999-111">vpnConfigurationId</span></span>|<span data-ttu-id="c7999-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c7999-112">String</span></span>|<span data-ttu-id="c7999-113">Die VPN-Konfigurations-ID, die für diese App verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="c7999-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7999-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c7999-114">Relationships</span></span>
<span data-ttu-id="c7999-115">Keine</span><span class="sxs-lookup"><span data-stu-id="c7999-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c7999-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c7999-116">JSON Representation</span></span>
<span data-ttu-id="c7999-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c7999-117">Here is a JSON representation of the resource.</span></span>
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



