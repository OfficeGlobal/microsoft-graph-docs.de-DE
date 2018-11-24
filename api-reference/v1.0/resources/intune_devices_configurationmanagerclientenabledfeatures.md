# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="21f01-101">configurationManagerClientEnabledFeatures-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="21f01-101">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="21f01-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="21f01-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21f01-103">Im Konfigurations-Manager-Client aktivierte Features</span><span class="sxs-lookup"><span data-stu-id="21f01-103">configuration Manager client enabled features</span></span>
## <a name="properties"></a><span data-ttu-id="21f01-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="21f01-104">Properties</span></span>
|<span data-ttu-id="21f01-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="21f01-105">Property</span></span>|<span data-ttu-id="21f01-106">Typ</span><span class="sxs-lookup"><span data-stu-id="21f01-106">Type</span></span>|<span data-ttu-id="21f01-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="21f01-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21f01-108">inventory</span><span class="sxs-lookup"><span data-stu-id="21f01-108">inventory</span></span>|<span data-ttu-id="21f01-109">Boolean</span><span class="sxs-lookup"><span data-stu-id="21f01-109">Boolean</span></span>|<span data-ttu-id="21f01-110">Gibt an, ob der Bestand von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="21f01-110">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="21f01-111">modernApps</span><span class="sxs-lookup"><span data-stu-id="21f01-111">modernApps</span></span>|<span data-ttu-id="21f01-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="21f01-112">Boolean</span></span>|<span data-ttu-id="21f01-113">Gibt an, ob die moderne Anwendung von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="21f01-113">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="21f01-114">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="21f01-114">resourceAccess</span></span>|<span data-ttu-id="21f01-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="21f01-115">Boolean</span></span>|<span data-ttu-id="21f01-116">Gibt an, ob der Zugriff auf Ressourcen von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="21f01-116">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="21f01-117">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="21f01-117">deviceConfiguration</span></span>|<span data-ttu-id="21f01-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="21f01-118">Boolean</span></span>|<span data-ttu-id="21f01-119">Gibt an, ob die Gerätekonfiguration von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="21f01-119">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="21f01-120">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="21f01-120">compliancePolicy</span></span>|<span data-ttu-id="21f01-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="21f01-121">Boolean</span></span>|<span data-ttu-id="21f01-122">Gibt an, ob Compliance-Richtlinie von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="21f01-122">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="21f01-123">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="21f01-123">windowsUpdateForBusiness</span></span>|<span data-ttu-id="21f01-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="21f01-124">Boolean</span></span>|<span data-ttu-id="21f01-125">Gibt an, ob Windows Update for Business von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="21f01-125">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="21f01-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="21f01-126">Relationships</span></span>
<span data-ttu-id="21f01-127">Keine</span><span class="sxs-lookup"><span data-stu-id="21f01-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="21f01-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="21f01-128">JSON Representation</span></span>
<span data-ttu-id="21f01-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="21f01-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientEnabledFeatures",
  "inventory": true,
  "modernApps": true,
  "resourceAccess": true,
  "deviceConfiguration": true,
  "compliancePolicy": true,
  "windowsUpdateForBusiness": true
}
```



