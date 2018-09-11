# <a name="actionstate-enum-type"></a><span data-ttu-id="3873e-101">actionState Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="3873e-101">actionState enum type</span></span>

> <span data-ttu-id="3873e-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3873e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3873e-103">Status der Aktion auf dem Gerät</span><span class="sxs-lookup"><span data-stu-id="3873e-103">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="3873e-104">Elemente</span><span class="sxs-lookup"><span data-stu-id="3873e-104">Members</span></span>
|<span data-ttu-id="3873e-105">Element</span><span class="sxs-lookup"><span data-stu-id="3873e-105">Member</span></span>|<span data-ttu-id="3873e-106">Wert</span><span class="sxs-lookup"><span data-stu-id="3873e-106">Value</span></span>|<span data-ttu-id="3873e-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3873e-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3873e-108">keine</span><span class="sxs-lookup"><span data-stu-id="3873e-108">none</span></span>|<span data-ttu-id="3873e-109">0</span><span class="sxs-lookup"><span data-stu-id="3873e-109">0%</span></span>|<span data-ttu-id="3873e-110">Kein gültiger Aktionszustand</span><span class="sxs-lookup"><span data-stu-id="3873e-110">Not a valid action state</span></span>|
|<span data-ttu-id="3873e-111">pending</span><span class="sxs-lookup"><span data-stu-id="3873e-111">Pending</span></span>|<span data-ttu-id="3873e-112">1</span><span class="sxs-lookup"><span data-stu-id="3873e-112">-1</span></span>|<span data-ttu-id="3873e-113">Die Aktion steht noch aus</span><span class="sxs-lookup"><span data-stu-id="3873e-113">Action is pending</span></span>|
|<span data-ttu-id="3873e-114">canceled</span><span class="sxs-lookup"><span data-stu-id="3873e-114">Canceled</span></span>|<span data-ttu-id="3873e-115">2</span><span class="sxs-lookup"><span data-stu-id="3873e-115">-2</span></span>|<span data-ttu-id="3873e-116">Die Aktion wurde abgebrochen.</span><span class="sxs-lookup"><span data-stu-id="3873e-116">Action has been cancelled.</span></span>|
|<span data-ttu-id="3873e-117">active</span><span class="sxs-lookup"><span data-stu-id="3873e-117">Active</span></span>|<span data-ttu-id="3873e-118">3</span><span class="sxs-lookup"><span data-stu-id="3873e-118">-3</span></span>|<span data-ttu-id="3873e-119">Die Aktion ist aktiv.</span><span class="sxs-lookup"><span data-stu-id="3873e-119">Action is active.</span></span>|
|<span data-ttu-id="3873e-120">done</span><span class="sxs-lookup"><span data-stu-id="3873e-120">done</span></span>|<span data-ttu-id="3873e-121">4</span><span class="sxs-lookup"><span data-stu-id="3873e-121">-4</span></span>|<span data-ttu-id="3873e-122">Die Aktion wurde ohne Fehler abgeschlossen.</span><span class="sxs-lookup"><span data-stu-id="3873e-122">Action completed without errors.</span></span>|
|<span data-ttu-id="3873e-123">failed</span><span class="sxs-lookup"><span data-stu-id="3873e-123">failed</span></span>|<span data-ttu-id="3873e-124">5</span><span class="sxs-lookup"><span data-stu-id="3873e-124">$-5</span></span>|<span data-ttu-id="3873e-125">Die Aktion ist fehlgeschlagen</span><span class="sxs-lookup"><span data-stu-id="3873e-125">Action failed</span></span>|
|<span data-ttu-id="3873e-126">notSupported</span><span class="sxs-lookup"><span data-stu-id="3873e-126">notSupported</span></span>|<span data-ttu-id="3873e-127">6</span><span class="sxs-lookup"><span data-stu-id="3873e-127">-6</span></span>|<span data-ttu-id="3873e-128">Die Aktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3873e-128">Expand is not supported.</span></span>|








