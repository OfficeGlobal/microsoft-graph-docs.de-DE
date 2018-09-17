# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="c474c-101">appLockerApplicationControlType Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="c474c-101">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="c474c-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c474c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c474c-103">Mögliche Werte von AppLocker Anwendungs-Steuerelementtypen</span><span class="sxs-lookup"><span data-stu-id="c474c-103">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="c474c-104">Elemente</span><span class="sxs-lookup"><span data-stu-id="c474c-104">Members</span></span>
|<span data-ttu-id="c474c-105">Element</span><span class="sxs-lookup"><span data-stu-id="c474c-105">Member</span></span>|<span data-ttu-id="c474c-106">Wert</span><span class="sxs-lookup"><span data-stu-id="c474c-106">Value</span></span>|<span data-ttu-id="c474c-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c474c-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c474c-108">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c474c-108">notConfigured</span></span>|<span data-ttu-id="c474c-109">0</span><span class="sxs-lookup"><span data-stu-id="c474c-109">0%</span></span>|<span data-ttu-id="c474c-110">Standardwert des Geräts, kein Anwendungs-Steuerelementtyp ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="c474c-110">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="c474c-111">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="c474c-111">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="c474c-112">1</span><span class="sxs-lookup"><span data-stu-id="c474c-112">-1</span></span>|<span data-ttu-id="c474c-113">Windows-Komponenten und Store-Apps erzwingen.</span><span class="sxs-lookup"><span data-stu-id="c474c-113">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="c474c-114">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="c474c-114">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="c474c-115">2</span><span class="sxs-lookup"><span data-stu-id="c474c-115">-2</span></span>|<span data-ttu-id="c474c-116">Windows-Komponenten und Store-Apps prüfen.</span><span class="sxs-lookup"><span data-stu-id="c474c-116">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="c474c-117">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="c474c-117">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="c474c-118">3</span><span class="sxs-lookup"><span data-stu-id="c474c-118">-3</span></span>|<span data-ttu-id="c474c-119">Windows-Komponenten, Store-Apps und Smart Locker erzwingen.</span><span class="sxs-lookup"><span data-stu-id="c474c-119">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="c474c-120">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="c474c-120">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="c474c-121">4</span><span class="sxs-lookup"><span data-stu-id="c474c-121">-4</span></span>|<span data-ttu-id="c474c-122">Windows-Komponenten, Store-Apps und Smart Locker prüfen.</span><span class="sxs-lookup"><span data-stu-id="c474c-122">Audit Windows components, store apps and smart locker.</span></span>|








