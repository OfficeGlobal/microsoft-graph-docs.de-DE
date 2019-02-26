---
title: edgeSearchEngineCustom-Ressourcentyp
description: Ermöglicht es IT-Administratoren, eine benutzerdefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 523a2de33619886997cbcb052079bbf2937c9d48
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263581"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="acfd9-103">edgeSearchEngineCustom-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="acfd9-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="acfd9-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="acfd9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="acfd9-105">Ermöglicht es IT-Administratoren, eine benutzerdefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.</span><span class="sxs-lookup"><span data-stu-id="acfd9-105">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="acfd9-106">Erbt von [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="acfd9-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="acfd9-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="acfd9-107">Properties</span></span>
|<span data-ttu-id="acfd9-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="acfd9-108">Property</span></span>|<span data-ttu-id="acfd9-109">Typ</span><span class="sxs-lookup"><span data-stu-id="acfd9-109">Type</span></span>|<span data-ttu-id="acfd9-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="acfd9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acfd9-111">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="acfd9-111">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="acfd9-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="acfd9-112">String</span></span>|<span data-ttu-id="acfd9-113">Verweist auf einen Https-Link mit der OpenSearch-XML-Datei, die mindestens den Kurznamen und die URL der Suchmaschine enthält.</span><span class="sxs-lookup"><span data-stu-id="acfd9-113">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="acfd9-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="acfd9-114">Relationships</span></span>
<span data-ttu-id="acfd9-115">Keine</span><span class="sxs-lookup"><span data-stu-id="acfd9-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="acfd9-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="acfd9-116">JSON Representation</span></span>
<span data-ttu-id="acfd9-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="acfd9-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngineCustom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineCustom",
  "edgeSearchEngineOpenSearchXmlUrl": "String"
}
```



