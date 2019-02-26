---
title: edgeHomeButtonOpensCustomURL-Ressourcentyp
description: Schaltfläche "Start" anzeigen; beim Klicken auf die Schaltfläche "Startseite" wird eine bestimmte URL geladen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e83fd3dbb0961011584ef9d65e01c361ccf6a228
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143239"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="07273-103">edgeHomeButtonOpensCustomURL-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="07273-103">edgeHomeButtonOpensCustomURL resource type</span></span>

> <span data-ttu-id="07273-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="07273-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07273-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="07273-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07273-106">Schaltfläche "Start" anzeigen; beim Klicken auf die Schaltfläche "Startseite" wird eine bestimmte URL geladen.</span><span class="sxs-lookup"><span data-stu-id="07273-106">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="07273-107">Erbt von [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="07273-107">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="07273-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="07273-108">Properties</span></span>
|<span data-ttu-id="07273-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="07273-109">Property</span></span>|<span data-ttu-id="07273-110">Typ</span><span class="sxs-lookup"><span data-stu-id="07273-110">Type</span></span>|<span data-ttu-id="07273-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07273-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07273-112">homeButtonCustomURL</span><span class="sxs-lookup"><span data-stu-id="07273-112">homeButtonCustomURL</span></span>|<span data-ttu-id="07273-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="07273-113">String</span></span>|<span data-ttu-id="07273-114">Die zu ladende URL.</span><span class="sxs-lookup"><span data-stu-id="07273-114">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07273-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="07273-115">Relationships</span></span>
<span data-ttu-id="07273-116">Keine</span><span class="sxs-lookup"><span data-stu-id="07273-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07273-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="07273-117">JSON Representation</span></span>
<span data-ttu-id="07273-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="07273-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeHomeButtonOpensCustomURL"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeHomeButtonOpensCustomURL",
  "homeButtonCustomURL": "String"
}
```




