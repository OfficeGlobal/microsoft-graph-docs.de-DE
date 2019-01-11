---
title: mimeContent-Ressourcentyp
description: Enthält die Eigenschaften für generischen MIME-Inhalt.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 826606d41feb0f0a156a1b8240bde7f4ac926a5a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838227"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="94220-103">mimeContent-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="94220-103">mimeContent resource type</span></span>

> <span data-ttu-id="94220-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="94220-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94220-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="94220-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="94220-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="94220-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="94220-107">Enthält die Eigenschaften für generischen MIME-Inhalt.</span><span class="sxs-lookup"><span data-stu-id="94220-107">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="94220-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="94220-108">Properties</span></span>
|<span data-ttu-id="94220-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="94220-109">Property</span></span>|<span data-ttu-id="94220-110">Typ</span><span class="sxs-lookup"><span data-stu-id="94220-110">Type</span></span>|<span data-ttu-id="94220-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="94220-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94220-112">type</span><span class="sxs-lookup"><span data-stu-id="94220-112">type</span></span>|<span data-ttu-id="94220-113">String</span><span class="sxs-lookup"><span data-stu-id="94220-113">String</span></span>|<span data-ttu-id="94220-114">Gibt den MIME-Typ des Inhalts an.</span><span class="sxs-lookup"><span data-stu-id="94220-114">Indicates the content mime type.</span></span>|
|<span data-ttu-id="94220-115">Wert</span><span class="sxs-lookup"><span data-stu-id="94220-115">value</span></span>|<span data-ttu-id="94220-116">Binär</span><span class="sxs-lookup"><span data-stu-id="94220-116">Binary</span></span>|<span data-ttu-id="94220-117">Das Bytearray, das den tatsächlichen Inhalt enthält.</span><span class="sxs-lookup"><span data-stu-id="94220-117">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94220-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="94220-118">Relationships</span></span>
<span data-ttu-id="94220-119">Keine</span><span class="sxs-lookup"><span data-stu-id="94220-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="94220-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="94220-120">JSON Representation</span></span>
<span data-ttu-id="94220-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="94220-121">Here is a JSON representation of the resource.</span></span>
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





