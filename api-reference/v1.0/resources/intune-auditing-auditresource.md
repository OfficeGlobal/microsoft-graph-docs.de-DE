---
title: auditResource-Ressourcentyp
description: Eine Klasse, die die Eigenschaften für die Audit-Ressource enthält.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7f8fc3a96b3d17759e1e65eaa17c6571e4cec347
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844737"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="a20a1-103">auditResource-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a20a1-103">auditResource resource type</span></span>

> <span data-ttu-id="a20a1-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a20a1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a20a1-105">Eine Klasse, die die Eigenschaften für die Audit-Ressource enthält.</span><span class="sxs-lookup"><span data-stu-id="a20a1-105">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="a20a1-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a20a1-106">Properties</span></span>
|<span data-ttu-id="a20a1-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a20a1-107">Property</span></span>|<span data-ttu-id="a20a1-108">Typ</span><span class="sxs-lookup"><span data-stu-id="a20a1-108">Type</span></span>|<span data-ttu-id="a20a1-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a20a1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a20a1-110">displayName</span><span class="sxs-lookup"><span data-stu-id="a20a1-110">displayName</span></span>|<span data-ttu-id="a20a1-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a20a1-111">String</span></span>|<span data-ttu-id="a20a1-112">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="a20a1-112">Display name.</span></span>|
|<span data-ttu-id="a20a1-113">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="a20a1-113">modifiedProperties</span></span>|<span data-ttu-id="a20a1-114">[auditProperty](../resources/intune-auditing-auditproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a20a1-114">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="a20a1-115">Liste der geänderten Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a20a1-115">List of modified properties.</span></span>|
|<span data-ttu-id="a20a1-116">Typ</span><span class="sxs-lookup"><span data-stu-id="a20a1-116">type</span></span>|<span data-ttu-id="a20a1-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a20a1-117">String</span></span>|<span data-ttu-id="a20a1-118">Typ der Audit-Ressource</span><span class="sxs-lookup"><span data-stu-id="a20a1-118">Audit resource's type.</span></span>|
|<span data-ttu-id="a20a1-119">resourceId</span><span class="sxs-lookup"><span data-stu-id="a20a1-119">resourceId</span></span>|<span data-ttu-id="a20a1-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a20a1-120">String</span></span>|<span data-ttu-id="a20a1-121">ID der Audit-Ressource</span><span class="sxs-lookup"><span data-stu-id="a20a1-121">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a20a1-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a20a1-122">Relationships</span></span>
<span data-ttu-id="a20a1-123">Keine</span><span class="sxs-lookup"><span data-stu-id="a20a1-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a20a1-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a20a1-124">JSON Representation</span></span>
<span data-ttu-id="a20a1-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a20a1-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditResource",
  "displayName": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.auditProperty",
      "displayName": "String",
      "oldValue": "String",
      "newValue": "String"
    }
  ],
  "type": "String",
  "resourceId": "String"
}
```



