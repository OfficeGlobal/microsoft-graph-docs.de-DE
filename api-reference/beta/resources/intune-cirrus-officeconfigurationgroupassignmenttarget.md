---
title: Ressourcentyp officeConfigurationGroupAssignmentTarget
description: Office-Client-Konfiguration AAD Zuordnung Ziel gruppieren
ms.openlocfilehash: 263e48bfc5800231a9f36159e802f65294e6ac02
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063992"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="c9b4d-103">Ressourcentyp officeConfigurationGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c9b4d-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="c9b4d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c9b4d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9b4d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c9b4d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c9b4d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c9b4d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9b4d-107">Office-Client-Konfiguration AAD Zuordnung Ziel gruppieren</span><span class="sxs-lookup"><span data-stu-id="c9b4d-107">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="c9b4d-108">Erbt vom [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="c9b4d-108">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c9b4d-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c9b4d-109">Properties</span></span>
|<span data-ttu-id="c9b4d-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c9b4d-110">Property</span></span>|<span data-ttu-id="c9b4d-111">Typ</span><span class="sxs-lookup"><span data-stu-id="c9b4d-111">Type</span></span>|<span data-ttu-id="c9b4d-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c9b4d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9b4d-113">groupId</span><span class="sxs-lookup"><span data-stu-id="c9b4d-113">groupId</span></span>|<span data-ttu-id="c9b4d-114">String</span><span class="sxs-lookup"><span data-stu-id="c9b4d-114">String</span></span>|<span data-ttu-id="c9b4d-115">Die Id der Gruppe AAD sind wir Gerätekonfiguration zu adressieren.</span><span class="sxs-lookup"><span data-stu-id="c9b4d-115">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9b4d-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c9b4d-116">Relationships</span></span>
<span data-ttu-id="c9b4d-117">Keine</span><span class="sxs-lookup"><span data-stu-id="c9b4d-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c9b4d-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c9b4d-118">JSON Representation</span></span>
<span data-ttu-id="c9b4d-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c9b4d-119">Here is a JSON representation of the resource.</span></span>
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



