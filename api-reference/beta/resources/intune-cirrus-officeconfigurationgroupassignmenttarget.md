---
title: officeConfigurationGroupAssignmentTarget-Ressourcentyp
description: Office-Client Konfigurations Ziel für AAD-Gruppenzuweisung.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7a3451d4bddec96c1e21cd605b05cb34d96372ff
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153550"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="684d0-103">officeConfigurationGroupAssignmentTarget-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="684d0-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="684d0-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="684d0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="684d0-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="684d0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="684d0-106">Office-Client Konfigurations Ziel für AAD-Gruppenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="684d0-106">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="684d0-107">Erbt von [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="684d0-107">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="684d0-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="684d0-108">Properties</span></span>
|<span data-ttu-id="684d0-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="684d0-109">Property</span></span>|<span data-ttu-id="684d0-110">Typ</span><span class="sxs-lookup"><span data-stu-id="684d0-110">Type</span></span>|<span data-ttu-id="684d0-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="684d0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="684d0-112">groupId</span><span class="sxs-lookup"><span data-stu-id="684d0-112">groupId</span></span>|<span data-ttu-id="684d0-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="684d0-113">String</span></span>|<span data-ttu-id="684d0-114">Die ID der AAD-Gruppe, auf die die Gerätekonfiguration zielt.</span><span class="sxs-lookup"><span data-stu-id="684d0-114">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="684d0-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="684d0-115">Relationships</span></span>
<span data-ttu-id="684d0-116">Keine</span><span class="sxs-lookup"><span data-stu-id="684d0-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="684d0-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="684d0-117">JSON Representation</span></span>
<span data-ttu-id="684d0-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="684d0-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfigurationGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfigurationGroupAssignmentTarget",
  "groupId": "String"
}
```



