---
title: edgeSearchEngineCustom-Ressourcentyp
description: Ermöglicht es IT-Administratoren, eine benutzerdefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.
author: tfitzmac
ms.openlocfilehash: f648f41bafcbaa37c972500139ecc8d3e70113ca
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357974"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="2370a-103">edgeSearchEngineCustom-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2370a-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="2370a-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2370a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2370a-105">Ermöglicht es IT-Administratoren, eine benutzerdefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.</span><span class="sxs-lookup"><span data-stu-id="2370a-105">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="2370a-106">Erbt von [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="2370a-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2370a-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2370a-107">Properties</span></span>
|<span data-ttu-id="2370a-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2370a-108">Property</span></span>|<span data-ttu-id="2370a-109">Typ</span><span class="sxs-lookup"><span data-stu-id="2370a-109">Type</span></span>|<span data-ttu-id="2370a-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2370a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2370a-111">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="2370a-111">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="2370a-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2370a-112">String</span></span>|<span data-ttu-id="2370a-113">Verweist auf einen Https-Link mit der OpenSearch-XML-Datei, die mindestens den Kurznamen und die URL der Suchmaschine enthält.</span><span class="sxs-lookup"><span data-stu-id="2370a-113">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2370a-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2370a-114">Relationships</span></span>
<span data-ttu-id="2370a-115">Keine</span><span class="sxs-lookup"><span data-stu-id="2370a-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2370a-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2370a-116">JSON Representation</span></span>
<span data-ttu-id="2370a-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2370a-117">Here is a JSON representation of the resource.</span></span>
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



