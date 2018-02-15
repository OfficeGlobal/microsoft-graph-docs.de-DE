# <a name="windowsminimumoperatingsystem-resource-type"></a><span data-ttu-id="b8eee-101">windowsMinimumOperatingSystem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b8eee-101">windowsMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="b8eee-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b8eee-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8eee-103">Das mindestens für eine mobile Windows-App erforderliche Betriebssystem.</span><span class="sxs-lookup"><span data-stu-id="b8eee-103">The minimum operating system required for a Windows mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="b8eee-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b8eee-104">Properties</span></span>
|<span data-ttu-id="b8eee-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b8eee-105">Property</span></span>|<span data-ttu-id="b8eee-106">Typ</span><span class="sxs-lookup"><span data-stu-id="b8eee-106">Type</span></span>|<span data-ttu-id="b8eee-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8eee-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8eee-108">v8_0</span><span class="sxs-lookup"><span data-stu-id="b8eee-108">v8_0</span></span>|<span data-ttu-id="b8eee-109">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8eee-109">Boolean</span></span>|<span data-ttu-id="b8eee-110">Windows-Version 8.0 oder höher</span><span class="sxs-lookup"><span data-stu-id="b8eee-110">Windows version 8.0 or later.</span></span>|
|<span data-ttu-id="b8eee-111">v8_1</span><span class="sxs-lookup"><span data-stu-id="b8eee-111">v8_1</span></span>|<span data-ttu-id="b8eee-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8eee-112">Boolean</span></span>|<span data-ttu-id="b8eee-113">Windows-Version 8.1 oder höher</span><span class="sxs-lookup"><span data-stu-id="b8eee-113">Windows version 8.1 or later.</span></span>|
|<span data-ttu-id="b8eee-114">v10_0</span><span class="sxs-lookup"><span data-stu-id="b8eee-114">v10_0</span></span>|<span data-ttu-id="b8eee-115">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8eee-115">Boolean</span></span>|<span data-ttu-id="b8eee-116">Windows-Version 10.0 oder höher</span><span class="sxs-lookup"><span data-stu-id="b8eee-116">Windows version 10.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8eee-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b8eee-117">Relationships</span></span>
<span data-ttu-id="b8eee-118">Keine</span><span class="sxs-lookup"><span data-stu-id="b8eee-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b8eee-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b8eee-119">JSON Representation</span></span>
<span data-ttu-id="b8eee-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b8eee-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMinimumOperatingSystem",
  "v8_0": true,
  "v8_1": true,
  "v10_0": true
}
```



