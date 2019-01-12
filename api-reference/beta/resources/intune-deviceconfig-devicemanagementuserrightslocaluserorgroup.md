---
title: Ressourcentyp deviceManagementUserRightsLocalUserOrGroup
description: Stellt Informationen für einen lokalen Benutzer oder eine Gruppe, die zum Festlegen von Benutzerrechten an.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 63e2dc3d16d17b76c4437e76eae642976711071c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972894"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="e1434-103">Ressourcentyp deviceManagementUserRightsLocalUserOrGroup</span><span class="sxs-lookup"><span data-stu-id="e1434-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="e1434-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e1434-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1434-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e1434-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e1434-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e1434-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1434-107">Stellt Informationen für einen lokalen Benutzer oder eine Gruppe, die zum Festlegen von Benutzerrechten an.</span><span class="sxs-lookup"><span data-stu-id="e1434-107">Represents information for a local user or group used for user rights setting.</span></span>
## <a name="properties"></a><span data-ttu-id="e1434-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e1434-108">Properties</span></span>
|<span data-ttu-id="e1434-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e1434-109">Property</span></span>|<span data-ttu-id="e1434-110">Typ</span><span class="sxs-lookup"><span data-stu-id="e1434-110">Type</span></span>|<span data-ttu-id="e1434-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e1434-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1434-112">name</span><span class="sxs-lookup"><span data-stu-id="e1434-112">name</span></span>|<span data-ttu-id="e1434-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e1434-113">String</span></span>|<span data-ttu-id="e1434-114">Der Name des lokalen Benutzers oder der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="e1434-114">The name of this local user or group.</span></span>|
|<span data-ttu-id="e1434-115">description</span><span class="sxs-lookup"><span data-stu-id="e1434-115">description</span></span>|<span data-ttu-id="e1434-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e1434-116">String</span></span>|<span data-ttu-id="e1434-117">Der Admin-Beschreibung des lokalen Benutzers oder der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="e1434-117">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="e1434-118">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="e1434-118">securityIdentifier</span></span>|<span data-ttu-id="e1434-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e1434-119">String</span></span>|<span data-ttu-id="e1434-120">Die Sicherheits-ID der lokalen Benutzer oder Gruppen (z. B. \* S-1-5-32-544).</span><span class="sxs-lookup"><span data-stu-id="e1434-120">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1434-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e1434-121">Relationships</span></span>
<span data-ttu-id="e1434-122">Keine</span><span class="sxs-lookup"><span data-stu-id="e1434-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e1434-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e1434-123">JSON Representation</span></span>
<span data-ttu-id="e1434-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e1434-124">Here is a JSON representation of the resource.</span></span>
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





