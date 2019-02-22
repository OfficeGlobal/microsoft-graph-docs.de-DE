---
title: iosLobAppAssignmentSettings-Ressourcentyp
description: Enthält Eigenschaften zum Zuweisen einer mobilen iOS-Branchen-App zu einer Gruppe.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c8f1dadc7a302c3b4b78f0fc9e278e9285ecbcc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172310"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="69121-103">iosLobAppAssignmentSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="69121-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="69121-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="69121-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69121-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="69121-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69121-106">Enthält Eigenschaften zum Zuweisen einer mobilen iOS-Branchen-App zu einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="69121-106">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="69121-107">Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="69121-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="69121-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="69121-108">Properties</span></span>
|<span data-ttu-id="69121-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="69121-109">Property</span></span>|<span data-ttu-id="69121-110">Typ</span><span class="sxs-lookup"><span data-stu-id="69121-110">Type</span></span>|<span data-ttu-id="69121-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="69121-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69121-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="69121-112">vpnConfigurationId</span></span>|<span data-ttu-id="69121-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="69121-113">String</span></span>|<span data-ttu-id="69121-114">Die VPN-Konfigurations-ID, die für diese App verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="69121-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69121-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="69121-115">Relationships</span></span>
<span data-ttu-id="69121-116">Keine</span><span class="sxs-lookup"><span data-stu-id="69121-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="69121-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="69121-117">JSON Representation</span></span>
<span data-ttu-id="69121-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="69121-118">Here is a JSON representation of the resource.</span></span>
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




