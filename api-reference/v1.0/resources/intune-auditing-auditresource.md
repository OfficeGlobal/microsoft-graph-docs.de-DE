---
title: auditResource-Ressourcentyp
description: Eine Klasse, die die Eigenschaften für die Audit-Ressource enthält.
author: tfitzmac
ms.openlocfilehash: 5cfc23a80b2247b9f561d802ce844091c623ef62
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302660"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="184fd-103">auditResource-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="184fd-103">auditResource resource type</span></span>

> <span data-ttu-id="184fd-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="184fd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="184fd-105">Eine Klasse, die die Eigenschaften für die Audit-Ressource enthält.</span><span class="sxs-lookup"><span data-stu-id="184fd-105">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="184fd-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="184fd-106">Properties</span></span>
|<span data-ttu-id="184fd-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="184fd-107">Property</span></span>|<span data-ttu-id="184fd-108">Typ</span><span class="sxs-lookup"><span data-stu-id="184fd-108">Type</span></span>|<span data-ttu-id="184fd-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="184fd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="184fd-110">displayName</span><span class="sxs-lookup"><span data-stu-id="184fd-110">displayName</span></span>|<span data-ttu-id="184fd-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="184fd-111">String</span></span>|<span data-ttu-id="184fd-112">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="184fd-112">Display name.</span></span>|
|<span data-ttu-id="184fd-113">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="184fd-113">modifiedProperties</span></span>|<span data-ttu-id="184fd-114">[auditProperty](../resources/intune-auditing-auditproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="184fd-114">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="184fd-115">Liste der geänderten Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="184fd-115">List of modified properties.</span></span>|
|<span data-ttu-id="184fd-116">Typ</span><span class="sxs-lookup"><span data-stu-id="184fd-116">type</span></span>|<span data-ttu-id="184fd-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="184fd-117">String</span></span>|<span data-ttu-id="184fd-118">Typ der Audit-Ressource</span><span class="sxs-lookup"><span data-stu-id="184fd-118">Audit resource's type.</span></span>|
|<span data-ttu-id="184fd-119">resourceId</span><span class="sxs-lookup"><span data-stu-id="184fd-119">resourceId</span></span>|<span data-ttu-id="184fd-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="184fd-120">String</span></span>|<span data-ttu-id="184fd-121">ID der Audit-Ressource</span><span class="sxs-lookup"><span data-stu-id="184fd-121">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="184fd-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="184fd-122">Relationships</span></span>
<span data-ttu-id="184fd-123">Keine</span><span class="sxs-lookup"><span data-stu-id="184fd-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="184fd-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="184fd-124">JSON Representation</span></span>
<span data-ttu-id="184fd-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="184fd-125">Here is a JSON representation of the resource.</span></span>
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



