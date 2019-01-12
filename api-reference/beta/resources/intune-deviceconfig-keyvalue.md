---
title: KeyValue Ressourcentyp
description: Definition von Schlüssel-Wert.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5027388b455a41bc5895009a4ce79ca195ab8340
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957879"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="0f1da-103">KeyValue Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0f1da-103">keyValue resource type</span></span>

> <span data-ttu-id="0f1da-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0f1da-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f1da-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0f1da-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f1da-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0f1da-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f1da-107">Definition von Schlüssel-Wert.</span><span class="sxs-lookup"><span data-stu-id="0f1da-107">Key Value definition.</span></span>
## <a name="properties"></a><span data-ttu-id="0f1da-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0f1da-108">Properties</span></span>
|<span data-ttu-id="0f1da-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0f1da-109">Property</span></span>|<span data-ttu-id="0f1da-110">Typ</span><span class="sxs-lookup"><span data-stu-id="0f1da-110">Type</span></span>|<span data-ttu-id="0f1da-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f1da-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f1da-112">Key</span><span class="sxs-lookup"><span data-stu-id="0f1da-112">key</span></span>|<span data-ttu-id="0f1da-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0f1da-113">String</span></span>|<span data-ttu-id="0f1da-114">Schlüssel.</span><span class="sxs-lookup"><span data-stu-id="0f1da-114">Key.</span></span>|
|<span data-ttu-id="0f1da-115">Wert</span><span class="sxs-lookup"><span data-stu-id="0f1da-115">value</span></span>|<span data-ttu-id="0f1da-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0f1da-116">String</span></span>|<span data-ttu-id="0f1da-117">Wert.</span><span class="sxs-lookup"><span data-stu-id="0f1da-117">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f1da-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0f1da-118">Relationships</span></span>
<span data-ttu-id="0f1da-119">Keine</span><span class="sxs-lookup"><span data-stu-id="0f1da-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0f1da-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0f1da-120">JSON Representation</span></span>
<span data-ttu-id="0f1da-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0f1da-121">Here is a JSON representation of the resource.</span></span>
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





