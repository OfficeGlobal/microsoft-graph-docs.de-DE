---
title: auditProperty-Ressourcentyp
description: Eine Klasse, die die Eigenschaften für die Audit-Eigenschaft enthält.
ms.openlocfilehash: eaffa5552d611ac2ef8bb236009b9520d1134586
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019461"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="c6aea-103">auditProperty-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c6aea-103">auditProperty resource type</span></span>

> <span data-ttu-id="c6aea-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c6aea-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6aea-105">Eine Klasse, die die Eigenschaften für die Audit-Eigenschaft enthält.</span><span class="sxs-lookup"><span data-stu-id="c6aea-105">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="c6aea-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c6aea-106">Properties</span></span>
|<span data-ttu-id="c6aea-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c6aea-107">Property</span></span>|<span data-ttu-id="c6aea-108">Typ</span><span class="sxs-lookup"><span data-stu-id="c6aea-108">Type</span></span>|<span data-ttu-id="c6aea-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c6aea-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6aea-110">displayName</span><span class="sxs-lookup"><span data-stu-id="c6aea-110">displayName</span></span>|<span data-ttu-id="c6aea-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c6aea-111">String</span></span>|<span data-ttu-id="c6aea-112">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="c6aea-112">Display name.</span></span>|
|<span data-ttu-id="c6aea-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="c6aea-113">oldValue</span></span>|<span data-ttu-id="c6aea-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c6aea-114">String</span></span>|<span data-ttu-id="c6aea-115">Alter Wert</span><span class="sxs-lookup"><span data-stu-id="c6aea-115">Old value.</span></span>|
|<span data-ttu-id="c6aea-116">newValue</span><span class="sxs-lookup"><span data-stu-id="c6aea-116">newValue</span></span>|<span data-ttu-id="c6aea-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c6aea-117">String</span></span>|<span data-ttu-id="c6aea-118">Neuer Wert</span><span class="sxs-lookup"><span data-stu-id="c6aea-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6aea-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c6aea-119">Relationships</span></span>
<span data-ttu-id="c6aea-120">Keine</span><span class="sxs-lookup"><span data-stu-id="c6aea-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c6aea-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c6aea-121">JSON Representation</span></span>
<span data-ttu-id="c6aea-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c6aea-122">Here is a JSON representation of the resource.</span></span>
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



