---
title: auditProperty-Ressourcentyp
description: Eine Klasse, die die Eigenschaften für die Audit-Eigenschaft enthält.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0d06bd1b628848a34e6fa830a525c049526b46ee
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139032"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="14555-103">auditProperty-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="14555-103">auditProperty resource type</span></span>

> <span data-ttu-id="14555-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="14555-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14555-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="14555-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14555-106">Eine Klasse, die die Eigenschaften für die Audit-Eigenschaft enthält.</span><span class="sxs-lookup"><span data-stu-id="14555-106">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="14555-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="14555-107">Properties</span></span>
|<span data-ttu-id="14555-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="14555-108">Property</span></span>|<span data-ttu-id="14555-109">Typ</span><span class="sxs-lookup"><span data-stu-id="14555-109">Type</span></span>|<span data-ttu-id="14555-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="14555-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14555-111">displayName</span><span class="sxs-lookup"><span data-stu-id="14555-111">displayName</span></span>|<span data-ttu-id="14555-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="14555-112">String</span></span>|<span data-ttu-id="14555-113">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="14555-113">Display name.</span></span>|
|<span data-ttu-id="14555-114">oldValue</span><span class="sxs-lookup"><span data-stu-id="14555-114">oldValue</span></span>|<span data-ttu-id="14555-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="14555-115">String</span></span>|<span data-ttu-id="14555-116">Alter Wert</span><span class="sxs-lookup"><span data-stu-id="14555-116">Old value.</span></span>|
|<span data-ttu-id="14555-117">newValue</span><span class="sxs-lookup"><span data-stu-id="14555-117">newValue</span></span>|<span data-ttu-id="14555-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="14555-118">String</span></span>|<span data-ttu-id="14555-119">Neuer Wert</span><span class="sxs-lookup"><span data-stu-id="14555-119">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14555-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="14555-120">Relationships</span></span>
<span data-ttu-id="14555-121">Keine</span><span class="sxs-lookup"><span data-stu-id="14555-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="14555-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="14555-122">JSON Representation</span></span>
<span data-ttu-id="14555-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="14555-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditProperty",
  "displayName": "String",
  "oldValue": "String",
  "newValue": "String"
}
```




