---
title: iosLobAppAssignmentSettings-Ressourcentyp
description: Enthält Eigenschaften zum Zuweisen einer mobilen iOS-Branchen-App zu einer Gruppe.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5beacfd60eb2237ed85a95bca21c27a38f956d16
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255206"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="f2ff3-103">iosLobAppAssignmentSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f2ff3-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="f2ff3-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f2ff3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2ff3-105">Enthält Eigenschaften zum Zuweisen einer mobilen iOS-Branchen-App zu einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="f2ff3-105">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="f2ff3-106">Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="f2ff3-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f2ff3-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f2ff3-107">Properties</span></span>
|<span data-ttu-id="f2ff3-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f2ff3-108">Property</span></span>|<span data-ttu-id="f2ff3-109">Typ</span><span class="sxs-lookup"><span data-stu-id="f2ff3-109">Type</span></span>|<span data-ttu-id="f2ff3-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f2ff3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2ff3-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="f2ff3-111">vpnConfigurationId</span></span>|<span data-ttu-id="f2ff3-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f2ff3-112">String</span></span>|<span data-ttu-id="f2ff3-113">Die VPN-Konfigurations-ID, die für diese App verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="f2ff3-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2ff3-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f2ff3-114">Relationships</span></span>
<span data-ttu-id="f2ff3-115">Keine</span><span class="sxs-lookup"><span data-stu-id="f2ff3-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2ff3-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f2ff3-116">JSON Representation</span></span>
<span data-ttu-id="f2ff3-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f2ff3-117">Here is a JSON representation of the resource.</span></span>
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



