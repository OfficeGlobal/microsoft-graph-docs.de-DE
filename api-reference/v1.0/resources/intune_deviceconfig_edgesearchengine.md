# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="4ccc6-101">edgeSearchEngine-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4ccc6-101">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="4ccc6-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4ccc6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ccc6-103">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="4ccc6-103">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="4ccc6-104">Erbt von [edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="4ccc6-104">Inherits from [edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4ccc6-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4ccc6-105">Properties</span></span>
|<span data-ttu-id="4ccc6-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4ccc6-106">Property</span></span>|<span data-ttu-id="4ccc6-107">Typ</span><span class="sxs-lookup"><span data-stu-id="4ccc6-107">Type</span></span>|<span data-ttu-id="4ccc6-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4ccc6-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ccc6-109">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="4ccc6-109">edgeSearchEngineType</span></span>|[<span data-ttu-id="4ccc6-110">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="4ccc6-110">edgeSearchEngineType</span></span>](../resources/intune_deviceconfig_edgesearchenginetype.md)|<span data-ttu-id="4ccc6-p101">Ermöglicht es IT-Administratoren, ein vordefiniertes standardmäßiges Suchmodul für MDM-gesteuerte Geräte festzulegen. Mögliche Werte: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="4ccc6-p101">Allows IT admins to set a predefined default search engine for MDM-Controlled devices. The possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ccc6-113">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4ccc6-113">Relationships</span></span>
<span data-ttu-id="4ccc6-114">Keine</span><span class="sxs-lookup"><span data-stu-id="4ccc6-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4ccc6-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4ccc6-115">JSON Representation</span></span>
<span data-ttu-id="4ccc6-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4ccc6-116">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngine"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngine",
  "edgeSearchEngineType": "String"
}
```








