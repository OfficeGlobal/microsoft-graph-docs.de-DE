---
title: mimeContent-Ressourcentyp
description: Enthält die Eigenschaften für generischen MIME-Inhalt.
ms.openlocfilehash: 7f25a1c16b86a45886cd763c1a8a3aa6142c47e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017620"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="3770d-103">mimeContent-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3770d-103">mimeContent resource type</span></span>

> <span data-ttu-id="3770d-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3770d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3770d-105">Enthält die Eigenschaften für generischen MIME-Inhalt.</span><span class="sxs-lookup"><span data-stu-id="3770d-105">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="3770d-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3770d-106">Properties</span></span>
|<span data-ttu-id="3770d-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3770d-107">Property</span></span>|<span data-ttu-id="3770d-108">Typ</span><span class="sxs-lookup"><span data-stu-id="3770d-108">Type</span></span>|<span data-ttu-id="3770d-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3770d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3770d-110">Typ</span><span class="sxs-lookup"><span data-stu-id="3770d-110">type</span></span>|<span data-ttu-id="3770d-111">String</span><span class="sxs-lookup"><span data-stu-id="3770d-111">String</span></span>|<span data-ttu-id="3770d-112">Gibt den MIME-Typ des Inhalts an.</span><span class="sxs-lookup"><span data-stu-id="3770d-112">Indicates the content mime type.</span></span>|
|<span data-ttu-id="3770d-113">Wert</span><span class="sxs-lookup"><span data-stu-id="3770d-113">value</span></span>|<span data-ttu-id="3770d-114">Binär</span><span class="sxs-lookup"><span data-stu-id="3770d-114">Binary</span></span>|<span data-ttu-id="3770d-115">Das Bytearray, das den tatsächlichen Inhalt enthält.</span><span class="sxs-lookup"><span data-stu-id="3770d-115">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3770d-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3770d-116">Relationships</span></span>
<span data-ttu-id="3770d-117">Keine</span><span class="sxs-lookup"><span data-stu-id="3770d-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3770d-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3770d-118">JSON Representation</span></span>
<span data-ttu-id="3770d-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3770d-119">Here is a JSON representation of the resource.</span></span>
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



