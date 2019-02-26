---
title: keyValuePair-Ressourcentyp
description: Schlüssel-Wert-Paar zum Speichern benutzerdefinierter Einstellungen
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ed4af707320da09c9b72537168f8fd77a424c790
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258737"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="7bc51-103">keyValuePair-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7bc51-103">keyValuePair resource type</span></span>

> <span data-ttu-id="7bc51-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7bc51-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bc51-105">Schlüssel-Wert-Paar zum Speichern benutzerdefinierter Einstellungen</span><span class="sxs-lookup"><span data-stu-id="7bc51-105">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="7bc51-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7bc51-106">Properties</span></span>
|<span data-ttu-id="7bc51-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7bc51-107">Property</span></span>|<span data-ttu-id="7bc51-108">Typ</span><span class="sxs-lookup"><span data-stu-id="7bc51-108">Type</span></span>|<span data-ttu-id="7bc51-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7bc51-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bc51-110">name</span><span class="sxs-lookup"><span data-stu-id="7bc51-110">name</span></span>|<span data-ttu-id="7bc51-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7bc51-111">String</span></span>|<span data-ttu-id="7bc51-112">Namen für dieses Schlüssel-Wert-Paar</span><span class="sxs-lookup"><span data-stu-id="7bc51-112">Name for this key-value pair</span></span>|
|<span data-ttu-id="7bc51-113">Wert</span><span class="sxs-lookup"><span data-stu-id="7bc51-113">value</span></span>|<span data-ttu-id="7bc51-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7bc51-114">String</span></span>|<span data-ttu-id="7bc51-115">Wert für dieses Schlüssel-Wert-Paar</span><span class="sxs-lookup"><span data-stu-id="7bc51-115">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="7bc51-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7bc51-116">Relationships</span></span>
<span data-ttu-id="7bc51-117">Keine</span><span class="sxs-lookup"><span data-stu-id="7bc51-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7bc51-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7bc51-118">JSON Representation</span></span>
<span data-ttu-id="7bc51-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7bc51-119">Here is a JSON representation of the resource.</span></span>
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



