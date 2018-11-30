---
title: iosVppAppAssignmentSettings-Ressourcentyp
description: Enthält Eigenschaften zum Zuweisen einer mobilen iOS-VPP-App zu einer Gruppe.
ms.openlocfilehash: 6fc529fe1aeea6bdbef46ad0cd97fb5830250b4c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019071"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="0f4ca-103">iosVppAppAssignmentSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0f4ca-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="0f4ca-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0f4ca-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f4ca-105">Enthält Eigenschaften zum Zuweisen einer mobilen iOS-VPP-App zu einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="0f4ca-105">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>

<span data-ttu-id="0f4ca-106">Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="0f4ca-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0f4ca-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0f4ca-107">Properties</span></span>
|<span data-ttu-id="0f4ca-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0f4ca-108">Property</span></span>|<span data-ttu-id="0f4ca-109">Typ</span><span class="sxs-lookup"><span data-stu-id="0f4ca-109">Type</span></span>|<span data-ttu-id="0f4ca-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f4ca-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f4ca-111">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="0f4ca-111">useDeviceLicensing</span></span>|<span data-ttu-id="0f4ca-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0f4ca-112">Boolean</span></span>|<span data-ttu-id="0f4ca-113">Gibt an, ob die Gerätelizenzierung verwendet werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="0f4ca-113">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="0f4ca-114">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="0f4ca-114">vpnConfigurationId</span></span>|<span data-ttu-id="0f4ca-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0f4ca-115">String</span></span>|<span data-ttu-id="0f4ca-116">Die VPN-Konfigurations-ID, die für diese App verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="0f4ca-116">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f4ca-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0f4ca-117">Relationships</span></span>
<span data-ttu-id="0f4ca-118">Keine</span><span class="sxs-lookup"><span data-stu-id="0f4ca-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0f4ca-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0f4ca-119">JSON Representation</span></span>
<span data-ttu-id="0f4ca-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0f4ca-120">Here is a JSON representation of the resource.</span></span>
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



