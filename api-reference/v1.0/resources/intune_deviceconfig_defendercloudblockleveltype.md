# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="c4179-101">defenderCloudBlockLevelTyp Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="c4179-101">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="c4179-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c4179-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c4179-103">Mögliche Werte für die Cloud-Block-Ebene</span><span class="sxs-lookup"><span data-stu-id="c4179-103">Possible values of Cloud Block Level</span></span>
## <a name="members"></a><span data-ttu-id="c4179-104">Elemente</span><span class="sxs-lookup"><span data-stu-id="c4179-104">Members</span></span>
|<span data-ttu-id="c4179-105">Element</span><span class="sxs-lookup"><span data-stu-id="c4179-105">Member</span></span>|<span data-ttu-id="c4179-106">Wert</span><span class="sxs-lookup"><span data-stu-id="c4179-106">Value</span></span>|<span data-ttu-id="c4179-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c4179-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4179-108">Nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="c4179-108">notConfigured</span></span>|<span data-ttu-id="c4179-109">0</span><span class="sxs-lookup"><span data-stu-id="c4179-109">0%</span></span>|<span data-ttu-id="c4179-110">Standardwert: Verwendet die standardmäßige Windows Defender Antivirus-Blockierungsstufe und bietet eine starke Erkennung, ohne das Risiko zu erhöhen, legitime Dateien zu erkennen</span><span class="sxs-lookup"><span data-stu-id="c4179-110">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="c4179-111">high</span><span class="sxs-lookup"><span data-stu-id="c4179-111">High.</span></span>|<span data-ttu-id="c4179-112">1</span><span class="sxs-lookup"><span data-stu-id="c4179-112">-1</span></span>|<span data-ttu-id="c4179-113">Der Wert "high" wendet eine starke Erkennungsstufe an.</span><span class="sxs-lookup"><span data-stu-id="c4179-113">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="c4179-114">highPlus</span><span class="sxs-lookup"><span data-stu-id="c4179-114">highPlus</span></span>|<span data-ttu-id="c4179-115">2</span><span class="sxs-lookup"><span data-stu-id="c4179-115">-2</span></span>|<span data-ttu-id="c4179-116">High + verwendet das High-Level und wendet zusätzliche Schutzmaßnahmen an</span><span class="sxs-lookup"><span data-stu-id="c4179-116">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="c4179-117">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="c4179-117">zeroTolerance</span></span>|<span data-ttu-id="c4179-118">3</span><span class="sxs-lookup"><span data-stu-id="c4179-118">-3</span></span>|<span data-ttu-id="c4179-119">ZeroTolerance blockiert alle unbekannten, ausführbaren Dateien</span><span class="sxs-lookup"><span data-stu-id="c4179-119">Zero tolerance blocks all unknown executables</span></span>|








