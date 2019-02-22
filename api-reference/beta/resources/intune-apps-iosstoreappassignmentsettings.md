---
title: iosStoreAppAssignmentSettings-Ressourcentyp
description: Enthält Eigenschaften zum Zuweisen einer mobilen iOS-Store-App zu einer Gruppe.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4d700b6a736f7d4a33362a66aeb8b75e6df7c605
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153963"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="76bbe-103">iosStoreAppAssignmentSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="76bbe-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="76bbe-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="76bbe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76bbe-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="76bbe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76bbe-106">Enthält Eigenschaften zum Zuweisen einer mobilen iOS-Store-App zu einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="76bbe-106">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="76bbe-107">Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="76bbe-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="76bbe-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="76bbe-108">Properties</span></span>
|<span data-ttu-id="76bbe-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="76bbe-109">Property</span></span>|<span data-ttu-id="76bbe-110">Typ</span><span class="sxs-lookup"><span data-stu-id="76bbe-110">Type</span></span>|<span data-ttu-id="76bbe-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="76bbe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76bbe-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="76bbe-112">vpnConfigurationId</span></span>|<span data-ttu-id="76bbe-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="76bbe-113">String</span></span>|<span data-ttu-id="76bbe-114">Die VPN-Konfigurations-ID, die für diese App verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="76bbe-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="76bbe-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="76bbe-115">Relationships</span></span>
<span data-ttu-id="76bbe-116">Keine</span><span class="sxs-lookup"><span data-stu-id="76bbe-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="76bbe-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="76bbe-117">JSON Representation</span></span>
<span data-ttu-id="76bbe-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="76bbe-118">Here is a JSON representation of the resource.</span></span>
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




