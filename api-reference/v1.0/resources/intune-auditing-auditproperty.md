---
title: auditProperty-Ressourcentyp
description: Eine Klasse, die die Eigenschaften für die Audit-Eigenschaft enthält.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e91f3771be981f6ff410e8774f6a8ac9fbc121dd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870917"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="7d596-103">auditProperty-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7d596-103">auditProperty resource type</span></span>

> <span data-ttu-id="7d596-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7d596-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d596-105">Eine Klasse, die die Eigenschaften für die Audit-Eigenschaft enthält.</span><span class="sxs-lookup"><span data-stu-id="7d596-105">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="7d596-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7d596-106">Properties</span></span>
|<span data-ttu-id="7d596-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7d596-107">Property</span></span>|<span data-ttu-id="7d596-108">Typ</span><span class="sxs-lookup"><span data-stu-id="7d596-108">Type</span></span>|<span data-ttu-id="7d596-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7d596-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d596-110">displayName</span><span class="sxs-lookup"><span data-stu-id="7d596-110">displayName</span></span>|<span data-ttu-id="7d596-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7d596-111">String</span></span>|<span data-ttu-id="7d596-112">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="7d596-112">Display name.</span></span>|
|<span data-ttu-id="7d596-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="7d596-113">oldValue</span></span>|<span data-ttu-id="7d596-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7d596-114">String</span></span>|<span data-ttu-id="7d596-115">Alter Wert</span><span class="sxs-lookup"><span data-stu-id="7d596-115">Old value.</span></span>|
|<span data-ttu-id="7d596-116">newValue</span><span class="sxs-lookup"><span data-stu-id="7d596-116">newValue</span></span>|<span data-ttu-id="7d596-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7d596-117">String</span></span>|<span data-ttu-id="7d596-118">Neuer Wert</span><span class="sxs-lookup"><span data-stu-id="7d596-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d596-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7d596-119">Relationships</span></span>
<span data-ttu-id="7d596-120">Keine</span><span class="sxs-lookup"><span data-stu-id="7d596-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7d596-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7d596-121">JSON Representation</span></span>
<span data-ttu-id="7d596-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7d596-122">Here is a JSON representation of the resource.</span></span>
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



