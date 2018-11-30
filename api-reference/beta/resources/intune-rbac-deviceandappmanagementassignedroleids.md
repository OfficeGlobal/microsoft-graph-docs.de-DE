---
title: Ressourcentyp deviceAndAppManagementAssignedRoleIds
description: Noch nicht dokumentiert
ms.openlocfilehash: 9d9fbf9bc6dcfa422316a236dfd890369d069c2f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062474"
---
# <a name="deviceandappmanagementassignedroleids-resource-type"></a><span data-ttu-id="78c8b-103">Ressourcentyp deviceAndAppManagementAssignedRoleIds</span><span class="sxs-lookup"><span data-stu-id="78c8b-103">deviceAndAppManagementAssignedRoleIds resource type</span></span>

> <span data-ttu-id="78c8b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="78c8b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78c8b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="78c8b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="78c8b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="78c8b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="78c8b-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="78c8b-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="78c8b-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="78c8b-108">Properties</span></span>
|<span data-ttu-id="78c8b-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="78c8b-109">Property</span></span>|<span data-ttu-id="78c8b-110">Typ</span><span class="sxs-lookup"><span data-stu-id="78c8b-110">Type</span></span>|<span data-ttu-id="78c8b-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="78c8b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78c8b-112">roleDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="78c8b-112">roleDefinitionIds</span></span>|<span data-ttu-id="78c8b-113">GUID-Sammlung</span><span class="sxs-lookup"><span data-stu-id="78c8b-113">Guid collection</span></span>|<span data-ttu-id="78c8b-114">Role-Definition-IDs für die spezifische Rollendefinitionen, die einem Benutzer zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="78c8b-114">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="78c8b-115">roleAssignmentIds</span><span class="sxs-lookup"><span data-stu-id="78c8b-115">roleAssignmentIds</span></span>|<span data-ttu-id="78c8b-116">GUID-Sammlung</span><span class="sxs-lookup"><span data-stu-id="78c8b-116">Guid collection</span></span>|<span data-ttu-id="78c8b-117">Role Assignment-IDs für die spezifische Rollenzuweisungen, die einem Benutzer zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="78c8b-117">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78c8b-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="78c8b-118">Relationships</span></span>
<span data-ttu-id="78c8b-119">Keine</span><span class="sxs-lookup"><span data-stu-id="78c8b-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="78c8b-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="78c8b-120">JSON Representation</span></span>
<span data-ttu-id="78c8b-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="78c8b-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceAndAppManagementAssignedRoleIds"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignedRoleIds",
  "roleDefinitionIds": [
    "Guid"
  ],
  "roleAssignmentIds": [
    "Guid"
  ]
}
```





