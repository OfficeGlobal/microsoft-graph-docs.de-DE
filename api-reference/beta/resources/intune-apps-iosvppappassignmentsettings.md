---
title: iosVppAppAssignmentSettings-Ressourcentyp
description: Enthält Eigenschaften zum Zuweisen einer mobilen iOS-VPP-App zu einer Gruppe.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4d8269de61d91e5c855cd7b5741bb768e8063321
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154033"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="fa0c6-103">iosVppAppAssignmentSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fa0c6-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="fa0c6-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fa0c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa0c6-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="fa0c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa0c6-106">Enthält Eigenschaften zum Zuweisen einer mobilen iOS-VPP-App zu einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="fa0c6-106">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="fa0c6-107">Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="fa0c6-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fa0c6-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fa0c6-108">Properties</span></span>
|<span data-ttu-id="fa0c6-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fa0c6-109">Property</span></span>|<span data-ttu-id="fa0c6-110">Typ</span><span class="sxs-lookup"><span data-stu-id="fa0c6-110">Type</span></span>|<span data-ttu-id="fa0c6-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa0c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa0c6-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="fa0c6-112">useDeviceLicensing</span></span>|<span data-ttu-id="fa0c6-113">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="fa0c6-113">Boolean</span></span>|<span data-ttu-id="fa0c6-114">Gibt an, ob die Gerätelizenzierung verwendet werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="fa0c6-114">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="fa0c6-115">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="fa0c6-115">vpnConfigurationId</span></span>|<span data-ttu-id="fa0c6-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa0c6-116">String</span></span>|<span data-ttu-id="fa0c6-117">Die VPN-Konfigurations-ID, die für diese App verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="fa0c6-117">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa0c6-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fa0c6-118">Relationships</span></span>
<span data-ttu-id="fa0c6-119">Keine</span><span class="sxs-lookup"><span data-stu-id="fa0c6-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa0c6-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fa0c6-120">JSON Representation</span></span>
<span data-ttu-id="fa0c6-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fa0c6-121">Here is a JSON representation of the resource.</span></span>
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




