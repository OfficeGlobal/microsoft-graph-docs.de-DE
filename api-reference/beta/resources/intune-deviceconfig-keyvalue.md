---
title: KeyValue Ressourcentyp
description: Definition von Schlüssel-Wert.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: aae0fea85c5dd4f647a72c0fe66890bd8b82520b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885015"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="6c4c1-103">KeyValue Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6c4c1-103">keyValue resource type</span></span>

> <span data-ttu-id="6c4c1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6c4c1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c4c1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6c4c1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6c4c1-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6c4c1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6c4c1-107">Definition von Schlüssel-Wert.</span><span class="sxs-lookup"><span data-stu-id="6c4c1-107">Key Value definition.</span></span>
## <a name="properties"></a><span data-ttu-id="6c4c1-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6c4c1-108">Properties</span></span>
|<span data-ttu-id="6c4c1-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6c4c1-109">Property</span></span>|<span data-ttu-id="6c4c1-110">Typ</span><span class="sxs-lookup"><span data-stu-id="6c4c1-110">Type</span></span>|<span data-ttu-id="6c4c1-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6c4c1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c4c1-112">Key</span><span class="sxs-lookup"><span data-stu-id="6c4c1-112">key</span></span>|<span data-ttu-id="6c4c1-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6c4c1-113">String</span></span>|<span data-ttu-id="6c4c1-114">Schlüssel.</span><span class="sxs-lookup"><span data-stu-id="6c4c1-114">Key.</span></span>|
|<span data-ttu-id="6c4c1-115">Wert</span><span class="sxs-lookup"><span data-stu-id="6c4c1-115">value</span></span>|<span data-ttu-id="6c4c1-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6c4c1-116">String</span></span>|<span data-ttu-id="6c4c1-117">Wert.</span><span class="sxs-lookup"><span data-stu-id="6c4c1-117">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c4c1-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6c4c1-118">Relationships</span></span>
<span data-ttu-id="6c4c1-119">Keine</span><span class="sxs-lookup"><span data-stu-id="6c4c1-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6c4c1-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6c4c1-120">JSON Representation</span></span>
<span data-ttu-id="6c4c1-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6c4c1-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValue",
  "key": "String",
  "value": "String"
}
```





