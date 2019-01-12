---
title: edgeSearchEngineCustom-Ressourcentyp
description: Ermöglicht es IT-Administratoren, eine benutzerdefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8171c293610efc790eadc0619c99fe604d6c933b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932889"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="a7d2c-103">edgeSearchEngineCustom-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a7d2c-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="a7d2c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a7d2c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7d2c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a7d2c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a7d2c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a7d2c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7d2c-107">Ermöglicht es IT-Administratoren, eine benutzerdefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.</span><span class="sxs-lookup"><span data-stu-id="a7d2c-107">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="a7d2c-108">Erbt von [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="a7d2c-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a7d2c-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a7d2c-109">Properties</span></span>
|<span data-ttu-id="a7d2c-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a7d2c-110">Property</span></span>|<span data-ttu-id="a7d2c-111">Typ</span><span class="sxs-lookup"><span data-stu-id="a7d2c-111">Type</span></span>|<span data-ttu-id="a7d2c-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a7d2c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7d2c-113">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="a7d2c-113">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="a7d2c-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a7d2c-114">String</span></span>|<span data-ttu-id="a7d2c-115">Verweist auf einen Https-Link mit der OpenSearch-XML-Datei, die mindestens den Kurznamen und die URL der Suchmaschine enthält.</span><span class="sxs-lookup"><span data-stu-id="a7d2c-115">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7d2c-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a7d2c-116">Relationships</span></span>
<span data-ttu-id="a7d2c-117">Keine</span><span class="sxs-lookup"><span data-stu-id="a7d2c-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a7d2c-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a7d2c-118">JSON Representation</span></span>
<span data-ttu-id="a7d2c-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a7d2c-119">Here is a JSON representation of the resource.</span></span>
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





