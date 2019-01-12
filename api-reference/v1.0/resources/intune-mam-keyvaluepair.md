---
title: keyValuePair-Ressourcentyp
description: Schlüssel-Wert-Paar zum Speichern benutzerdefinierter Einstellungen
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: db3e24c1c14cb208be66b7a2b0364ad12b162956
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926442"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="72cf9-103">keyValuePair-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="72cf9-103">keyValuePair resource type</span></span>

> <span data-ttu-id="72cf9-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="72cf9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="72cf9-105">Schlüssel-Wert-Paar zum Speichern benutzerdefinierter Einstellungen</span><span class="sxs-lookup"><span data-stu-id="72cf9-105">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="72cf9-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="72cf9-106">Properties</span></span>
|<span data-ttu-id="72cf9-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="72cf9-107">Property</span></span>|<span data-ttu-id="72cf9-108">Typ</span><span class="sxs-lookup"><span data-stu-id="72cf9-108">Type</span></span>|<span data-ttu-id="72cf9-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="72cf9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72cf9-110">name</span><span class="sxs-lookup"><span data-stu-id="72cf9-110">name</span></span>|<span data-ttu-id="72cf9-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="72cf9-111">String</span></span>|<span data-ttu-id="72cf9-112">Namen für dieses Schlüssel-Wert-Paar</span><span class="sxs-lookup"><span data-stu-id="72cf9-112">Name for this key-value pair</span></span>|
|<span data-ttu-id="72cf9-113">Wert</span><span class="sxs-lookup"><span data-stu-id="72cf9-113">value</span></span>|<span data-ttu-id="72cf9-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="72cf9-114">String</span></span>|<span data-ttu-id="72cf9-115">Wert für dieses Schlüssel-Wert-Paar</span><span class="sxs-lookup"><span data-stu-id="72cf9-115">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="72cf9-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="72cf9-116">Relationships</span></span>
<span data-ttu-id="72cf9-117">Keine</span><span class="sxs-lookup"><span data-stu-id="72cf9-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="72cf9-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="72cf9-118">JSON Representation</span></span>
<span data-ttu-id="72cf9-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="72cf9-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValuePair",
  "name": "String",
  "value": "String"
}
```



