---
title: keyValuePair-Ressourcentyp
description: Schlüssel-Wert-Paar zum Speichern benutzerdefinierter Einstellungen
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f31e83c5e53ea4c2873fd2b425cc0e0c02678ea7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415782"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="0a97e-103">keyValuePair-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0a97e-103">keyValuePair resource type</span></span>

> <span data-ttu-id="0a97e-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="0a97e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0a97e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0a97e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a97e-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0a97e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a97e-107">Schlüssel-Wert-Paar zum Speichern benutzerdefinierter Einstellungen</span><span class="sxs-lookup"><span data-stu-id="0a97e-107">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="0a97e-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0a97e-108">Properties</span></span>
|<span data-ttu-id="0a97e-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0a97e-109">Property</span></span>|<span data-ttu-id="0a97e-110">Typ</span><span class="sxs-lookup"><span data-stu-id="0a97e-110">Type</span></span>|<span data-ttu-id="0a97e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a97e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a97e-112">name</span><span class="sxs-lookup"><span data-stu-id="0a97e-112">name</span></span>|<span data-ttu-id="0a97e-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0a97e-113">String</span></span>|<span data-ttu-id="0a97e-114">Namen für dieses Schlüssel-Wert-Paar</span><span class="sxs-lookup"><span data-stu-id="0a97e-114">Name for this key-value pair</span></span>|
|<span data-ttu-id="0a97e-115">Wert</span><span class="sxs-lookup"><span data-stu-id="0a97e-115">value</span></span>|<span data-ttu-id="0a97e-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0a97e-116">String</span></span>|<span data-ttu-id="0a97e-117">Wert für dieses Schlüssel-Wert-Paar</span><span class="sxs-lookup"><span data-stu-id="0a97e-117">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a97e-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0a97e-118">Relationships</span></span>
<span data-ttu-id="0a97e-119">Keine</span><span class="sxs-lookup"><span data-stu-id="0a97e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0a97e-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0a97e-120">JSON Representation</span></span>
<span data-ttu-id="0a97e-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0a97e-121">Here is a JSON representation of the resource.</span></span>
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




