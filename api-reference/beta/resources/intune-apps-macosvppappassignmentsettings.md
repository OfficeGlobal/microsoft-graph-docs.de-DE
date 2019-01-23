---
title: Ressourcentyp macOsVppAppAssignmentSettings
description: Enthält Eigenschaften, die zum Zuweisen einer mobilen Mac VPP-app zu einer Gruppe.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0927277b11416da001ad826200bf4ec841341118
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431582"
---
# <a name="macosvppappassignmentsettings-resource-type"></a><span data-ttu-id="674f7-103">Ressourcentyp macOsVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="674f7-103">macOsVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="674f7-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="674f7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="674f7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="674f7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="674f7-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="674f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="674f7-107">Enthält Eigenschaften, die zum Zuweisen einer mobilen Mac VPP-app zu einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="674f7-107">Contains properties used to assign an Mac VPP mobile app to a group.</span></span>


<span data-ttu-id="674f7-108">Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="674f7-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="674f7-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="674f7-109">Properties</span></span>
|<span data-ttu-id="674f7-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="674f7-110">Property</span></span>|<span data-ttu-id="674f7-111">Typ</span><span class="sxs-lookup"><span data-stu-id="674f7-111">Type</span></span>|<span data-ttu-id="674f7-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="674f7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="674f7-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="674f7-113">useDeviceLicensing</span></span>|<span data-ttu-id="674f7-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="674f7-114">Boolean</span></span>|<span data-ttu-id="674f7-115">Gibt an, ob die Gerätelizenzierung verwendet werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="674f7-115">Whether or not to use device licensing.</span></span>|

## <a name="relationships"></a><span data-ttu-id="674f7-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="674f7-116">Relationships</span></span>
<span data-ttu-id="674f7-117">Keine</span><span class="sxs-lookup"><span data-stu-id="674f7-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="674f7-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="674f7-118">JSON Representation</span></span>
<span data-ttu-id="674f7-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="674f7-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOsVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignmentSettings",
  "useDeviceLicensing": true
}
```




