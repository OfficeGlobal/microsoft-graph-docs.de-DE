---
title: keyValuePair-Ressourcentyp
description: Schlüssel-Wert-Paar zum Speichern benutzerdefinierter Einstellungen
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5a8feecabeca3cfc916c0bd3ce1b87cab3a68809
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160795"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="64f67-103">keyValuePair-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="64f67-103">keyValuePair resource type</span></span>

> <span data-ttu-id="64f67-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="64f67-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64f67-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="64f67-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64f67-106">Schlüssel-Wert-Paar zum Speichern benutzerdefinierter Einstellungen</span><span class="sxs-lookup"><span data-stu-id="64f67-106">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="64f67-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="64f67-107">Properties</span></span>
|<span data-ttu-id="64f67-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="64f67-108">Property</span></span>|<span data-ttu-id="64f67-109">Typ</span><span class="sxs-lookup"><span data-stu-id="64f67-109">Type</span></span>|<span data-ttu-id="64f67-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="64f67-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64f67-111">name</span><span class="sxs-lookup"><span data-stu-id="64f67-111">name</span></span>|<span data-ttu-id="64f67-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="64f67-112">String</span></span>|<span data-ttu-id="64f67-113">Namen für dieses Schlüssel-Wert-Paar</span><span class="sxs-lookup"><span data-stu-id="64f67-113">Name for this key-value pair</span></span>|
|<span data-ttu-id="64f67-114">Wert</span><span class="sxs-lookup"><span data-stu-id="64f67-114">value</span></span>|<span data-ttu-id="64f67-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="64f67-115">String</span></span>|<span data-ttu-id="64f67-116">Wert für dieses Schlüssel-Wert-Paar</span><span class="sxs-lookup"><span data-stu-id="64f67-116">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="64f67-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="64f67-117">Relationships</span></span>
<span data-ttu-id="64f67-118">Keine</span><span class="sxs-lookup"><span data-stu-id="64f67-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="64f67-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="64f67-119">JSON Representation</span></span>
<span data-ttu-id="64f67-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="64f67-120">Here is a JSON representation of the resource.</span></span>
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




