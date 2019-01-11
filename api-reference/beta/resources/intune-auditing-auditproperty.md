---
title: auditProperty-Ressourcentyp
description: Eine Klasse, die die Eigenschaften für die Audit-Eigenschaft enthält.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b0a04d924560e712a0656584693940b127210645
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812866"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="56b1b-103">auditProperty-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="56b1b-103">auditProperty resource type</span></span>

> <span data-ttu-id="56b1b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="56b1b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56b1b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="56b1b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="56b1b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="56b1b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56b1b-107">Eine Klasse, die die Eigenschaften für die Audit-Eigenschaft enthält.</span><span class="sxs-lookup"><span data-stu-id="56b1b-107">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="56b1b-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="56b1b-108">Properties</span></span>
|<span data-ttu-id="56b1b-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="56b1b-109">Property</span></span>|<span data-ttu-id="56b1b-110">Typ</span><span class="sxs-lookup"><span data-stu-id="56b1b-110">Type</span></span>|<span data-ttu-id="56b1b-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="56b1b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56b1b-112">displayName</span><span class="sxs-lookup"><span data-stu-id="56b1b-112">displayName</span></span>|<span data-ttu-id="56b1b-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="56b1b-113">String</span></span>|<span data-ttu-id="56b1b-114">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="56b1b-114">Display name.</span></span>|
|<span data-ttu-id="56b1b-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="56b1b-115">oldValue</span></span>|<span data-ttu-id="56b1b-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="56b1b-116">String</span></span>|<span data-ttu-id="56b1b-117">Alter Wert</span><span class="sxs-lookup"><span data-stu-id="56b1b-117">Old value.</span></span>|
|<span data-ttu-id="56b1b-118">newValue</span><span class="sxs-lookup"><span data-stu-id="56b1b-118">newValue</span></span>|<span data-ttu-id="56b1b-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="56b1b-119">String</span></span>|<span data-ttu-id="56b1b-120">Neuer Wert</span><span class="sxs-lookup"><span data-stu-id="56b1b-120">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56b1b-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="56b1b-121">Relationships</span></span>
<span data-ttu-id="56b1b-122">Keine</span><span class="sxs-lookup"><span data-stu-id="56b1b-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="56b1b-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="56b1b-123">JSON Representation</span></span>
<span data-ttu-id="56b1b-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="56b1b-124">Here is a JSON representation of the resource.</span></span>
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





