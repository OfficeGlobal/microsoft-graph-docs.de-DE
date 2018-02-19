# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="5fe70-101">windowsInformationProtectionDesktopApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5fe70-101">windowsInformationProtectionDesktopApp resource type</span></span>

> <span data-ttu-id="5fe70-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5fe70-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5fe70-103">Desktop-App für Windows-Informationsschutz</span><span class="sxs-lookup"><span data-stu-id="5fe70-103">Desktop App for Windows information protection</span></span>

<span data-ttu-id="5fe70-104">Erbt von [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="5fe70-104">Inherits from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5fe70-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5fe70-105">Properties</span></span>
|<span data-ttu-id="5fe70-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5fe70-106">Property</span></span>|<span data-ttu-id="5fe70-107">Typ</span><span class="sxs-lookup"><span data-stu-id="5fe70-107">Type</span></span>|<span data-ttu-id="5fe70-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5fe70-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fe70-109">displayName</span><span class="sxs-lookup"><span data-stu-id="5fe70-109">displayName</span></span>|<span data-ttu-id="5fe70-110">String</span><span class="sxs-lookup"><span data-stu-id="5fe70-110">String</span></span>|<span data-ttu-id="5fe70-111">Anzeigename der App.</span><span class="sxs-lookup"><span data-stu-id="5fe70-111">App display name.</span></span> <span data-ttu-id="5fe70-112">Geerbt von [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="5fe70-112">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="5fe70-113">description</span><span class="sxs-lookup"><span data-stu-id="5fe70-113">description</span></span>|<span data-ttu-id="5fe70-114">String</span><span class="sxs-lookup"><span data-stu-id="5fe70-114">String</span></span>|<span data-ttu-id="5fe70-115">Die Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="5fe70-115">The app's description.</span></span> <span data-ttu-id="5fe70-116">Geerbt von [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="5fe70-116">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="5fe70-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="5fe70-117">publisherName</span></span>|<span data-ttu-id="5fe70-118">String</span><span class="sxs-lookup"><span data-stu-id="5fe70-118">String</span></span>|<span data-ttu-id="5fe70-119">Der Name des Herausgebers, geerbt von [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="5fe70-119">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="5fe70-120">productName</span><span class="sxs-lookup"><span data-stu-id="5fe70-120">productName</span></span>|<span data-ttu-id="5fe70-121">String</span><span class="sxs-lookup"><span data-stu-id="5fe70-121">String</span></span>|<span data-ttu-id="5fe70-122">Der Produktname.</span><span class="sxs-lookup"><span data-stu-id="5fe70-122">The product name.</span></span> <span data-ttu-id="5fe70-123">Geerbt von [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="5fe70-123">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="5fe70-124">denied</span><span class="sxs-lookup"><span data-stu-id="5fe70-124">Permission denied</span></span>|<span data-ttu-id="5fe70-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fe70-125">Boolean</span></span>|<span data-ttu-id="5fe70-126">Bei „true“ wird der App der Schutz oder eine Ausnahme verweigert.</span><span class="sxs-lookup"><span data-stu-id="5fe70-126">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="5fe70-127">Geerbt von [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="5fe70-127">Inherited from [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="5fe70-128">binaryName</span><span class="sxs-lookup"><span data-stu-id="5fe70-128">binaryName</span></span>|<span data-ttu-id="5fe70-129">String</span><span class="sxs-lookup"><span data-stu-id="5fe70-129">String</span></span>|<span data-ttu-id="5fe70-130">Der binäre Name</span><span class="sxs-lookup"><span data-stu-id="5fe70-130">The binary name.</span></span>|
|<span data-ttu-id="5fe70-131">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="5fe70-131">binaryVersionLow</span></span>|<span data-ttu-id="5fe70-132">String</span><span class="sxs-lookup"><span data-stu-id="5fe70-132">String</span></span>|<span data-ttu-id="5fe70-133">Die niedrigere Binärversion.</span><span class="sxs-lookup"><span data-stu-id="5fe70-133">The lower binary version.</span></span>|
|<span data-ttu-id="5fe70-134">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="5fe70-134">binaryVersionHigh</span></span>|<span data-ttu-id="5fe70-135">String</span><span class="sxs-lookup"><span data-stu-id="5fe70-135">String</span></span>|<span data-ttu-id="5fe70-136">Die größte Binärversion.</span><span class="sxs-lookup"><span data-stu-id="5fe70-136">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5fe70-137">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5fe70-137">Relationships</span></span>
<span data-ttu-id="5fe70-138">Keine</span><span class="sxs-lookup"><span data-stu-id="5fe70-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5fe70-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5fe70-139">JSON Representation</span></span>
<span data-ttu-id="5fe70-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5fe70-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDesktopApp"
}
-->
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



