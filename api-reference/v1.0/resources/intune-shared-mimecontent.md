---
title: mimeContent-Ressourcentyp
description: Enthält die Eigenschaften für generischen MIME-Inhalt.
author: tfitzmac
ms.openlocfilehash: 53776793fdd057ef057118decf2d72bb0b61a042
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307063"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="e09a7-103">mimeContent-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e09a7-103">mimeContent resource type</span></span>

> <span data-ttu-id="e09a7-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e09a7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e09a7-105">Enthält die Eigenschaften für generischen MIME-Inhalt.</span><span class="sxs-lookup"><span data-stu-id="e09a7-105">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="e09a7-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e09a7-106">Properties</span></span>
|<span data-ttu-id="e09a7-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e09a7-107">Property</span></span>|<span data-ttu-id="e09a7-108">Typ</span><span class="sxs-lookup"><span data-stu-id="e09a7-108">Type</span></span>|<span data-ttu-id="e09a7-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e09a7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e09a7-110">type</span><span class="sxs-lookup"><span data-stu-id="e09a7-110">type</span></span>|<span data-ttu-id="e09a7-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e09a7-111">String</span></span>|<span data-ttu-id="e09a7-112">Gibt den MIME-Typ des Inhalts an.</span><span class="sxs-lookup"><span data-stu-id="e09a7-112">Indicates the content mime type.</span></span>|
|<span data-ttu-id="e09a7-113">Wert</span><span class="sxs-lookup"><span data-stu-id="e09a7-113">value</span></span>|<span data-ttu-id="e09a7-114">Binär</span><span class="sxs-lookup"><span data-stu-id="e09a7-114">Binary</span></span>|<span data-ttu-id="e09a7-115">Das Bytearray, das den tatsächlichen Inhalt enthält.</span><span class="sxs-lookup"><span data-stu-id="e09a7-115">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e09a7-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e09a7-116">Relationships</span></span>
<span data-ttu-id="e09a7-117">Keine</span><span class="sxs-lookup"><span data-stu-id="e09a7-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e09a7-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e09a7-118">JSON Representation</span></span>
<span data-ttu-id="e09a7-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e09a7-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mimeContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mimeContent",
  "type": "String",
  "value": "binary"
}
```



