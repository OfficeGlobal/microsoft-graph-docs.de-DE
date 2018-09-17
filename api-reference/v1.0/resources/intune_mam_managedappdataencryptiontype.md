# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="dbe2b-101">ManagedAppDataEncryptionType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="dbe2b-101">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="dbe2b-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="dbe2b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dbe2b-103">Stellt den Verschlüsselungsgrad von App-Daten für verwaltete Apps dar</span><span class="sxs-lookup"><span data-stu-id="dbe2b-103">Represents the level to which app data is encrypted for managed apps</span></span>
## <a name="members"></a><span data-ttu-id="dbe2b-104">Elemente</span><span class="sxs-lookup"><span data-stu-id="dbe2b-104">Members</span></span>
|<span data-ttu-id="dbe2b-105">Element</span><span class="sxs-lookup"><span data-stu-id="dbe2b-105">Member</span></span>|<span data-ttu-id="dbe2b-106">Wert</span><span class="sxs-lookup"><span data-stu-id="dbe2b-106">Value</span></span>|<span data-ttu-id="dbe2b-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dbe2b-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbe2b-108">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="dbe2b-108">useDeviceSettings</span></span>|<span data-ttu-id="dbe2b-109">0</span><span class="sxs-lookup"><span data-stu-id="dbe2b-109">0%</span></span>|<span data-ttu-id="dbe2b-110">App-Daten werden basierend auf den Standardeinstellungen des Geräts verschlüsselt.</span><span class="sxs-lookup"><span data-stu-id="dbe2b-110">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="dbe2b-111">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="dbe2b-111">afterDeviceRestart</span></span>|<span data-ttu-id="dbe2b-112">1</span><span class="sxs-lookup"><span data-stu-id="dbe2b-112">-1</span></span>|<span data-ttu-id="dbe2b-113">App-Daten werden verschlüsselt, wenn das Gerät neu gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="dbe2b-113">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="dbe2b-114">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="dbe2b-114">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="dbe2b-115">2</span><span class="sxs-lookup"><span data-stu-id="dbe2b-115">-2</span></span>|<span data-ttu-id="dbe2b-116">App-Daten, die dieser Richtlinie zugeordnet sind, werden verschlüsselt, wenn das Gerät gesperrt ist. Davon ausgenommen sind Daten in geöffneten Dateien.</span><span class="sxs-lookup"><span data-stu-id="dbe2b-116">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="dbe2b-117">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="dbe2b-117">whenDeviceLocked</span></span>|<span data-ttu-id="dbe2b-118">3</span><span class="sxs-lookup"><span data-stu-id="dbe2b-118">-3</span></span>|<span data-ttu-id="dbe2b-119">App-Daten, die dieser Richtlinie zugeordnet sind, werden verschlüsselt, wenn das Gerät gesperrt ist.</span><span class="sxs-lookup"><span data-stu-id="dbe2b-119">App data associated with this policy is encrypted when the device is locked</span></span>|








