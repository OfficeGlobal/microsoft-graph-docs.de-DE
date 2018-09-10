# <a name="resourceaction-resource-type"></a><span data-ttu-id="c2619-101">resourceAction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c2619-101">resourceAction resource type</span></span>

> <span data-ttu-id="c2619-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c2619-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c2619-103">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="c2619-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="c2619-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c2619-104">Properties</span></span>
|<span data-ttu-id="c2619-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c2619-105">Property</span></span>|<span data-ttu-id="c2619-106">Typ</span><span class="sxs-lookup"><span data-stu-id="c2619-106">Type</span></span>|<span data-ttu-id="c2619-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c2619-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2619-108">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="c2619-108">allowedResourceActions</span></span>|<span data-ttu-id="c2619-109">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="c2619-109">String collection</span></span>|<span data-ttu-id="c2619-110">Zulässige Aktionen</span><span class="sxs-lookup"><span data-stu-id="c2619-110">Allowed Actions</span></span>|
|<span data-ttu-id="c2619-111">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="c2619-111">notAllowedResourceActions</span></span>|<span data-ttu-id="c2619-112">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="c2619-112">String collection</span></span>|<span data-ttu-id="c2619-113">Nicht zulässige Aktionen</span><span class="sxs-lookup"><span data-stu-id="c2619-113">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2619-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c2619-114">Relationships</span></span>
<span data-ttu-id="c2619-115">Keine</span><span class="sxs-lookup"><span data-stu-id="c2619-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c2619-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c2619-116">JSON Representation</span></span>
<span data-ttu-id="c2619-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c2619-117">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```








