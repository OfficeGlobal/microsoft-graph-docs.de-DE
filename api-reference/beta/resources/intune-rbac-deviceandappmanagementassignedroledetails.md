---
title: deviceAndAppManagementAssignedRoleDetails-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eafacd349b5d315cb7a1149d7bcc7070700b7130
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160074"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a><span data-ttu-id="1128b-103">deviceAndAppManagementAssignedRoleDetails-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1128b-103">deviceAndAppManagementAssignedRoleDetails resource type</span></span>

> <span data-ttu-id="1128b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1128b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1128b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1128b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1128b-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="1128b-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="1128b-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1128b-107">Properties</span></span>
|<span data-ttu-id="1128b-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1128b-108">Property</span></span>|<span data-ttu-id="1128b-109">Typ</span><span class="sxs-lookup"><span data-stu-id="1128b-109">Type</span></span>|<span data-ttu-id="1128b-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1128b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1128b-111">roleDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="1128b-111">roleDefinitionIds</span></span>|<span data-ttu-id="1128b-112">String collection</span><span class="sxs-lookup"><span data-stu-id="1128b-112">String collection</span></span>|<span data-ttu-id="1128b-113">Rollen Definitions-IDs für die spezifische-Rollendefinitionen, die einem Benutzer zugewiesen sind.</span><span class="sxs-lookup"><span data-stu-id="1128b-113">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="1128b-114">roleAssignmentIds</span><span class="sxs-lookup"><span data-stu-id="1128b-114">roleAssignmentIds</span></span>|<span data-ttu-id="1128b-115">String collection</span><span class="sxs-lookup"><span data-stu-id="1128b-115">String collection</span></span>|<span data-ttu-id="1128b-116">Rollen Zuweisungs-IDs für die spezifische-Rollenzuweisungen, die einem Benutzer zugewiesen sind.</span><span class="sxs-lookup"><span data-stu-id="1128b-116">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1128b-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1128b-117">Relationships</span></span>
<span data-ttu-id="1128b-118">Keine</span><span class="sxs-lookup"><span data-stu-id="1128b-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1128b-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1128b-119">JSON Representation</span></span>
<span data-ttu-id="1128b-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1128b-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceAndAppManagementAssignedRoleDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignedRoleDetails",
  "roleDefinitionIds": [
    "String"
  ],
  "roleAssignmentIds": [
    "String"
  ]
}
```




