---
title: edgeSearchEngineCustom-Ressourcentyp
description: Ermöglicht es IT-Administratoren, eine benutzerdefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9797b311ae5c4741364a99da0c056c8fb3e18788
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845801"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="f1b78-103">edgeSearchEngineCustom-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f1b78-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="f1b78-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f1b78-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1b78-105">Ermöglicht es IT-Administratoren, eine benutzerdefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.</span><span class="sxs-lookup"><span data-stu-id="f1b78-105">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="f1b78-106">Erbt von [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="f1b78-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f1b78-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f1b78-107">Properties</span></span>
|<span data-ttu-id="f1b78-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f1b78-108">Property</span></span>|<span data-ttu-id="f1b78-109">Typ</span><span class="sxs-lookup"><span data-stu-id="f1b78-109">Type</span></span>|<span data-ttu-id="f1b78-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f1b78-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1b78-111">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="f1b78-111">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="f1b78-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f1b78-112">String</span></span>|<span data-ttu-id="f1b78-113">Verweist auf einen Https-Link mit der OpenSearch-XML-Datei, die mindestens den Kurznamen und die URL der Suchmaschine enthält.</span><span class="sxs-lookup"><span data-stu-id="f1b78-113">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1b78-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f1b78-114">Relationships</span></span>
<span data-ttu-id="f1b78-115">Keine</span><span class="sxs-lookup"><span data-stu-id="f1b78-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f1b78-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f1b78-116">JSON Representation</span></span>
<span data-ttu-id="f1b78-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f1b78-117">Here is a JSON representation of the resource.</span></span>
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



