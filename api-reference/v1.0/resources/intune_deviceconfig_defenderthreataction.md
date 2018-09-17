# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="4cb63-101">DefenderThreatAction Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="4cb63-101">defenderThreatAction enum type</span></span>

> <span data-ttu-id="4cb63-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4cb63-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4cb63-103">Standard-Aktion des Defenders, um auf erkannte Malware-Bedrohungen zu reagieren.</span><span class="sxs-lookup"><span data-stu-id="4cb63-103">Defender’s default action to take on detected Malware threats.</span></span>
## <a name="members"></a><span data-ttu-id="4cb63-104">Elemente</span><span class="sxs-lookup"><span data-stu-id="4cb63-104">Members</span></span>
|<span data-ttu-id="4cb63-105">Element</span><span class="sxs-lookup"><span data-stu-id="4cb63-105">Member</span></span>|<span data-ttu-id="4cb63-106">Wert</span><span class="sxs-lookup"><span data-stu-id="4cb63-106">Value</span></span>|<span data-ttu-id="4cb63-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4cb63-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cb63-108">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="4cb63-108">deviceDefault</span></span>|<span data-ttu-id="4cb63-109">0</span><span class="sxs-lookup"><span data-stu-id="4cb63-109">0%</span></span>|<span data-ttu-id="4cb63-110">Aktion basierend auf der Update-Definition anwenden.</span><span class="sxs-lookup"><span data-stu-id="4cb63-110">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="4cb63-111">clean</span><span class="sxs-lookup"><span data-stu-id="4cb63-111">clean</span></span>|<span data-ttu-id="4cb63-112">1</span><span class="sxs-lookup"><span data-stu-id="4cb63-112">-1</span></span>|<span data-ttu-id="4cb63-113">Die erkannte Bedrohung säubern.</span><span class="sxs-lookup"><span data-stu-id="4cb63-113">Clean the detected threat.</span></span>|
|<span data-ttu-id="4cb63-114">quarantine</span><span class="sxs-lookup"><span data-stu-id="4cb63-114">Quarantine</span></span>|<span data-ttu-id="4cb63-115">2</span><span class="sxs-lookup"><span data-stu-id="4cb63-115">-2</span></span>|<span data-ttu-id="4cb63-116">Die erkannte Bedrohung unter Quarantäne stellen.</span><span class="sxs-lookup"><span data-stu-id="4cb63-116">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="4cb63-117">remove</span><span class="sxs-lookup"><span data-stu-id="4cb63-117">remove</span></span>|<span data-ttu-id="4cb63-118">3</span><span class="sxs-lookup"><span data-stu-id="4cb63-118">-3</span></span>|<span data-ttu-id="4cb63-119">Erkannte Bedrohung entfernen.</span><span class="sxs-lookup"><span data-stu-id="4cb63-119">Remove the detected threat.</span></span>|
|<span data-ttu-id="4cb63-120">allow</span><span class="sxs-lookup"><span data-stu-id="4cb63-120">Allow</span></span>|<span data-ttu-id="4cb63-121">4</span><span class="sxs-lookup"><span data-stu-id="4cb63-121">-4</span></span>|<span data-ttu-id="4cb63-122">Zulassen der erkannten Bedrohung.</span><span class="sxs-lookup"><span data-stu-id="4cb63-122">Allow the detected threat.</span></span>|
|<span data-ttu-id="4cb63-123">userDefined</span><span class="sxs-lookup"><span data-stu-id="4cb63-123">User-defined</span></span>|<span data-ttu-id="4cb63-124">5</span><span class="sxs-lookup"><span data-stu-id="4cb63-124">$-5</span></span>|<span data-ttu-id="4cb63-125">Erlaubt es dem Benutzer, die Aktion zu bestimmen, die bei einer erkannten Bedrohung durchgeführt werden soll.</span><span class="sxs-lookup"><span data-stu-id="4cb63-125">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="4cb63-126">block</span><span class="sxs-lookup"><span data-stu-id="4cb63-126">Block</span></span>|<span data-ttu-id="4cb63-127">6</span><span class="sxs-lookup"><span data-stu-id="4cb63-127">-6</span></span>|<span data-ttu-id="4cb63-128">Blockieren der erkannten Bedrohung.</span><span class="sxs-lookup"><span data-stu-id="4cb63-128">Block the detected threat.</span></span>|








