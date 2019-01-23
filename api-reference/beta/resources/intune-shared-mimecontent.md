---
title: mimeContent-Ressourcentyp
description: Enthält die Eigenschaften für generischen MIME-Inhalt.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 62132b9e55b8130f82fc8414cbb6e90ba34bb70f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413458"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="c4899-103">mimeContent-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c4899-103">mimeContent resource type</span></span>

> <span data-ttu-id="c4899-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="c4899-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c4899-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c4899-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c4899-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c4899-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4899-107">Enthält die Eigenschaften für generischen MIME-Inhalt.</span><span class="sxs-lookup"><span data-stu-id="c4899-107">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="c4899-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c4899-108">Properties</span></span>
|<span data-ttu-id="c4899-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c4899-109">Property</span></span>|<span data-ttu-id="c4899-110">Typ</span><span class="sxs-lookup"><span data-stu-id="c4899-110">Type</span></span>|<span data-ttu-id="c4899-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c4899-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4899-112">type</span><span class="sxs-lookup"><span data-stu-id="c4899-112">type</span></span>|<span data-ttu-id="c4899-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c4899-113">String</span></span>|<span data-ttu-id="c4899-114">Gibt den MIME-Typ des Inhalts an.</span><span class="sxs-lookup"><span data-stu-id="c4899-114">Indicates the content mime type.</span></span>|
|<span data-ttu-id="c4899-115">Wert</span><span class="sxs-lookup"><span data-stu-id="c4899-115">value</span></span>|<span data-ttu-id="c4899-116">Binär</span><span class="sxs-lookup"><span data-stu-id="c4899-116">Binary</span></span>|<span data-ttu-id="c4899-117">Das Bytearray, das den tatsächlichen Inhalt enthält.</span><span class="sxs-lookup"><span data-stu-id="c4899-117">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c4899-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c4899-118">Relationships</span></span>
<span data-ttu-id="c4899-119">Keine</span><span class="sxs-lookup"><span data-stu-id="c4899-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c4899-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c4899-120">JSON Representation</span></span>
<span data-ttu-id="c4899-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c4899-121">Here is a JSON representation of the resource.</span></span>
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




