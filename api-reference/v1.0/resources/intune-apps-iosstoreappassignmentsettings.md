---
title: iosStoreAppAssignmentSettings-Ressourcentyp
description: Enthält Eigenschaften zum Zuweisen einer mobilen iOS-Store-App zu einer Gruppe.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4d58490e97aec48f664ab6882198e4c1da3511e8
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250313"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="9e928-103">iosStoreAppAssignmentSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9e928-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="9e928-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9e928-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e928-105">Enthält Eigenschaften zum Zuweisen einer mobilen iOS-Store-App zu einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="9e928-105">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="9e928-106">Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="9e928-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9e928-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9e928-107">Properties</span></span>
|<span data-ttu-id="9e928-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9e928-108">Property</span></span>|<span data-ttu-id="9e928-109">Typ</span><span class="sxs-lookup"><span data-stu-id="9e928-109">Type</span></span>|<span data-ttu-id="9e928-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9e928-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e928-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="9e928-111">vpnConfigurationId</span></span>|<span data-ttu-id="9e928-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9e928-112">String</span></span>|<span data-ttu-id="9e928-113">Die VPN-Konfigurations-ID, die für diese App verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="9e928-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e928-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9e928-114">Relationships</span></span>
<span data-ttu-id="9e928-115">Keine</span><span class="sxs-lookup"><span data-stu-id="9e928-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e928-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9e928-116">JSON Representation</span></span>
<span data-ttu-id="9e928-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9e928-117">Here is a JSON representation of the resource.</span></span>
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



