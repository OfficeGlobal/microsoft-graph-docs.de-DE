---
title: auditResource-Ressourcentyp
description: Eine Klasse, die die Eigenschaften für die Audit-Ressource enthält.
ms.openlocfilehash: 452df4cb27dba5de04022c6ba7be08471286d866
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019009"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="bca6a-103">auditResource-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bca6a-103">auditResource resource type</span></span>

> <span data-ttu-id="bca6a-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bca6a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bca6a-105">Eine Klasse, die die Eigenschaften für die Audit-Ressource enthält.</span><span class="sxs-lookup"><span data-stu-id="bca6a-105">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="bca6a-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bca6a-106">Properties</span></span>
|<span data-ttu-id="bca6a-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bca6a-107">Property</span></span>|<span data-ttu-id="bca6a-108">Typ</span><span class="sxs-lookup"><span data-stu-id="bca6a-108">Type</span></span>|<span data-ttu-id="bca6a-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bca6a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bca6a-110">displayName</span><span class="sxs-lookup"><span data-stu-id="bca6a-110">displayName</span></span>|<span data-ttu-id="bca6a-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bca6a-111">String</span></span>|<span data-ttu-id="bca6a-112">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="bca6a-112">Display name.</span></span>|
|<span data-ttu-id="bca6a-113">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="bca6a-113">modifiedProperties</span></span>|<span data-ttu-id="bca6a-114">[auditProperty](../resources/intune-auditing-auditproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bca6a-114">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="bca6a-115">Liste der geänderten Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bca6a-115">List of modified properties.</span></span>|
|<span data-ttu-id="bca6a-116">Typ</span><span class="sxs-lookup"><span data-stu-id="bca6a-116">type</span></span>|<span data-ttu-id="bca6a-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bca6a-117">String</span></span>|<span data-ttu-id="bca6a-118">Typ der Audit-Ressource</span><span class="sxs-lookup"><span data-stu-id="bca6a-118">Audit resource's type.</span></span>|
|<span data-ttu-id="bca6a-119">resourceId</span><span class="sxs-lookup"><span data-stu-id="bca6a-119">resourceId</span></span>|<span data-ttu-id="bca6a-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bca6a-120">String</span></span>|<span data-ttu-id="bca6a-121">ID der Audit-Ressource</span><span class="sxs-lookup"><span data-stu-id="bca6a-121">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bca6a-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bca6a-122">Relationships</span></span>
<span data-ttu-id="bca6a-123">Keine</span><span class="sxs-lookup"><span data-stu-id="bca6a-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bca6a-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bca6a-124">JSON Representation</span></span>
<span data-ttu-id="bca6a-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bca6a-125">Here is a JSON representation of the resource.</span></span>
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



