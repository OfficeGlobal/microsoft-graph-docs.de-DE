---
title: Ressourcentyp officeConfigurationGroupAssignmentTarget
description: Office-Client-Konfiguration AAD Zuordnung Ziel gruppieren
author: tfitzmac
ms.openlocfilehash: 82008de6e5cb64885e9e2d5804a00956da2ff434
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335868"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="733ed-103">Ressourcentyp officeConfigurationGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="733ed-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="733ed-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="733ed-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="733ed-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="733ed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="733ed-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="733ed-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="733ed-107">Office-Client-Konfiguration AAD Zuordnung Ziel gruppieren</span><span class="sxs-lookup"><span data-stu-id="733ed-107">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="733ed-108">Erbt vom [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="733ed-108">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="733ed-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="733ed-109">Properties</span></span>
|<span data-ttu-id="733ed-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="733ed-110">Property</span></span>|<span data-ttu-id="733ed-111">Typ</span><span class="sxs-lookup"><span data-stu-id="733ed-111">Type</span></span>|<span data-ttu-id="733ed-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="733ed-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="733ed-113">groupId</span><span class="sxs-lookup"><span data-stu-id="733ed-113">groupId</span></span>|<span data-ttu-id="733ed-114">String</span><span class="sxs-lookup"><span data-stu-id="733ed-114">String</span></span>|<span data-ttu-id="733ed-115">Die Id der Gruppe AAD sind wir Gerätekonfiguration zu adressieren.</span><span class="sxs-lookup"><span data-stu-id="733ed-115">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="733ed-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="733ed-116">Relationships</span></span>
<span data-ttu-id="733ed-117">Keine</span><span class="sxs-lookup"><span data-stu-id="733ed-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="733ed-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="733ed-118">JSON Representation</span></span>
<span data-ttu-id="733ed-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="733ed-119">Here is a JSON representation of the resource.</span></span>
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



