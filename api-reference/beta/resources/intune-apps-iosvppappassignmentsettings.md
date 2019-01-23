---
title: iosVppAppAssignmentSettings-Ressourcentyp
description: Enthält Eigenschaften zum Zuweisen einer mobilen iOS-VPP-App zu einer Gruppe.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1148336c5fa868cea90f223e66bf3868775647c6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423678"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="2e719-103">iosVppAppAssignmentSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2e719-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="2e719-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="2e719-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2e719-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2e719-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2e719-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2e719-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e719-107">Enthält Eigenschaften zum Zuweisen einer mobilen iOS-VPP-App zu einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="2e719-107">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="2e719-108">Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="2e719-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2e719-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2e719-109">Properties</span></span>
|<span data-ttu-id="2e719-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2e719-110">Property</span></span>|<span data-ttu-id="2e719-111">Typ</span><span class="sxs-lookup"><span data-stu-id="2e719-111">Type</span></span>|<span data-ttu-id="2e719-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2e719-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e719-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="2e719-113">useDeviceLicensing</span></span>|<span data-ttu-id="2e719-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2e719-114">Boolean</span></span>|<span data-ttu-id="2e719-115">Gibt an, ob die Gerätelizenzierung verwendet werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="2e719-115">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="2e719-116">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="2e719-116">vpnConfigurationId</span></span>|<span data-ttu-id="2e719-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2e719-117">String</span></span>|<span data-ttu-id="2e719-118">Die VPN-Konfigurations-ID, die für diese App verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="2e719-118">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e719-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2e719-119">Relationships</span></span>
<span data-ttu-id="2e719-120">Keine</span><span class="sxs-lookup"><span data-stu-id="2e719-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e719-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2e719-121">JSON Representation</span></span>
<span data-ttu-id="2e719-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2e719-122">Here is a JSON representation of the resource.</span></span>
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




