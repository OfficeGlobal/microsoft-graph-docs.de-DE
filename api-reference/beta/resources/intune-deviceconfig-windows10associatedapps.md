---
title: windows10AssociatedApps-Ressourcentyp
description: Windows 10-zugeordnete Anwendungsdefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 95f0114bbd39e85c137da2a71b7640ba8051b6dc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146683"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="e9b78-103">windows10AssociatedApps-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e9b78-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="e9b78-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e9b78-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9b78-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e9b78-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9b78-106">Windows 10-zugeordnete Anwendungsdefinition.</span><span class="sxs-lookup"><span data-stu-id="e9b78-106">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="e9b78-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e9b78-107">Properties</span></span>
|<span data-ttu-id="e9b78-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e9b78-108">Property</span></span>|<span data-ttu-id="e9b78-109">Typ</span><span class="sxs-lookup"><span data-stu-id="e9b78-109">Type</span></span>|<span data-ttu-id="e9b78-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e9b78-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9b78-111">appType</span><span class="sxs-lookup"><span data-stu-id="e9b78-111">appType</span></span>|[<span data-ttu-id="e9b78-112">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="e9b78-112">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="e9b78-113">Anwendungstyp.</span><span class="sxs-lookup"><span data-stu-id="e9b78-113">Application type.</span></span> <span data-ttu-id="e9b78-114">Mögliche Werte sind: `desktop` und `universal`.</span><span class="sxs-lookup"><span data-stu-id="e9b78-114">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="e9b78-115">Bezeichner</span><span class="sxs-lookup"><span data-stu-id="e9b78-115">identifier</span></span>|<span data-ttu-id="e9b78-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e9b78-116">String</span></span>|<span data-ttu-id="e9b78-117">Bezeichner.</span><span class="sxs-lookup"><span data-stu-id="e9b78-117">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9b78-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e9b78-118">Relationships</span></span>
<span data-ttu-id="e9b78-119">Keine</span><span class="sxs-lookup"><span data-stu-id="e9b78-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9b78-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e9b78-120">JSON Representation</span></span>
<span data-ttu-id="e9b78-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e9b78-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AssociatedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AssociatedApps",
  "appType": "String",
  "identifier": "String"
}
```




