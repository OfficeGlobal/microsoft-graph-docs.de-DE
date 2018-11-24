# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="b91b5-101">windowsInformationProtectionIPRangeCollection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b91b5-101">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="b91b5-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b91b5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b91b5-103">Windows Information Protection – IP-Bereichssammlung</span><span class="sxs-lookup"><span data-stu-id="b91b5-103">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="b91b5-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b91b5-104">Properties</span></span>
|<span data-ttu-id="b91b5-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b91b5-105">Property</span></span>|<span data-ttu-id="b91b5-106">Typ</span><span class="sxs-lookup"><span data-stu-id="b91b5-106">Type</span></span>|<span data-ttu-id="b91b5-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b91b5-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b91b5-108">displayName</span><span class="sxs-lookup"><span data-stu-id="b91b5-108">displayName</span></span>|<span data-ttu-id="b91b5-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b91b5-109">String</span></span>|<span data-ttu-id="b91b5-110">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="b91b5-110">Display name</span></span>|
|<span data-ttu-id="b91b5-111">ranges</span><span class="sxs-lookup"><span data-stu-id="b91b5-111">ranges</span></span>|<span data-ttu-id="b91b5-112">[ipRange](../resources/intune_mam_iprange.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b91b5-112">[ipRange](../resources/intune_mam_iprange.md) collection</span></span>|<span data-ttu-id="b91b5-113">Sammlung der IP-Bereiche</span><span class="sxs-lookup"><span data-stu-id="b91b5-113">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="b91b5-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b91b5-114">Relationships</span></span>
<span data-ttu-id="b91b5-115">Keine</span><span class="sxs-lookup"><span data-stu-id="b91b5-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b91b5-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b91b5-116">JSON Representation</span></span>
<span data-ttu-id="b91b5-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b91b5-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionIPRangeCollection",
  "displayName": "String",
  "ranges": [
    {
      "@odata.type": "microsoft.graph.ipRange",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ]
}
```



