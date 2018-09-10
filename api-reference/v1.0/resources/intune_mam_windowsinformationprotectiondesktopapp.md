# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="14ee2-101">windowsInformationProtectionDesktopApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="14ee2-101">windowsInformationProtectionDesktopApp resource type</span></span>

> <span data-ttu-id="14ee2-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="14ee2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="14ee2-103">Desktop-App für Windows-Informationsschutz</span><span class="sxs-lookup"><span data-stu-id="14ee2-103">Desktop App for Windows information protection</span></span>

<span data-ttu-id="14ee2-104">Erbt von [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="14ee2-104">Inherits from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="14ee2-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="14ee2-105">Properties</span></span>
|<span data-ttu-id="14ee2-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="14ee2-106">Property</span></span>|<span data-ttu-id="14ee2-107">Typ</span><span class="sxs-lookup"><span data-stu-id="14ee2-107">Type</span></span>|<span data-ttu-id="14ee2-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="14ee2-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14ee2-109">displayName</span><span class="sxs-lookup"><span data-stu-id="14ee2-109">displayName</span></span>|<span data-ttu-id="14ee2-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="14ee2-110">String</span></span>|<span data-ttu-id="14ee2-111">Anzeigename der App.</span><span class="sxs-lookup"><span data-stu-id="14ee2-111">App display name.</span></span> <span data-ttu-id="14ee2-112">Geerbt von [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="14ee2-112">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="14ee2-113">description</span><span class="sxs-lookup"><span data-stu-id="14ee2-113">description</span></span>|<span data-ttu-id="14ee2-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="14ee2-114">String</span></span>|<span data-ttu-id="14ee2-115">Die Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="14ee2-115">The app's description.</span></span> <span data-ttu-id="14ee2-116">Geerbt von [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="14ee2-116">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="14ee2-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="14ee2-117">publisherName</span></span>|<span data-ttu-id="14ee2-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="14ee2-118">String</span></span>|<span data-ttu-id="14ee2-119">Der Name des Herausgebers, geerbt von [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="14ee2-119">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="14ee2-120">productName</span><span class="sxs-lookup"><span data-stu-id="14ee2-120">productName</span></span>|<span data-ttu-id="14ee2-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="14ee2-121">String</span></span>|<span data-ttu-id="14ee2-122">Der Produktname.</span><span class="sxs-lookup"><span data-stu-id="14ee2-122">The product name.</span></span> <span data-ttu-id="14ee2-123">Geerbt von [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="14ee2-123">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="14ee2-124">denied</span><span class="sxs-lookup"><span data-stu-id="14ee2-124">denied</span></span>|<span data-ttu-id="14ee2-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="14ee2-125">Boolean</span></span>|<span data-ttu-id="14ee2-126">Bei „true“ wird der App der Schutz oder eine Ausnahme verweigert.</span><span class="sxs-lookup"><span data-stu-id="14ee2-126">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="14ee2-127">Geerbt von [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="14ee2-127">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="14ee2-128">binaryName</span><span class="sxs-lookup"><span data-stu-id="14ee2-128">binaryName</span></span>|<span data-ttu-id="14ee2-129">String</span><span class="sxs-lookup"><span data-stu-id="14ee2-129">String</span></span>|<span data-ttu-id="14ee2-130">Der binäre Name</span><span class="sxs-lookup"><span data-stu-id="14ee2-130">The binary name.</span></span>|
|<span data-ttu-id="14ee2-131">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="14ee2-131">binaryVersionLow</span></span>|<span data-ttu-id="14ee2-132">String</span><span class="sxs-lookup"><span data-stu-id="14ee2-132">String</span></span>|<span data-ttu-id="14ee2-133">Die niedrigere Binärversion.</span><span class="sxs-lookup"><span data-stu-id="14ee2-133">The lower binary version.</span></span>|
|<span data-ttu-id="14ee2-134">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="14ee2-134">binaryVersionHigh</span></span>|<span data-ttu-id="14ee2-135">String</span><span class="sxs-lookup"><span data-stu-id="14ee2-135">String</span></span>|<span data-ttu-id="14ee2-136">Die größte Binärversion.</span><span class="sxs-lookup"><span data-stu-id="14ee2-136">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14ee2-137">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="14ee2-137">Relationships</span></span>
<span data-ttu-id="14ee2-138">Keine</span><span class="sxs-lookup"><span data-stu-id="14ee2-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="14ee2-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="14ee2-139">JSON Representation</span></span>
<span data-ttu-id="14ee2-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="14ee2-140">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
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








