---
title: keyValuePair-Ressourcentyp
description: Schlüssel-Wert-Paar zum Speichern benutzerdefinierter Einstellungen
ms.openlocfilehash: 803dd9e347ef06bc9d4a9fce13d2265c4fc969a3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019194"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="6bf9b-103">keyValuePair-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6bf9b-103">keyValuePair resource type</span></span>

> <span data-ttu-id="6bf9b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6bf9b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6bf9b-105">Schlüssel-Wert-Paar zum Speichern benutzerdefinierter Einstellungen</span><span class="sxs-lookup"><span data-stu-id="6bf9b-105">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="6bf9b-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6bf9b-106">Properties</span></span>
|<span data-ttu-id="6bf9b-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6bf9b-107">Property</span></span>|<span data-ttu-id="6bf9b-108">Typ</span><span class="sxs-lookup"><span data-stu-id="6bf9b-108">Type</span></span>|<span data-ttu-id="6bf9b-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6bf9b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bf9b-110">name</span><span class="sxs-lookup"><span data-stu-id="6bf9b-110">name</span></span>|<span data-ttu-id="6bf9b-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6bf9b-111">String</span></span>|<span data-ttu-id="6bf9b-112">Namen für dieses Schlüssel-Wert-Paar</span><span class="sxs-lookup"><span data-stu-id="6bf9b-112">Name for this key-value pair</span></span>|
|<span data-ttu-id="6bf9b-113">Wert</span><span class="sxs-lookup"><span data-stu-id="6bf9b-113">value</span></span>|<span data-ttu-id="6bf9b-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6bf9b-114">String</span></span>|<span data-ttu-id="6bf9b-115">Wert für dieses Schlüssel-Wert-Paar</span><span class="sxs-lookup"><span data-stu-id="6bf9b-115">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="6bf9b-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6bf9b-116">Relationships</span></span>
<span data-ttu-id="6bf9b-117">Keine</span><span class="sxs-lookup"><span data-stu-id="6bf9b-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6bf9b-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6bf9b-118">JSON Representation</span></span>
<span data-ttu-id="6bf9b-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6bf9b-119">Here is a JSON representation of the resource.</span></span>
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



