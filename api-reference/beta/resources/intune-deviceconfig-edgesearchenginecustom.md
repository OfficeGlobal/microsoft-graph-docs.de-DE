---
title: edgeSearchEngineCustom-Ressourcentyp
description: Ermöglicht es IT-Administratoren, eine benutzerdefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 69395d09c01c1b92f2ae3ee1abf26eeff09618f8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425981"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="56b21-103">edgeSearchEngineCustom-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="56b21-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="56b21-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="56b21-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="56b21-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="56b21-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="56b21-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="56b21-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56b21-107">Ermöglicht es IT-Administratoren, eine benutzerdefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.</span><span class="sxs-lookup"><span data-stu-id="56b21-107">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="56b21-108">Erbt von [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="56b21-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="56b21-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="56b21-109">Properties</span></span>
|<span data-ttu-id="56b21-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="56b21-110">Property</span></span>|<span data-ttu-id="56b21-111">Typ</span><span class="sxs-lookup"><span data-stu-id="56b21-111">Type</span></span>|<span data-ttu-id="56b21-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="56b21-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56b21-113">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="56b21-113">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="56b21-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="56b21-114">String</span></span>|<span data-ttu-id="56b21-115">Verweist auf einen Https-Link mit der OpenSearch-XML-Datei, die mindestens den Kurznamen und die URL der Suchmaschine enthält.</span><span class="sxs-lookup"><span data-stu-id="56b21-115">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56b21-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="56b21-116">Relationships</span></span>
<span data-ttu-id="56b21-117">Keine</span><span class="sxs-lookup"><span data-stu-id="56b21-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56b21-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="56b21-118">JSON Representation</span></span>
<span data-ttu-id="56b21-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="56b21-119">Here is a JSON representation of the resource.</span></span>
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




