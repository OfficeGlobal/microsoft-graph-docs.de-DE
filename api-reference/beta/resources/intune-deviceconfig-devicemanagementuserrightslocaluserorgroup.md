---
title: deviceManagementUserRightsLocalUserOrGroup-Ressourcentyp
description: Stellt Informationen für einen lokalen Benutzer oder eine Gruppe dar, die für die Benutzerrechte Einstellung verwendet wird.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 68c514635540bcf12db27e8a9ca816573293d3ad
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174860"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="34b76-103">deviceManagementUserRightsLocalUserOrGroup-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="34b76-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="34b76-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34b76-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34b76-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="34b76-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34b76-106">Stellt Informationen für einen lokalen Benutzer oder eine Gruppe dar, die für die Benutzerrechte Einstellung verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="34b76-106">Represents information for a local user or group used for user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="34b76-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="34b76-107">Properties</span></span>
|<span data-ttu-id="34b76-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="34b76-108">Property</span></span>|<span data-ttu-id="34b76-109">Typ</span><span class="sxs-lookup"><span data-stu-id="34b76-109">Type</span></span>|<span data-ttu-id="34b76-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="34b76-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34b76-111">name</span><span class="sxs-lookup"><span data-stu-id="34b76-111">name</span></span>|<span data-ttu-id="34b76-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34b76-112">String</span></span>|<span data-ttu-id="34b76-113">Der Name dieses lokalen Benutzers oder dieser Gruppe.</span><span class="sxs-lookup"><span data-stu-id="34b76-113">The name of this local user or group.</span></span>|
|<span data-ttu-id="34b76-114">description</span><span class="sxs-lookup"><span data-stu-id="34b76-114">description</span></span>|<span data-ttu-id="34b76-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34b76-115">String</span></span>|<span data-ttu-id="34b76-116">Die Beschreibung des Administrators dieses lokalen Benutzers oder dieser Gruppe.</span><span class="sxs-lookup"><span data-stu-id="34b76-116">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="34b76-117">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="34b76-117">securityIdentifier</span></span>|<span data-ttu-id="34b76-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34b76-118">String</span></span>|<span data-ttu-id="34b76-119">Die Sicherheits-ID dieses lokalen Benutzers oder einer Gruppe (z. b. \* S-1-5-32-544).</span><span class="sxs-lookup"><span data-stu-id="34b76-119">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="34b76-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="34b76-120">Relationships</span></span>
<span data-ttu-id="34b76-121">Keine</span><span class="sxs-lookup"><span data-stu-id="34b76-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34b76-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="34b76-122">JSON Representation</span></span>
<span data-ttu-id="34b76-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="34b76-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
  "name": "String",
  "description": "String",
  "securityIdentifier": "String"
}
```




