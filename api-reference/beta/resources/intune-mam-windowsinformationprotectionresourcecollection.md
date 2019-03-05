---
title: windowsInformationProtectionResourceCollection-Ressourcentyp
description: Windows Information Protection – Ressourcensammlung
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cbeb58464ccfd7aff3dfc6066ab276a2bd73f5c6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149749"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="ae79b-103">windowsInformationProtectionResourceCollection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ae79b-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="ae79b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ae79b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae79b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ae79b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae79b-106">Windows Information Protection – Ressourcensammlung</span><span class="sxs-lookup"><span data-stu-id="ae79b-106">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="ae79b-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ae79b-107">Properties</span></span>
|<span data-ttu-id="ae79b-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ae79b-108">Property</span></span>|<span data-ttu-id="ae79b-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ae79b-109">Type</span></span>|<span data-ttu-id="ae79b-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae79b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae79b-111">displayName</span><span class="sxs-lookup"><span data-stu-id="ae79b-111">displayName</span></span>|<span data-ttu-id="ae79b-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ae79b-112">String</span></span>|<span data-ttu-id="ae79b-113">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="ae79b-113">Display name</span></span>|
|<span data-ttu-id="ae79b-114">Ressourcen</span><span class="sxs-lookup"><span data-stu-id="ae79b-114">resources</span></span>|<span data-ttu-id="ae79b-115">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="ae79b-115">String collection</span></span>|<span data-ttu-id="ae79b-116">Sammlung von Ressourcen</span><span class="sxs-lookup"><span data-stu-id="ae79b-116">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae79b-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ae79b-117">Relationships</span></span>
<span data-ttu-id="ae79b-118">Keine</span><span class="sxs-lookup"><span data-stu-id="ae79b-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae79b-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ae79b-119">JSON Representation</span></span>
<span data-ttu-id="ae79b-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ae79b-120">Here is a JSON representation of the resource.</span></span>
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




