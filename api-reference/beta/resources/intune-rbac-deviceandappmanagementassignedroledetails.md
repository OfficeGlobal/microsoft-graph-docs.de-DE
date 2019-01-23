---
title: Ressourcentyp deviceAndAppManagementAssignedRoleDetails
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d6ace16ba496feb24948c3e40c32dd8fcb2fcf48
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29428884"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a><span data-ttu-id="0b9c3-103">Ressourcentyp deviceAndAppManagementAssignedRoleDetails</span><span class="sxs-lookup"><span data-stu-id="0b9c3-103">deviceAndAppManagementAssignedRoleDetails resource type</span></span>

> <span data-ttu-id="0b9c3-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="0b9c3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0b9c3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0b9c3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0b9c3-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0b9c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b9c3-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="0b9c3-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="0b9c3-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0b9c3-108">Properties</span></span>
|<span data-ttu-id="0b9c3-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0b9c3-109">Property</span></span>|<span data-ttu-id="0b9c3-110">Typ</span><span class="sxs-lookup"><span data-stu-id="0b9c3-110">Type</span></span>|<span data-ttu-id="0b9c3-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0b9c3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b9c3-112">roleDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="0b9c3-112">roleDefinitionIds</span></span>|<span data-ttu-id="0b9c3-113">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="0b9c3-113">String collection</span></span>|<span data-ttu-id="0b9c3-114">Role-Definition-IDs für die spezifische Rollendefinitionen, die einem Benutzer zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="0b9c3-114">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="0b9c3-115">roleAssignmentIds</span><span class="sxs-lookup"><span data-stu-id="0b9c3-115">roleAssignmentIds</span></span>|<span data-ttu-id="0b9c3-116">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="0b9c3-116">String collection</span></span>|<span data-ttu-id="0b9c3-117">Role Assignment-IDs für die spezifische Rollenzuweisungen, die einem Benutzer zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="0b9c3-117">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b9c3-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0b9c3-118">Relationships</span></span>
<span data-ttu-id="0b9c3-119">Keine</span><span class="sxs-lookup"><span data-stu-id="0b9c3-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b9c3-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0b9c3-120">JSON Representation</span></span>
<span data-ttu-id="0b9c3-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0b9c3-121">Here is a JSON representation of the resource.</span></span>
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




