---
title: windowsInformationProtectionResourceCollection-Ressourcentyp
description: Windows Information Protection – Ressourcensammlung
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c4a8ad51177507613c3fd84b524503d0e79c208f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424679"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="fc19a-103">windowsInformationProtectionResourceCollection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fc19a-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="fc19a-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="fc19a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fc19a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fc19a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fc19a-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fc19a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc19a-107">Windows Information Protection – Ressourcensammlung</span><span class="sxs-lookup"><span data-stu-id="fc19a-107">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="fc19a-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fc19a-108">Properties</span></span>
|<span data-ttu-id="fc19a-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fc19a-109">Property</span></span>|<span data-ttu-id="fc19a-110">Typ</span><span class="sxs-lookup"><span data-stu-id="fc19a-110">Type</span></span>|<span data-ttu-id="fc19a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc19a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc19a-112">displayName</span><span class="sxs-lookup"><span data-stu-id="fc19a-112">displayName</span></span>|<span data-ttu-id="fc19a-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fc19a-113">String</span></span>|<span data-ttu-id="fc19a-114">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="fc19a-114">Display name</span></span>|
|<span data-ttu-id="fc19a-115">Ressourcen</span><span class="sxs-lookup"><span data-stu-id="fc19a-115">resources</span></span>|<span data-ttu-id="fc19a-116">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="fc19a-116">String collection</span></span>|<span data-ttu-id="fc19a-117">Sammlung von Ressourcen</span><span class="sxs-lookup"><span data-stu-id="fc19a-117">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc19a-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fc19a-118">Relationships</span></span>
<span data-ttu-id="fc19a-119">Keine</span><span class="sxs-lookup"><span data-stu-id="fc19a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc19a-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fc19a-120">JSON Representation</span></span>
<span data-ttu-id="fc19a-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fc19a-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionResourceCollection",
  "displayName": "String",
  "resources": [
    "String"
  ]
}
```




