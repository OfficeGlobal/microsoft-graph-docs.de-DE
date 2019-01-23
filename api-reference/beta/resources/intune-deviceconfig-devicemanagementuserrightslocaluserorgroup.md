---
title: Ressourcentyp deviceManagementUserRightsLocalUserOrGroup
description: Stellt Informationen für einen lokalen Benutzer oder eine Gruppe, die zum Festlegen von Benutzerrechten an.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8a2cc0ff5b9e054398e7878b7d99619b59d109a4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422061"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="838d0-103">Ressourcentyp deviceManagementUserRightsLocalUserOrGroup</span><span class="sxs-lookup"><span data-stu-id="838d0-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="838d0-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="838d0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="838d0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="838d0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="838d0-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="838d0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="838d0-107">Stellt Informationen für einen lokalen Benutzer oder eine Gruppe, die zum Festlegen von Benutzerrechten an.</span><span class="sxs-lookup"><span data-stu-id="838d0-107">Represents information for a local user or group used for user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="838d0-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="838d0-108">Properties</span></span>
|<span data-ttu-id="838d0-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="838d0-109">Property</span></span>|<span data-ttu-id="838d0-110">Typ</span><span class="sxs-lookup"><span data-stu-id="838d0-110">Type</span></span>|<span data-ttu-id="838d0-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="838d0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="838d0-112">name</span><span class="sxs-lookup"><span data-stu-id="838d0-112">name</span></span>|<span data-ttu-id="838d0-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="838d0-113">String</span></span>|<span data-ttu-id="838d0-114">Der Name des lokalen Benutzers oder der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="838d0-114">The name of this local user or group.</span></span>|
|<span data-ttu-id="838d0-115">description</span><span class="sxs-lookup"><span data-stu-id="838d0-115">description</span></span>|<span data-ttu-id="838d0-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="838d0-116">String</span></span>|<span data-ttu-id="838d0-117">Der Admin-Beschreibung des lokalen Benutzers oder der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="838d0-117">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="838d0-118">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="838d0-118">securityIdentifier</span></span>|<span data-ttu-id="838d0-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="838d0-119">String</span></span>|<span data-ttu-id="838d0-120">Die Sicherheits-ID der lokalen Benutzer oder Gruppen (z. B. \* S-1-5-32-544).</span><span class="sxs-lookup"><span data-stu-id="838d0-120">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="838d0-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="838d0-121">Relationships</span></span>
<span data-ttu-id="838d0-122">Keine</span><span class="sxs-lookup"><span data-stu-id="838d0-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="838d0-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="838d0-123">JSON Representation</span></span>
<span data-ttu-id="838d0-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="838d0-124">Here is a JSON representation of the resource.</span></span>
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




