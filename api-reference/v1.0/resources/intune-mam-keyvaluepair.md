---
title: keyValuePair-Ressourcentyp
description: Schlüssel-Wert-Paar zum Speichern benutzerdefinierter Einstellungen
author: tfitzmac
ms.openlocfilehash: 078d414330e7a6c333042b6f6eb83ec44e255d73
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355076"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="61ee7-103">keyValuePair-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="61ee7-103">keyValuePair resource type</span></span>

> <span data-ttu-id="61ee7-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="61ee7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61ee7-105">Schlüssel-Wert-Paar zum Speichern benutzerdefinierter Einstellungen</span><span class="sxs-lookup"><span data-stu-id="61ee7-105">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="61ee7-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="61ee7-106">Properties</span></span>
|<span data-ttu-id="61ee7-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="61ee7-107">Property</span></span>|<span data-ttu-id="61ee7-108">Typ</span><span class="sxs-lookup"><span data-stu-id="61ee7-108">Type</span></span>|<span data-ttu-id="61ee7-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61ee7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61ee7-110">name</span><span class="sxs-lookup"><span data-stu-id="61ee7-110">name</span></span>|<span data-ttu-id="61ee7-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="61ee7-111">String</span></span>|<span data-ttu-id="61ee7-112">Namen für dieses Schlüssel-Wert-Paar</span><span class="sxs-lookup"><span data-stu-id="61ee7-112">Name for this key-value pair</span></span>|
|<span data-ttu-id="61ee7-113">Wert</span><span class="sxs-lookup"><span data-stu-id="61ee7-113">value</span></span>|<span data-ttu-id="61ee7-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="61ee7-114">String</span></span>|<span data-ttu-id="61ee7-115">Wert für dieses Schlüssel-Wert-Paar</span><span class="sxs-lookup"><span data-stu-id="61ee7-115">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="61ee7-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="61ee7-116">Relationships</span></span>
<span data-ttu-id="61ee7-117">Keine</span><span class="sxs-lookup"><span data-stu-id="61ee7-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="61ee7-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="61ee7-118">JSON Representation</span></span>
<span data-ttu-id="61ee7-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="61ee7-119">Here is a JSON representation of the resource.</span></span>
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



