---
title: mimeContent-Ressourcentyp
description: Enthält die Eigenschaften für generischen MIME-Inhalt.
ms.openlocfilehash: cc0d024c814588479e641114ad33d19a5e609ecd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063860"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="e022c-103">mimeContent-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e022c-103">mimeContent resource type</span></span>

> <span data-ttu-id="e022c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e022c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e022c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e022c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e022c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e022c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e022c-107">Enthält die Eigenschaften für generischen MIME-Inhalt.</span><span class="sxs-lookup"><span data-stu-id="e022c-107">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="e022c-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e022c-108">Properties</span></span>
|<span data-ttu-id="e022c-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e022c-109">Property</span></span>|<span data-ttu-id="e022c-110">Typ</span><span class="sxs-lookup"><span data-stu-id="e022c-110">Type</span></span>|<span data-ttu-id="e022c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e022c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e022c-112">Typ</span><span class="sxs-lookup"><span data-stu-id="e022c-112">type</span></span>|<span data-ttu-id="e022c-113">String</span><span class="sxs-lookup"><span data-stu-id="e022c-113">String</span></span>|<span data-ttu-id="e022c-114">Gibt den MIME-Typ des Inhalts an.</span><span class="sxs-lookup"><span data-stu-id="e022c-114">Indicates the content mime type.</span></span>|
|<span data-ttu-id="e022c-115">Wert</span><span class="sxs-lookup"><span data-stu-id="e022c-115">value</span></span>|<span data-ttu-id="e022c-116">Binär</span><span class="sxs-lookup"><span data-stu-id="e022c-116">Binary</span></span>|<span data-ttu-id="e022c-117">Das Bytearray, das den tatsächlichen Inhalt enthält.</span><span class="sxs-lookup"><span data-stu-id="e022c-117">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e022c-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e022c-118">Relationships</span></span>
<span data-ttu-id="e022c-119">Keine</span><span class="sxs-lookup"><span data-stu-id="e022c-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e022c-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e022c-120">JSON Representation</span></span>
<span data-ttu-id="e022c-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e022c-121">Here is a JSON representation of the resource.</span></span>
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





