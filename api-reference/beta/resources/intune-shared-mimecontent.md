---
title: mimeContent-Ressourcentyp
description: Enthält die Eigenschaften für generischen MIME-Inhalt.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f446983d5dfe101c89171baa776b32759726f279
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161656"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="1583d-103">mimeContent-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1583d-103">mimeContent resource type</span></span>

> <span data-ttu-id="1583d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1583d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1583d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1583d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1583d-106">Enthält die Eigenschaften für generischen MIME-Inhalt.</span><span class="sxs-lookup"><span data-stu-id="1583d-106">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="1583d-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1583d-107">Properties</span></span>
|<span data-ttu-id="1583d-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1583d-108">Property</span></span>|<span data-ttu-id="1583d-109">Typ</span><span class="sxs-lookup"><span data-stu-id="1583d-109">Type</span></span>|<span data-ttu-id="1583d-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1583d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1583d-111">type</span><span class="sxs-lookup"><span data-stu-id="1583d-111">type</span></span>|<span data-ttu-id="1583d-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1583d-112">String</span></span>|<span data-ttu-id="1583d-113">Gibt den MIME-Typ des Inhalts an.</span><span class="sxs-lookup"><span data-stu-id="1583d-113">Indicates the content mime type.</span></span>|
|<span data-ttu-id="1583d-114">Wert</span><span class="sxs-lookup"><span data-stu-id="1583d-114">value</span></span>|<span data-ttu-id="1583d-115">Binär</span><span class="sxs-lookup"><span data-stu-id="1583d-115">Binary</span></span>|<span data-ttu-id="1583d-116">Das Bytearray, das den tatsächlichen Inhalt enthält.</span><span class="sxs-lookup"><span data-stu-id="1583d-116">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1583d-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1583d-117">Relationships</span></span>
<span data-ttu-id="1583d-118">Keine</span><span class="sxs-lookup"><span data-stu-id="1583d-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1583d-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1583d-119">JSON Representation</span></span>
<span data-ttu-id="1583d-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1583d-120">Here is a JSON representation of the resource.</span></span>
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




