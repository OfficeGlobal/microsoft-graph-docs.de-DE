---
title: Ressourcentyp deviceManagementUserRightsSetting
description: Stellt eine Benutzerrechte festlegen.
ms.openlocfilehash: e657c15a76700ef87283220254937ec685c57784
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063359"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a><span data-ttu-id="dbf19-103">Ressourcentyp deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="dbf19-103">deviceManagementUserRightsSetting resource type</span></span>

> <span data-ttu-id="dbf19-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dbf19-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dbf19-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dbf19-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dbf19-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="dbf19-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dbf19-107">Stellt eine Benutzerrechte festlegen.</span><span class="sxs-lookup"><span data-stu-id="dbf19-107">Represents a user rights setting.</span></span>
## <a name="properties"></a><span data-ttu-id="dbf19-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dbf19-108">Properties</span></span>
|<span data-ttu-id="dbf19-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dbf19-109">Property</span></span>|<span data-ttu-id="dbf19-110">Typ</span><span class="sxs-lookup"><span data-stu-id="dbf19-110">Type</span></span>|<span data-ttu-id="dbf19-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dbf19-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbf19-112">state</span><span class="sxs-lookup"><span data-stu-id="dbf19-112">state</span></span>|[<span data-ttu-id="dbf19-113">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="dbf19-113">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="dbf19-114">Einstellung für Benutzerrechterichtlinien, die den aktuellen Status dieses Benutzers darstellt.</span><span class="sxs-lookup"><span data-stu-id="dbf19-114">Representing the current state of this user rights setting.</span></span> <span data-ttu-id="dbf19-115">Mögliche Werte sind: `notConfigured`, `blocked` und `allowed`.</span><span class="sxs-lookup"><span data-stu-id="dbf19-115">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="dbf19-116">localUsersOrGroups</span><span class="sxs-lookup"><span data-stu-id="dbf19-116">localUsersOrGroups</span></span>|<span data-ttu-id="dbf19-117">[DeviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="dbf19-117">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) collection</span></span>|<span data-ttu-id="dbf19-118">Eine Auflistung von lokalen Benutzern oder Gruppen, die auf Gerät festgelegt werden, wenn der Status dieser Einstellung zulässig ist, der darstellt.</span><span class="sxs-lookup"><span data-stu-id="dbf19-118">Representing a collection of local users or groups which will be set on device if the state of this setting is Allowed.</span></span> <span data-ttu-id="dbf19-119">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="dbf19-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dbf19-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="dbf19-120">Relationships</span></span>
<span data-ttu-id="dbf19-121">Keine</span><span class="sxs-lookup"><span data-stu-id="dbf19-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dbf19-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dbf19-122">JSON Representation</span></span>
<span data-ttu-id="dbf19-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="dbf19-123">Here is a JSON representation of the resource.</span></span>
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





