---
title: KeyValue Ressourcentyp
description: Definition von Schlüssel-Wert.
author: tfitzmac
ms.openlocfilehash: 5e5754657e679f3a703c2b5dec7cea36d1bad860
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302639"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="ef80e-103">KeyValue Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ef80e-103">keyValue resource type</span></span>

> <span data-ttu-id="ef80e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ef80e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef80e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ef80e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ef80e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ef80e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef80e-107">Definition von Schlüssel-Wert.</span><span class="sxs-lookup"><span data-stu-id="ef80e-107">Key Value definition.</span></span>
## <a name="properties"></a><span data-ttu-id="ef80e-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ef80e-108">Properties</span></span>
|<span data-ttu-id="ef80e-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ef80e-109">Property</span></span>|<span data-ttu-id="ef80e-110">Typ</span><span class="sxs-lookup"><span data-stu-id="ef80e-110">Type</span></span>|<span data-ttu-id="ef80e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ef80e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef80e-112">Key</span><span class="sxs-lookup"><span data-stu-id="ef80e-112">key</span></span>|<span data-ttu-id="ef80e-113">String</span><span class="sxs-lookup"><span data-stu-id="ef80e-113">String</span></span>|<span data-ttu-id="ef80e-114">Schlüssel.</span><span class="sxs-lookup"><span data-stu-id="ef80e-114">Key.</span></span>|
|<span data-ttu-id="ef80e-115">Wert</span><span class="sxs-lookup"><span data-stu-id="ef80e-115">value</span></span>|<span data-ttu-id="ef80e-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ef80e-116">String</span></span>|<span data-ttu-id="ef80e-117">Wert.</span><span class="sxs-lookup"><span data-stu-id="ef80e-117">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef80e-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ef80e-118">Relationships</span></span>
<span data-ttu-id="ef80e-119">Keine</span><span class="sxs-lookup"><span data-stu-id="ef80e-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ef80e-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ef80e-120">JSON Representation</span></span>
<span data-ttu-id="ef80e-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ef80e-121">Here is a JSON representation of the resource.</span></span>
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





