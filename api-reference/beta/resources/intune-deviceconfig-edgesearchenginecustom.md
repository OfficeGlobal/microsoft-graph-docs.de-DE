---
title: edgeSearchEngineCustom-Ressourcentyp
description: Ermöglicht es IT-Administratoren, eine benutzerdefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c1f97de9b4665769ea4e9731045603664673f64f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165730"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="f8bed-103">edgeSearchEngineCustom-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f8bed-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="f8bed-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f8bed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8bed-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f8bed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8bed-106">Ermöglicht es IT-Administratoren, eine benutzerdefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.</span><span class="sxs-lookup"><span data-stu-id="f8bed-106">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="f8bed-107">Erbt von [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="f8bed-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f8bed-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f8bed-108">Properties</span></span>
|<span data-ttu-id="f8bed-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f8bed-109">Property</span></span>|<span data-ttu-id="f8bed-110">Typ</span><span class="sxs-lookup"><span data-stu-id="f8bed-110">Type</span></span>|<span data-ttu-id="f8bed-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8bed-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8bed-112">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="f8bed-112">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="f8bed-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f8bed-113">String</span></span>|<span data-ttu-id="f8bed-114">Verweist auf einen Https-Link mit der OpenSearch-XML-Datei, die mindestens den Kurznamen und die URL der Suchmaschine enthält.</span><span class="sxs-lookup"><span data-stu-id="f8bed-114">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8bed-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f8bed-115">Relationships</span></span>
<span data-ttu-id="f8bed-116">Keine</span><span class="sxs-lookup"><span data-stu-id="f8bed-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f8bed-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f8bed-117">JSON Representation</span></span>
<span data-ttu-id="f8bed-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f8bed-118">Here is a JSON representation of the resource.</span></span>
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




