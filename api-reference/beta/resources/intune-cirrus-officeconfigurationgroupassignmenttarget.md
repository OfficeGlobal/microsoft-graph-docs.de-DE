---
title: Ressourcentyp officeConfigurationGroupAssignmentTarget
description: Office-Client-Konfiguration AAD Zuordnung Ziel gruppieren
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b2fe6a668c1f490c167fe61496af14cf2654cebb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814770"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="492af-103">Ressourcentyp officeConfigurationGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="492af-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="492af-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="492af-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="492af-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="492af-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="492af-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="492af-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="492af-107">Office-Client-Konfiguration AAD Zuordnung Ziel gruppieren</span><span class="sxs-lookup"><span data-stu-id="492af-107">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="492af-108">Erbt vom [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="492af-108">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="492af-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="492af-109">Properties</span></span>
|<span data-ttu-id="492af-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="492af-110">Property</span></span>|<span data-ttu-id="492af-111">Typ</span><span class="sxs-lookup"><span data-stu-id="492af-111">Type</span></span>|<span data-ttu-id="492af-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="492af-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="492af-113">groupId</span><span class="sxs-lookup"><span data-stu-id="492af-113">groupId</span></span>|<span data-ttu-id="492af-114">String</span><span class="sxs-lookup"><span data-stu-id="492af-114">String</span></span>|<span data-ttu-id="492af-115">Die Id der Gruppe AAD sind wir Gerätekonfiguration zu adressieren.</span><span class="sxs-lookup"><span data-stu-id="492af-115">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="492af-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="492af-116">Relationships</span></span>
<span data-ttu-id="492af-117">Keine</span><span class="sxs-lookup"><span data-stu-id="492af-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="492af-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="492af-118">JSON Representation</span></span>
<span data-ttu-id="492af-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="492af-119">Here is a JSON representation of the resource.</span></span>
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



