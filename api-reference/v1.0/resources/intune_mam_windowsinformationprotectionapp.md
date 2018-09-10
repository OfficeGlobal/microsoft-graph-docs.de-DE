# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="7fc12-101">windowsInformationProtectionApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7fc12-101">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="7fc12-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7fc12-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7fc12-103">App für Windows-Informationsschutz</span><span class="sxs-lookup"><span data-stu-id="7fc12-103">App for Windows information protection</span></span>
## <a name="properties"></a><span data-ttu-id="7fc12-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7fc12-104">Properties</span></span>
|<span data-ttu-id="7fc12-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7fc12-105">Property</span></span>|<span data-ttu-id="7fc12-106">Typ</span><span class="sxs-lookup"><span data-stu-id="7fc12-106">Type</span></span>|<span data-ttu-id="7fc12-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7fc12-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fc12-108">displayName</span><span class="sxs-lookup"><span data-stu-id="7fc12-108">displayName</span></span>|<span data-ttu-id="7fc12-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7fc12-109">String</span></span>|<span data-ttu-id="7fc12-110">Anzeigename der App</span><span class="sxs-lookup"><span data-stu-id="7fc12-110">App display name.</span></span>|
|<span data-ttu-id="7fc12-111">description</span><span class="sxs-lookup"><span data-stu-id="7fc12-111">description</span></span>|<span data-ttu-id="7fc12-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7fc12-112">String</span></span>|<span data-ttu-id="7fc12-113">Beschreibung der App</span><span class="sxs-lookup"><span data-stu-id="7fc12-113">The app's description.</span></span>|
|<span data-ttu-id="7fc12-114">publisherName</span><span class="sxs-lookup"><span data-stu-id="7fc12-114">publisherName</span></span>|<span data-ttu-id="7fc12-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7fc12-115">String</span></span>|<span data-ttu-id="7fc12-116">Name des Verlegers</span><span class="sxs-lookup"><span data-stu-id="7fc12-116">The publisher name</span></span>|
|<span data-ttu-id="7fc12-117">productName</span><span class="sxs-lookup"><span data-stu-id="7fc12-117">productName</span></span>|<span data-ttu-id="7fc12-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7fc12-118">String</span></span>|<span data-ttu-id="7fc12-119">Produktname</span><span class="sxs-lookup"><span data-stu-id="7fc12-119">The product name.</span></span>|
|<span data-ttu-id="7fc12-120">denied</span><span class="sxs-lookup"><span data-stu-id="7fc12-120">denied</span></span>|<span data-ttu-id="7fc12-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="7fc12-121">Boolean</span></span>|<span data-ttu-id="7fc12-122">Bei „true“ wird der App der Schutz oder eine Ausnahme verweigert.</span><span class="sxs-lookup"><span data-stu-id="7fc12-122">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7fc12-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7fc12-123">Relationships</span></span>
<span data-ttu-id="7fc12-124">Keine</span><span class="sxs-lookup"><span data-stu-id="7fc12-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7fc12-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7fc12-125">JSON Representation</span></span>
<span data-ttu-id="7fc12-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7fc12-126">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```








