---
title: mimeContent-Ressourcentyp
description: Enthält die Eigenschaften für generischen MIME-Inhalt.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de4360ce5a8873fde7d3286f55fc0c8993936a7c
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260004"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="c579b-103">mimeContent-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c579b-103">mimeContent resource type</span></span>

> <span data-ttu-id="c579b-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c579b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c579b-105">Enthält die Eigenschaften für generischen MIME-Inhalt.</span><span class="sxs-lookup"><span data-stu-id="c579b-105">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="c579b-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c579b-106">Properties</span></span>
|<span data-ttu-id="c579b-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c579b-107">Property</span></span>|<span data-ttu-id="c579b-108">Typ</span><span class="sxs-lookup"><span data-stu-id="c579b-108">Type</span></span>|<span data-ttu-id="c579b-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c579b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c579b-110">type</span><span class="sxs-lookup"><span data-stu-id="c579b-110">type</span></span>|<span data-ttu-id="c579b-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c579b-111">String</span></span>|<span data-ttu-id="c579b-112">Gibt den MIME-Typ des Inhalts an.</span><span class="sxs-lookup"><span data-stu-id="c579b-112">Indicates the content mime type.</span></span>|
|<span data-ttu-id="c579b-113">Wert</span><span class="sxs-lookup"><span data-stu-id="c579b-113">value</span></span>|<span data-ttu-id="c579b-114">Binär</span><span class="sxs-lookup"><span data-stu-id="c579b-114">Binary</span></span>|<span data-ttu-id="c579b-115">Das Bytearray, das den tatsächlichen Inhalt enthält.</span><span class="sxs-lookup"><span data-stu-id="c579b-115">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c579b-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c579b-116">Relationships</span></span>
<span data-ttu-id="c579b-117">Keine</span><span class="sxs-lookup"><span data-stu-id="c579b-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c579b-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c579b-118">JSON Representation</span></span>
<span data-ttu-id="c579b-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c579b-119">Here is a JSON representation of the resource.</span></span>
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



