---
title: edgeSearchEngineCustom-Ressourcentyp
description: Ermöglicht es IT-Administratoren, eine benutzerdefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.
ms.openlocfilehash: 5312f53e43921d71e6c338ccb112a851773abc43
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061202"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="03616-103">edgeSearchEngineCustom-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="03616-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="03616-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="03616-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03616-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="03616-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="03616-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="03616-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="03616-107">Ermöglicht es IT-Administratoren, eine benutzerdefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.</span><span class="sxs-lookup"><span data-stu-id="03616-107">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="03616-108">Erbt von [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="03616-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="03616-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="03616-109">Properties</span></span>
|<span data-ttu-id="03616-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="03616-110">Property</span></span>|<span data-ttu-id="03616-111">Typ</span><span class="sxs-lookup"><span data-stu-id="03616-111">Type</span></span>|<span data-ttu-id="03616-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="03616-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03616-113">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="03616-113">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="03616-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="03616-114">String</span></span>|<span data-ttu-id="03616-115">Verweist auf einen Https-Link mit der OpenSearch-XML-Datei, die mindestens den Kurznamen und die URL der Suchmaschine enthält.</span><span class="sxs-lookup"><span data-stu-id="03616-115">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03616-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="03616-116">Relationships</span></span>
<span data-ttu-id="03616-117">Keine</span><span class="sxs-lookup"><span data-stu-id="03616-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="03616-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="03616-118">JSON Representation</span></span>
<span data-ttu-id="03616-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="03616-119">Here is a JSON representation of the resource.</span></span>
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





