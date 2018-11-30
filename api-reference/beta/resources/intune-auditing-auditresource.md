---
title: auditResource-Ressourcentyp
description: Eine Klasse, die die Eigenschaften für die Audit-Ressource enthält.
ms.openlocfilehash: a3825418c1406bbe9fcce7feeba96217342c735e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063740"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="0e2a9-103">auditResource-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0e2a9-103">auditResource resource type</span></span>

> <span data-ttu-id="0e2a9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0e2a9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e2a9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0e2a9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0e2a9-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0e2a9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0e2a9-107">Eine Klasse, die die Eigenschaften für die Audit-Ressource enthält.</span><span class="sxs-lookup"><span data-stu-id="0e2a9-107">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="0e2a9-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0e2a9-108">Properties</span></span>
|<span data-ttu-id="0e2a9-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0e2a9-109">Property</span></span>|<span data-ttu-id="0e2a9-110">Typ</span><span class="sxs-lookup"><span data-stu-id="0e2a9-110">Type</span></span>|<span data-ttu-id="0e2a9-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e2a9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e2a9-112">displayName</span><span class="sxs-lookup"><span data-stu-id="0e2a9-112">displayName</span></span>|<span data-ttu-id="0e2a9-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0e2a9-113">String</span></span>|<span data-ttu-id="0e2a9-114">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="0e2a9-114">Display name.</span></span>|
|<span data-ttu-id="0e2a9-115">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="0e2a9-115">modifiedProperties</span></span>|<span data-ttu-id="0e2a9-116">[auditProperty](../resources/intune-auditing-auditproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="0e2a9-116">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="0e2a9-117">Liste der geänderten Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0e2a9-117">List of modified properties.</span></span>|
|<span data-ttu-id="0e2a9-118">Typ</span><span class="sxs-lookup"><span data-stu-id="0e2a9-118">type</span></span>|<span data-ttu-id="0e2a9-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0e2a9-119">String</span></span>|<span data-ttu-id="0e2a9-120">Typ der Audit-Ressource</span><span class="sxs-lookup"><span data-stu-id="0e2a9-120">Audit resource's type.</span></span>|
|<span data-ttu-id="0e2a9-121">resourceId</span><span class="sxs-lookup"><span data-stu-id="0e2a9-121">resourceId</span></span>|<span data-ttu-id="0e2a9-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0e2a9-122">String</span></span>|<span data-ttu-id="0e2a9-123">ID der Audit-Ressource</span><span class="sxs-lookup"><span data-stu-id="0e2a9-123">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e2a9-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0e2a9-124">Relationships</span></span>
<span data-ttu-id="0e2a9-125">Keine</span><span class="sxs-lookup"><span data-stu-id="0e2a9-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0e2a9-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0e2a9-126">JSON Representation</span></span>
<span data-ttu-id="0e2a9-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0e2a9-127">Here is a JSON representation of the resource.</span></span>
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





