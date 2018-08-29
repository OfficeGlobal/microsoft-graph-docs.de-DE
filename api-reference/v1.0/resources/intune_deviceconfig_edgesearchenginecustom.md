# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="435a0-101">edgeSearchEngineCustom-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="435a0-101">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="435a0-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="435a0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="435a0-103">Ermöglicht es IT-Administratoren, eine benutzerdefinierte standardmäßige Suchmaschine für MDM-gesteuerte Geräte festzulegen.</span><span class="sxs-lookup"><span data-stu-id="435a0-103">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="435a0-104">Erbt von [edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="435a0-104">Inherits from [edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="435a0-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="435a0-105">Properties</span></span>
|<span data-ttu-id="435a0-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="435a0-106">Property</span></span>|<span data-ttu-id="435a0-107">Typ</span><span class="sxs-lookup"><span data-stu-id="435a0-107">Type</span></span>|<span data-ttu-id="435a0-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="435a0-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="435a0-109">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="435a0-109">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="435a0-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="435a0-110">String</span></span>|<span data-ttu-id="435a0-111">Verweist auf einen Https-Link mit der OpenSearch-XML-Datei, die mindestens den Kurznamen und die URL der Suchmaschine enthält.</span><span class="sxs-lookup"><span data-stu-id="435a0-111">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="435a0-112">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="435a0-112">Relationships</span></span>
<span data-ttu-id="435a0-113">Keine</span><span class="sxs-lookup"><span data-stu-id="435a0-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="435a0-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="435a0-114">JSON Representation</span></span>
<span data-ttu-id="435a0-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="435a0-115">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.edgeSearchEngineBase",
  "@odata.type": "microsoft.graph.edgeSearchEngineCustom"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineCustom",
  "edgeSearchEngineOpenSearchXmlUrl": "String"
}
```



