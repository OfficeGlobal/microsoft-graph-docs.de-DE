# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="3d8f7-101">windowsInformationProtectionApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3d8f7-101">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="3d8f7-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3d8f7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3d8f7-103">App für Windows-Informationsschutz</span><span class="sxs-lookup"><span data-stu-id="3d8f7-103">App for Windows information protection</span></span>
## <a name="properties"></a><span data-ttu-id="3d8f7-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3d8f7-104">Properties</span></span>
|<span data-ttu-id="3d8f7-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3d8f7-105">Property</span></span>|<span data-ttu-id="3d8f7-106">Typ</span><span class="sxs-lookup"><span data-stu-id="3d8f7-106">Type</span></span>|<span data-ttu-id="3d8f7-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3d8f7-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d8f7-108">displayName</span><span class="sxs-lookup"><span data-stu-id="3d8f7-108">displayName</span></span>|<span data-ttu-id="3d8f7-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3d8f7-109">String</span></span>|<span data-ttu-id="3d8f7-110">Anzeigename der App</span><span class="sxs-lookup"><span data-stu-id="3d8f7-110">App display name.</span></span>|
|<span data-ttu-id="3d8f7-111">description</span><span class="sxs-lookup"><span data-stu-id="3d8f7-111">description</span></span>|<span data-ttu-id="3d8f7-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3d8f7-112">String</span></span>|<span data-ttu-id="3d8f7-113">Beschreibung der App</span><span class="sxs-lookup"><span data-stu-id="3d8f7-113">The app's description.</span></span>|
|<span data-ttu-id="3d8f7-114">publisherName</span><span class="sxs-lookup"><span data-stu-id="3d8f7-114">publisherName</span></span>|<span data-ttu-id="3d8f7-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3d8f7-115">String</span></span>|<span data-ttu-id="3d8f7-116">Name des Verlegers</span><span class="sxs-lookup"><span data-stu-id="3d8f7-116">The publisher name</span></span>|
|<span data-ttu-id="3d8f7-117">productName</span><span class="sxs-lookup"><span data-stu-id="3d8f7-117">productName</span></span>|<span data-ttu-id="3d8f7-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3d8f7-118">String</span></span>|<span data-ttu-id="3d8f7-119">Produktname</span><span class="sxs-lookup"><span data-stu-id="3d8f7-119">The product name.</span></span>|
|<span data-ttu-id="3d8f7-120">denied</span><span class="sxs-lookup"><span data-stu-id="3d8f7-120">Permission denied</span></span>|<span data-ttu-id="3d8f7-121">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3d8f7-121">Boolean</span></span>|<span data-ttu-id="3d8f7-122">Bei „true“ wird der App der Schutz oder eine Ausnahme verweigert.</span><span class="sxs-lookup"><span data-stu-id="3d8f7-122">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d8f7-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3d8f7-123">Relationships</span></span>
<span data-ttu-id="3d8f7-124">Keine</span><span class="sxs-lookup"><span data-stu-id="3d8f7-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3d8f7-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3d8f7-125">JSON Representation</span></span>
<span data-ttu-id="3d8f7-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3d8f7-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionApp"
}
-->
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



