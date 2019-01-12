---
title: iosVppAppAssignmentSettings-Ressourcentyp
description: Enthält Eigenschaften zum Zuweisen einer mobilen iOS-VPP-App zu einer Gruppe.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e221ceb67789f9d96195a31bd7eba8f37a9df6bc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917643"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="0d7b8-103">iosVppAppAssignmentSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0d7b8-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="0d7b8-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0d7b8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0d7b8-105">Enthält Eigenschaften zum Zuweisen einer mobilen iOS-VPP-App zu einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="0d7b8-105">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>

<span data-ttu-id="0d7b8-106">Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="0d7b8-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0d7b8-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0d7b8-107">Properties</span></span>
|<span data-ttu-id="0d7b8-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0d7b8-108">Property</span></span>|<span data-ttu-id="0d7b8-109">Typ</span><span class="sxs-lookup"><span data-stu-id="0d7b8-109">Type</span></span>|<span data-ttu-id="0d7b8-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0d7b8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d7b8-111">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="0d7b8-111">useDeviceLicensing</span></span>|<span data-ttu-id="0d7b8-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0d7b8-112">Boolean</span></span>|<span data-ttu-id="0d7b8-113">Gibt an, ob die Gerätelizenzierung verwendet werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="0d7b8-113">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="0d7b8-114">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="0d7b8-114">vpnConfigurationId</span></span>|<span data-ttu-id="0d7b8-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d7b8-115">String</span></span>|<span data-ttu-id="0d7b8-116">Die VPN-Konfigurations-ID, die für diese App verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="0d7b8-116">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d7b8-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0d7b8-117">Relationships</span></span>
<span data-ttu-id="0d7b8-118">Keine</span><span class="sxs-lookup"><span data-stu-id="0d7b8-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0d7b8-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0d7b8-119">JSON Representation</span></span>
<span data-ttu-id="0d7b8-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0d7b8-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignmentSettings",
  "useDeviceLicensing": true,
  "vpnConfigurationId": "String"
}
```



