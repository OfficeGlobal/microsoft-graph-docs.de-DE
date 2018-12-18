---
title: auditProperty-Ressourcentyp
description: Eine Klasse, die die Eigenschaften für die Audit-Eigenschaft enthält.
author: tfitzmac
ms.openlocfilehash: 2d7cd7f1fbbf9f813cf447ca53e0d4652eb0feda
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312901"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="60fe9-103">auditProperty-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="60fe9-103">auditProperty resource type</span></span>

> <span data-ttu-id="60fe9-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="60fe9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="60fe9-105">Eine Klasse, die die Eigenschaften für die Audit-Eigenschaft enthält.</span><span class="sxs-lookup"><span data-stu-id="60fe9-105">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="60fe9-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="60fe9-106">Properties</span></span>
|<span data-ttu-id="60fe9-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="60fe9-107">Property</span></span>|<span data-ttu-id="60fe9-108">Typ</span><span class="sxs-lookup"><span data-stu-id="60fe9-108">Type</span></span>|<span data-ttu-id="60fe9-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="60fe9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60fe9-110">displayName</span><span class="sxs-lookup"><span data-stu-id="60fe9-110">displayName</span></span>|<span data-ttu-id="60fe9-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="60fe9-111">String</span></span>|<span data-ttu-id="60fe9-112">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="60fe9-112">Display name.</span></span>|
|<span data-ttu-id="60fe9-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="60fe9-113">oldValue</span></span>|<span data-ttu-id="60fe9-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="60fe9-114">String</span></span>|<span data-ttu-id="60fe9-115">Alter Wert</span><span class="sxs-lookup"><span data-stu-id="60fe9-115">Old value.</span></span>|
|<span data-ttu-id="60fe9-116">newValue</span><span class="sxs-lookup"><span data-stu-id="60fe9-116">newValue</span></span>|<span data-ttu-id="60fe9-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="60fe9-117">String</span></span>|<span data-ttu-id="60fe9-118">Neuer Wert</span><span class="sxs-lookup"><span data-stu-id="60fe9-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60fe9-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="60fe9-119">Relationships</span></span>
<span data-ttu-id="60fe9-120">Keine</span><span class="sxs-lookup"><span data-stu-id="60fe9-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="60fe9-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="60fe9-121">JSON Representation</span></span>
<span data-ttu-id="60fe9-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="60fe9-122">Here is a JSON representation of the resource.</span></span>
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



