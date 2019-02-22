---
title: deviceManagementUserRightsSetting-Ressourcentyp
description: Stellt eine Einstellung für Benutzerrechte dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f8fd9d2217fd39c4d2dc8e9db28cb5b5dcd0a1e6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172184"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a><span data-ttu-id="be347-103">deviceManagementUserRightsSetting-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="be347-103">deviceManagementUserRightsSetting resource type</span></span>

> <span data-ttu-id="be347-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="be347-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be347-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="be347-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be347-106">Stellt eine Einstellung für Benutzerrechte dar.</span><span class="sxs-lookup"><span data-stu-id="be347-106">Represents a user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="be347-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="be347-107">Properties</span></span>
|<span data-ttu-id="be347-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="be347-108">Property</span></span>|<span data-ttu-id="be347-109">Typ</span><span class="sxs-lookup"><span data-stu-id="be347-109">Type</span></span>|<span data-ttu-id="be347-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="be347-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be347-111">state</span><span class="sxs-lookup"><span data-stu-id="be347-111">state</span></span>|[<span data-ttu-id="be347-112">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="be347-112">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="be347-113">Darstellen des aktuellen Status dieser Benutzerrechte Einstellung.</span><span class="sxs-lookup"><span data-stu-id="be347-113">Representing the current state of this user rights setting.</span></span> <span data-ttu-id="be347-114">Mögliche Werte sind: `notConfigured`, `blocked` und `allowed`.</span><span class="sxs-lookup"><span data-stu-id="be347-114">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="be347-115">localUsersOrGroups</span><span class="sxs-lookup"><span data-stu-id="be347-115">localUsersOrGroups</span></span>|<span data-ttu-id="be347-116">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="be347-116">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) collection</span></span>|<span data-ttu-id="be347-117">Darstellen einer Auflistung von lokalen Benutzern oder Gruppen, die auf dem Gerät festgelegt werden, wenn der Status dieser Einstellung zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="be347-117">Representing a collection of local users or groups which will be set on device if the state of this setting is Allowed.</span></span> <span data-ttu-id="be347-118">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="be347-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be347-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="be347-119">Relationships</span></span>
<span data-ttu-id="be347-120">Keine</span><span class="sxs-lookup"><span data-stu-id="be347-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="be347-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="be347-121">JSON Representation</span></span>
<span data-ttu-id="be347-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="be347-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsSetting",
  "state": "String",
  "localUsersOrGroups": [
    {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
      "name": "String",
      "description": "String",
      "securityIdentifier": "String"
    }
  ]
}
```




