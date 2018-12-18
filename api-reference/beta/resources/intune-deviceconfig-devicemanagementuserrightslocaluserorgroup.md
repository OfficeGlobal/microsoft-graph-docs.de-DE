---
title: Ressourcentyp deviceManagementUserRightsLocalUserOrGroup
description: Stellt Informationen für einen lokalen Benutzer oder eine Gruppe, die zum Festlegen von Benutzerrechten an.
author: tfitzmac
ms.openlocfilehash: baabd2f3bb9e3bce44d172cd83f61f57c5c2c98d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303731"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="40e8f-103">Ressourcentyp deviceManagementUserRightsLocalUserOrGroup</span><span class="sxs-lookup"><span data-stu-id="40e8f-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="40e8f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="40e8f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40e8f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="40e8f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="40e8f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="40e8f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40e8f-107">Stellt Informationen für einen lokalen Benutzer oder eine Gruppe, die zum Festlegen von Benutzerrechten an.</span><span class="sxs-lookup"><span data-stu-id="40e8f-107">Represents information for a local user or group used for user rights setting.</span></span>
## <a name="properties"></a><span data-ttu-id="40e8f-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="40e8f-108">Properties</span></span>
|<span data-ttu-id="40e8f-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="40e8f-109">Property</span></span>|<span data-ttu-id="40e8f-110">Typ</span><span class="sxs-lookup"><span data-stu-id="40e8f-110">Type</span></span>|<span data-ttu-id="40e8f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="40e8f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40e8f-112">name</span><span class="sxs-lookup"><span data-stu-id="40e8f-112">name</span></span>|<span data-ttu-id="40e8f-113">String</span><span class="sxs-lookup"><span data-stu-id="40e8f-113">String</span></span>|<span data-ttu-id="40e8f-114">Der Name des lokalen Benutzers oder der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="40e8f-114">The name of this local user or group.</span></span>|
|<span data-ttu-id="40e8f-115">description</span><span class="sxs-lookup"><span data-stu-id="40e8f-115">description</span></span>|<span data-ttu-id="40e8f-116">String</span><span class="sxs-lookup"><span data-stu-id="40e8f-116">String</span></span>|<span data-ttu-id="40e8f-117">Der Admin-Beschreibung des lokalen Benutzers oder der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="40e8f-117">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="40e8f-118">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="40e8f-118">securityIdentifier</span></span>|<span data-ttu-id="40e8f-119">String</span><span class="sxs-lookup"><span data-stu-id="40e8f-119">String</span></span>|<span data-ttu-id="40e8f-120">Die Sicherheits-ID der lokalen Benutzer oder Gruppen (z. B. \* S-1-5-32-544).</span><span class="sxs-lookup"><span data-stu-id="40e8f-120">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="40e8f-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="40e8f-121">Relationships</span></span>
<span data-ttu-id="40e8f-122">Keine</span><span class="sxs-lookup"><span data-stu-id="40e8f-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="40e8f-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="40e8f-123">JSON Representation</span></span>
<span data-ttu-id="40e8f-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="40e8f-124">Here is a JSON representation of the resource.</span></span>
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





