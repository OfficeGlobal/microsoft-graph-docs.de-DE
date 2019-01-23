---
title: Ressourcentyp deviceManagementUserRightsSetting
description: Stellt eine Benutzerrechte festlegen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 35e6ec1a5faa5556a0e113df145d718c488b1669
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415054"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a><span data-ttu-id="8f33f-103">Ressourcentyp deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8f33f-103">deviceManagementUserRightsSetting resource type</span></span>

> <span data-ttu-id="8f33f-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="8f33f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8f33f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8f33f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8f33f-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8f33f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f33f-107">Stellt eine Benutzerrechte festlegen.</span><span class="sxs-lookup"><span data-stu-id="8f33f-107">Represents a user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="8f33f-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8f33f-108">Properties</span></span>
|<span data-ttu-id="8f33f-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8f33f-109">Property</span></span>|<span data-ttu-id="8f33f-110">Typ</span><span class="sxs-lookup"><span data-stu-id="8f33f-110">Type</span></span>|<span data-ttu-id="8f33f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f33f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f33f-112">state</span><span class="sxs-lookup"><span data-stu-id="8f33f-112">state</span></span>|[<span data-ttu-id="8f33f-113">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="8f33f-113">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="8f33f-114">Einstellung für Benutzerrechterichtlinien, die den aktuellen Status dieses Benutzers darstellt.</span><span class="sxs-lookup"><span data-stu-id="8f33f-114">Representing the current state of this user rights setting.</span></span> <span data-ttu-id="8f33f-115">Mögliche Werte sind: `notConfigured`, `blocked` und `allowed`.</span><span class="sxs-lookup"><span data-stu-id="8f33f-115">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="8f33f-116">localUsersOrGroups</span><span class="sxs-lookup"><span data-stu-id="8f33f-116">localUsersOrGroups</span></span>|<span data-ttu-id="8f33f-117">[DeviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="8f33f-117">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) collection</span></span>|<span data-ttu-id="8f33f-118">Eine Auflistung von lokalen Benutzern oder Gruppen, die auf Gerät festgelegt werden, wenn der Status dieser Einstellung zulässig ist, der darstellt.</span><span class="sxs-lookup"><span data-stu-id="8f33f-118">Representing a collection of local users or groups which will be set on device if the state of this setting is Allowed.</span></span> <span data-ttu-id="8f33f-119">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="8f33f-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f33f-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8f33f-120">Relationships</span></span>
<span data-ttu-id="8f33f-121">Keine</span><span class="sxs-lookup"><span data-stu-id="8f33f-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f33f-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8f33f-122">JSON Representation</span></span>
<span data-ttu-id="8f33f-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8f33f-123">Here is a JSON representation of the resource.</span></span>
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




