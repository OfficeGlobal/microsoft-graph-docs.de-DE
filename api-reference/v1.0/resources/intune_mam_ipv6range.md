# <a name="ipv6range-resource-type"></a><span data-ttu-id="3f830-101">iPv6Range-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3f830-101">iPv6Range resource type</span></span>

> <span data-ttu-id="3f830-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3f830-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3f830-103">IPV6-Bereich</span><span class="sxs-lookup"><span data-stu-id="3f830-103">IP V6 range</span></span>

<span data-ttu-id="3f830-104">Erbt von [ipRange](../resources/intune_mam_iprange.md)</span><span class="sxs-lookup"><span data-stu-id="3f830-104">Inherits from [ipRange](../resources/intune_mam_iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3f830-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3f830-105">Properties</span></span>
|<span data-ttu-id="3f830-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3f830-106">Property</span></span>|<span data-ttu-id="3f830-107">Typ</span><span class="sxs-lookup"><span data-stu-id="3f830-107">Type</span></span>|<span data-ttu-id="3f830-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3f830-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f830-109">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="3f830-109">lowerAddress</span></span>|<span data-ttu-id="3f830-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3f830-110">String</span></span>|<span data-ttu-id="3f830-111">Untere IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="3f830-111">Lower IP Address</span></span>|
|<span data-ttu-id="3f830-112">upperAddress</span><span class="sxs-lookup"><span data-stu-id="3f830-112">upperAddress</span></span>|<span data-ttu-id="3f830-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3f830-113">String</span></span>|<span data-ttu-id="3f830-114">Obere IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="3f830-114">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f830-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3f830-115">Relationships</span></span>
<span data-ttu-id="3f830-116">Keine</span><span class="sxs-lookup"><span data-stu-id="3f830-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3f830-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3f830-117">JSON Representation</span></span>
<span data-ttu-id="3f830-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3f830-118">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv6Range"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv6Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```








