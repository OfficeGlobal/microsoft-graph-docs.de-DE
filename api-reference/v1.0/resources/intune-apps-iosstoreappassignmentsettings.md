---
title: iosStoreAppAssignmentSettings-Ressourcentyp
description: Enthält Eigenschaften zum Zuweisen einer mobilen iOS-Store-App zu einer Gruppe.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 34776d6002926486baa05d0720ce1c7eeecee927
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822232"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="59383-103">iosStoreAppAssignmentSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="59383-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="59383-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="59383-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59383-105">Enthält Eigenschaften zum Zuweisen einer mobilen iOS-Store-App zu einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="59383-105">Contains properties used to assign an iOS Store mobile app to a group.</span></span>

<span data-ttu-id="59383-106">Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="59383-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="59383-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="59383-107">Properties</span></span>
|<span data-ttu-id="59383-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="59383-108">Property</span></span>|<span data-ttu-id="59383-109">Typ</span><span class="sxs-lookup"><span data-stu-id="59383-109">Type</span></span>|<span data-ttu-id="59383-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="59383-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59383-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="59383-111">vpnConfigurationId</span></span>|<span data-ttu-id="59383-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="59383-112">String</span></span>|<span data-ttu-id="59383-113">Die VPN-Konfigurations-ID, die für diese App verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="59383-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="59383-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="59383-114">Relationships</span></span>
<span data-ttu-id="59383-115">Keine</span><span class="sxs-lookup"><span data-stu-id="59383-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="59383-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="59383-116">JSON Representation</span></span>
<span data-ttu-id="59383-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="59383-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosStoreAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosStoreAppAssignmentSettings",
  "vpnConfigurationId": "String"
}
```



