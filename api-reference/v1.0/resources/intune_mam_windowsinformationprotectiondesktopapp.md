# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="06cc5-101">windowsInformationProtectionDesktopApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="06cc5-101">windowsInformationProtectionDesktopApp resource type</span></span>

> <span data-ttu-id="06cc5-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="06cc5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06cc5-103">Desktop-App für Windows-Informationsschutz</span><span class="sxs-lookup"><span data-stu-id="06cc5-103">Desktop App for Windows information protection</span></span>

<span data-ttu-id="06cc5-104">Erbt von [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="06cc5-104">Inherits from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="06cc5-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="06cc5-105">Properties</span></span>
|<span data-ttu-id="06cc5-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="06cc5-106">Property</span></span>|<span data-ttu-id="06cc5-107">Typ</span><span class="sxs-lookup"><span data-stu-id="06cc5-107">Type</span></span>|<span data-ttu-id="06cc5-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06cc5-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06cc5-109">displayName</span><span class="sxs-lookup"><span data-stu-id="06cc5-109">displayName</span></span>|<span data-ttu-id="06cc5-110">String</span><span class="sxs-lookup"><span data-stu-id="06cc5-110">String</span></span>|<span data-ttu-id="06cc5-111">Anzeigename der App.</span><span class="sxs-lookup"><span data-stu-id="06cc5-111">App display name.</span></span> <span data-ttu-id="06cc5-112">Geerbt von [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="06cc5-112">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="06cc5-113">description</span><span class="sxs-lookup"><span data-stu-id="06cc5-113">description</span></span>|<span data-ttu-id="06cc5-114">String</span><span class="sxs-lookup"><span data-stu-id="06cc5-114">String</span></span>|<span data-ttu-id="06cc5-115">Die Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="06cc5-115">The app's description.</span></span> <span data-ttu-id="06cc5-116">Geerbt von [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="06cc5-116">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="06cc5-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="06cc5-117">publisherName</span></span>|<span data-ttu-id="06cc5-118">String</span><span class="sxs-lookup"><span data-stu-id="06cc5-118">String</span></span>|<span data-ttu-id="06cc5-119">Der Name des Herausgebers, geerbt von [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="06cc5-119">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="06cc5-120">productName</span><span class="sxs-lookup"><span data-stu-id="06cc5-120">productName</span></span>|<span data-ttu-id="06cc5-121">String</span><span class="sxs-lookup"><span data-stu-id="06cc5-121">String</span></span>|<span data-ttu-id="06cc5-122">Der Produktname.</span><span class="sxs-lookup"><span data-stu-id="06cc5-122">The product name.</span></span> <span data-ttu-id="06cc5-123">Geerbt von [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="06cc5-123">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="06cc5-124">denied</span><span class="sxs-lookup"><span data-stu-id="06cc5-124">denied</span></span>|<span data-ttu-id="06cc5-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="06cc5-125">Boolean</span></span>|<span data-ttu-id="06cc5-126">Bei „true“ wird der App der Schutz oder eine Ausnahme verweigert.</span><span class="sxs-lookup"><span data-stu-id="06cc5-126">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="06cc5-127">Geerbt von [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="06cc5-127">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="06cc5-128">binaryName</span><span class="sxs-lookup"><span data-stu-id="06cc5-128">binaryName</span></span>|<span data-ttu-id="06cc5-129">String</span><span class="sxs-lookup"><span data-stu-id="06cc5-129">String</span></span>|<span data-ttu-id="06cc5-130">Der binäre Name</span><span class="sxs-lookup"><span data-stu-id="06cc5-130">The binary name.</span></span>|
|<span data-ttu-id="06cc5-131">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="06cc5-131">binaryVersionLow</span></span>|<span data-ttu-id="06cc5-132">String</span><span class="sxs-lookup"><span data-stu-id="06cc5-132">String</span></span>|<span data-ttu-id="06cc5-133">Die niedrigere Binärversion.</span><span class="sxs-lookup"><span data-stu-id="06cc5-133">The lower binary version.</span></span>|
|<span data-ttu-id="06cc5-134">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="06cc5-134">binaryVersionHigh</span></span>|<span data-ttu-id="06cc5-135">String</span><span class="sxs-lookup"><span data-stu-id="06cc5-135">String</span></span>|<span data-ttu-id="06cc5-136">Die größte Binärversion.</span><span class="sxs-lookup"><span data-stu-id="06cc5-136">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06cc5-137">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="06cc5-137">Relationships</span></span>
<span data-ttu-id="06cc5-138">Keine</span><span class="sxs-lookup"><span data-stu-id="06cc5-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="06cc5-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="06cc5-139">JSON Representation</span></span>
<span data-ttu-id="06cc5-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="06cc5-140">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.windowsInformationProtectionApp",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDesktopApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDesktopApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true,
  "binaryName": "String",
  "binaryVersionLow": "String",
  "binaryVersionHigh": "String"
}
```



