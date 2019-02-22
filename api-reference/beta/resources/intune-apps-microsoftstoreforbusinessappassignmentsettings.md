---
title: microsoftStoreForBusinessAppAssignmentSettings-Ressourcentyp
description: Enthält die Eigenschaften, die verwendet werden, um eine mobile Microsoft Store für Unternehmen-App einer Gruppe zuzuweisen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6fdcf4633433f471383e4c5b1c670eb5f5a8cb37
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164925"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="02cd2-103">microsoftStoreForBusinessAppAssignmentSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="02cd2-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="02cd2-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02cd2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02cd2-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="02cd2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02cd2-106">Enthält die Eigenschaften, die verwendet werden, um eine mobile Microsoft Store für Unternehmen-App einer Gruppe zuzuweisen.</span><span class="sxs-lookup"><span data-stu-id="02cd2-106">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="02cd2-107">Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="02cd2-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="02cd2-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="02cd2-108">Properties</span></span>
|<span data-ttu-id="02cd2-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="02cd2-109">Property</span></span>|<span data-ttu-id="02cd2-110">Typ</span><span class="sxs-lookup"><span data-stu-id="02cd2-110">Type</span></span>|<span data-ttu-id="02cd2-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="02cd2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02cd2-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="02cd2-112">useDeviceContext</span></span>|<span data-ttu-id="02cd2-113">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="02cd2-113">Boolean</span></span>|<span data-ttu-id="02cd2-114">Gibt an, ob der Geräte-Ausführungskontext für mobile Microsoft Store für Unternehmen-Apps verwendet werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="02cd2-114">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="02cd2-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="02cd2-115">Relationships</span></span>
<span data-ttu-id="02cd2-116">Keine</span><span class="sxs-lookup"><span data-stu-id="02cd2-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="02cd2-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="02cd2-117">JSON Representation</span></span>
<span data-ttu-id="02cd2-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="02cd2-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings",
  "useDeviceContext": true
}
```




