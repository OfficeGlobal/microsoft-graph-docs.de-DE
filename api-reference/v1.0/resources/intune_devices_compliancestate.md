# <a name="compliancestate-enum-type"></a><span data-ttu-id="97db5-101">complianceState Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="97db5-101">complianceState enum type</span></span>

> <span data-ttu-id="97db5-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="97db5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97db5-103">Compliance-Status.</span><span class="sxs-lookup"><span data-stu-id="97db5-103">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="97db5-104">Elemente</span><span class="sxs-lookup"><span data-stu-id="97db5-104">Members</span></span>
|<span data-ttu-id="97db5-105">Element</span><span class="sxs-lookup"><span data-stu-id="97db5-105">Member</span></span>|<span data-ttu-id="97db5-106">Wert</span><span class="sxs-lookup"><span data-stu-id="97db5-106">Value</span></span>|<span data-ttu-id="97db5-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97db5-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97db5-108">unbekannt</span><span class="sxs-lookup"><span data-stu-id="97db5-108">unknown</span></span>|<span data-ttu-id="97db5-109">0</span><span class="sxs-lookup"><span data-stu-id="97db5-109">0%</span></span>|<span data-ttu-id="97db5-110">Unbekannt.</span><span class="sxs-lookup"><span data-stu-id="97db5-110">Unknown</span></span>|
|<span data-ttu-id="97db5-111">compliant</span><span class="sxs-lookup"><span data-stu-id="97db5-111">Compliant</span></span>|<span data-ttu-id="97db5-112">1</span><span class="sxs-lookup"><span data-stu-id="97db5-112">-1</span></span>|<span data-ttu-id="97db5-113">Kompatibel.</span><span class="sxs-lookup"><span data-stu-id="97db5-113">Compliant</span></span>|
|<span data-ttu-id="97db5-114">noncompliant</span><span class="sxs-lookup"><span data-stu-id="97db5-114">noncompliant</span></span>|<span data-ttu-id="97db5-115">2</span><span class="sxs-lookup"><span data-stu-id="97db5-115">-2</span></span>|<span data-ttu-id="97db5-116">Das Gerät ist nicht kompatibel und wird von Unternehmensressourcen blockiert.</span><span class="sxs-lookup"><span data-stu-id="97db5-116">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="97db5-117">Konflikt</span><span class="sxs-lookup"><span data-stu-id="97db5-117">Conflict</span></span>|<span data-ttu-id="97db5-118">3</span><span class="sxs-lookup"><span data-stu-id="97db5-118">-3</span></span>|<span data-ttu-id="97db5-119">Konflikt mit anderen Regeln.</span><span class="sxs-lookup"><span data-stu-id="97db5-119">Conflict with other rules.</span></span>|
|<span data-ttu-id="97db5-120">Fehler</span><span class="sxs-lookup"><span data-stu-id="97db5-120">error</span></span>|<span data-ttu-id="97db5-121">4</span><span class="sxs-lookup"><span data-stu-id="97db5-121">-4</span></span>|<span data-ttu-id="97db5-122">Fehler.</span><span class="sxs-lookup"><span data-stu-id="97db5-122">Error.</span></span>|
|<span data-ttu-id="97db5-123">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="97db5-123">inGracePeriod</span></span>|<span data-ttu-id="97db5-124">254
</span><span class="sxs-lookup"><span data-stu-id="97db5-124">254</span></span>|<span data-ttu-id="97db5-125">Das Gerät ist nicht kompatibel, hat aber dennoch Zugriff auf Unternehmensressourcen</span><span class="sxs-lookup"><span data-stu-id="97db5-125">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="97db5-126">configManager</span><span class="sxs-lookup"><span data-stu-id="97db5-126">configManager</span></span>|<span data-ttu-id="97db5-127">255</span><span class="sxs-lookup"><span data-stu-id="97db5-127">255 characters</span></span>|<span data-ttu-id="97db5-128">Vom Konfigurations-Manager verwaltet</span><span class="sxs-lookup"><span data-stu-id="97db5-128">Managed by Config Manager</span></span>|








