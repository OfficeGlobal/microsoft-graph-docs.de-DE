# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="7a8c0-101">deviceManagementExchangeConnectorType Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="7a8c0-101">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="7a8c0-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7a8c0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7a8c0-103">Der Typ des Exchange-Verbinders.</span><span class="sxs-lookup"><span data-stu-id="7a8c0-103">The type of Exchange Connector Configured.</span></span>
## <a name="members"></a><span data-ttu-id="7a8c0-104">Elemente</span><span class="sxs-lookup"><span data-stu-id="7a8c0-104">Members</span></span>
|<span data-ttu-id="7a8c0-105">Element</span><span class="sxs-lookup"><span data-stu-id="7a8c0-105">Member</span></span>|<span data-ttu-id="7a8c0-106">Wert</span><span class="sxs-lookup"><span data-stu-id="7a8c0-106">Value</span></span>|<span data-ttu-id="7a8c0-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7a8c0-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a8c0-108">onPremises</span><span class="sxs-lookup"><span data-stu-id="7a8c0-108">On-premises</span></span>|<span data-ttu-id="7a8c0-109">0</span><span class="sxs-lookup"><span data-stu-id="7a8c0-109">0%</span></span>|<span data-ttu-id="7a8c0-110">Stellt eine Verbindung zur lokalen Exchange-Umgebung her.</span><span class="sxs-lookup"><span data-stu-id="7a8c0-110">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="7a8c0-111">hosted</span><span class="sxs-lookup"><span data-stu-id="7a8c0-111">hosted</span></span>|<span data-ttu-id="7a8c0-112">1</span><span class="sxs-lookup"><span data-stu-id="7a8c0-112">-1</span></span>|<span data-ttu-id="7a8c0-113">Stellt eine Verbindung mit der mehrinstanzenfähigen Exchange-Umgebung von O365 her</span><span class="sxs-lookup"><span data-stu-id="7a8c0-113">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="7a8c0-114">serviceToService</span><span class="sxs-lookup"><span data-stu-id="7a8c0-114">Service-to-service</span></span>|<span data-ttu-id="7a8c0-115">2</span><span class="sxs-lookup"><span data-stu-id="7a8c0-115">-2</span></span>|<span data-ttu-id="7a8c0-116">Der Intune-Dienst stellt eine direkte Verbindung mit der mehrinstanzenfähigen Exchange-Umgebung von O365 her</span><span class="sxs-lookup"><span data-stu-id="7a8c0-116">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="7a8c0-117">dedicated</span><span class="sxs-lookup"><span data-stu-id="7a8c0-117">Dedicated</span></span>|<span data-ttu-id="7a8c0-118">3</span><span class="sxs-lookup"><span data-stu-id="7a8c0-118">-3</span></span>|<span data-ttu-id="7a8c0-119">Stellt eine Verbindung mit der speziellen Exchange-Umgebung von O365 her.</span><span class="sxs-lookup"><span data-stu-id="7a8c0-119">Connects to O365 Dedicated Exchange environment.</span></span>|








