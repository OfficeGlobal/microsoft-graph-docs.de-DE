# <a name="applistitem-resource-type"></a><span data-ttu-id="03a6e-101">appListItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="03a6e-101">appListItem resource type</span></span>

> <span data-ttu-id="03a6e-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="03a6e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="03a6e-103">Stellt eine App in der Liste der verwalteten Anwendungen dar.</span><span class="sxs-lookup"><span data-stu-id="03a6e-103">Represents an app in the list of managed applications</span></span>
## <a name="properties"></a><span data-ttu-id="03a6e-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="03a6e-104">Properties</span></span>
|<span data-ttu-id="03a6e-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="03a6e-105">Property</span></span>|<span data-ttu-id="03a6e-106">Typ</span><span class="sxs-lookup"><span data-stu-id="03a6e-106">Type</span></span>|<span data-ttu-id="03a6e-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="03a6e-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03a6e-108">name</span><span class="sxs-lookup"><span data-stu-id="03a6e-108">name</span></span>|<span data-ttu-id="03a6e-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="03a6e-109">String</span></span>|<span data-ttu-id="03a6e-110">Anwendungsname</span><span class="sxs-lookup"><span data-stu-id="03a6e-110">The application name</span></span>|
|<span data-ttu-id="03a6e-111">publisher</span><span class="sxs-lookup"><span data-stu-id="03a6e-111">publisher</span></span>|<span data-ttu-id="03a6e-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="03a6e-112">String</span></span>|<span data-ttu-id="03a6e-113">Herausgeber der App</span><span class="sxs-lookup"><span data-stu-id="03a6e-113">The publisher of the application</span></span>|
|<span data-ttu-id="03a6e-114">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="03a6e-114">appStoreUrl</span></span>|<span data-ttu-id="03a6e-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="03a6e-115">String</span></span>|<span data-ttu-id="03a6e-116">Store-URL der Anwendung</span><span class="sxs-lookup"><span data-stu-id="03a6e-116">The Store URL of the application</span></span>|
|<span data-ttu-id="03a6e-117">appId</span><span class="sxs-lookup"><span data-stu-id="03a6e-117">appId</span></span>|<span data-ttu-id="03a6e-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="03a6e-118">String</span></span>|<span data-ttu-id="03a6e-119">Anwendungs- oder Paket-ID der Anwendung</span><span class="sxs-lookup"><span data-stu-id="03a6e-119">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="03a6e-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="03a6e-120">Relationships</span></span>
<span data-ttu-id="03a6e-121">Keine</span><span class="sxs-lookup"><span data-stu-id="03a6e-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="03a6e-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="03a6e-122">JSON Representation</span></span>
<span data-ttu-id="03a6e-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="03a6e-123">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appListItem"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```



