# <a name="sharedpcaccountmanagerpolicy-resource-type"></a><span data-ttu-id="42883-101">sharedPCAccountManagerPolicy-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="42883-101">sharedPCAccountManagerPolicy resource type</span></span>

> <span data-ttu-id="42883-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="42883-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="42883-103">SharedPC-Konto-Manager-Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="42883-103">SharedPC Account Manager Policy.</span></span> <span data-ttu-id="42883-104">Gilt nur, wenn der Konto-Manager aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="42883-104">Only applies when the account manager is enabled.</span></span>
## <a name="properties"></a><span data-ttu-id="42883-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="42883-105">Properties</span></span>
|<span data-ttu-id="42883-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="42883-106">Property</span></span>|<span data-ttu-id="42883-107">Typ</span><span class="sxs-lookup"><span data-stu-id="42883-107">Type</span></span>|<span data-ttu-id="42883-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="42883-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42883-109">accountDeletionPolicy</span><span class="sxs-lookup"><span data-stu-id="42883-109">accountDeletionPolicy</span></span>|[<span data-ttu-id="42883-110">sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="42883-110">sharedPCAccountDeletionPolicyType</span></span>](../resources/intune_deviceconfig_sharedpcaccountdeletionpolicytype.md)|<span data-ttu-id="42883-111">Konfiguriert, wann Konten gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="42883-111">Configures when accounts are deleted.</span></span> <span data-ttu-id="42883-112">Mögliche Werte sind: `immediate`, `diskSpaceThreshold` und `diskSpaceThresholdOrInactiveThreshold`.</span><span class="sxs-lookup"><span data-stu-id="42883-112">Possible values are: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span></span>|
|<span data-ttu-id="42883-113">cacheAccountsAboveDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="42883-113">cacheAccountsAboveDiskFreePercentage</span></span>|<span data-ttu-id="42883-114">Int32</span><span class="sxs-lookup"><span data-stu-id="42883-114">Int32</span></span>|<span data-ttu-id="42883-115">Legt den Prozentsatz des verfügbaren Speicherplatzes fest, den ein PC haben sollte, damit keine weiteren zwischengespeicherten freigegebenen PC-Konten gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="42883-115">Sets the percentage of available disk space a PC should have before it stops deleting cached shared PC accounts.</span></span> <span data-ttu-id="42883-116">Gilt nur, wenn AccountDeletionPolicy den Wert DiskSpaceThreshold oder DiskSpaceThresholdOrInactiveThreshold hat.</span><span class="sxs-lookup"><span data-stu-id="42883-116">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="42883-117">Gültige Werte: 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="42883-117">Valid values 0 to 100</span></span>|
|<span data-ttu-id="42883-118">inactiveThresholdDays</span><span class="sxs-lookup"><span data-stu-id="42883-118">inactiveThresholdDays</span></span>|<span data-ttu-id="42883-119">Int32</span><span class="sxs-lookup"><span data-stu-id="42883-119">Int32</span></span>|<span data-ttu-id="42883-120">Gibt an, wann mit dem Löschen von Konten begonnen wird, wenn während des angegebenen Zeitraums (Anzahl von Tagen) keine Anmeldung stattgefunden hat.</span><span class="sxs-lookup"><span data-stu-id="42883-120">Specifies when the accounts will start being deleted when they have not been logged on during the specified period, given as number of days.</span></span> <span data-ttu-id="42883-121">Gilt nur, wenn AccountDeletionPolicy den Wert DiskSpaceThreshold oder DiskSpaceThresholdOrInactiveThreshold hat.</span><span class="sxs-lookup"><span data-stu-id="42883-121">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span>|
|<span data-ttu-id="42883-122">removeAccountsBelowDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="42883-122">removeAccountsBelowDiskFreePercentage</span></span>|<span data-ttu-id="42883-123">Int32</span><span class="sxs-lookup"><span data-stu-id="42883-123">Int32</span></span>|<span data-ttu-id="42883-124">Legt den auf einem PC verbleibenden Prozentsatz an Speicherplatz fest, ab dem Konten im Cache gelöscht werden, um Speicherplatz freizugeben.</span><span class="sxs-lookup"><span data-stu-id="42883-124">Sets the percentage of disk space remaining on a PC before cached accounts will be deleted to free disk space.</span></span> <span data-ttu-id="42883-125">Konten, die am längsten inaktiv waren, werden zuerst gelöscht.</span><span class="sxs-lookup"><span data-stu-id="42883-125">Accounts that have been inactive the longest will be deleted first.</span></span> <span data-ttu-id="42883-126">Gilt nur, wenn AccountDeletionPolicy den Wert DiskSpaceThresholdOrInactiveThreshold hat.</span><span class="sxs-lookup"><span data-stu-id="42883-126">Only applies when AccountDeletionPolicy is DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="42883-127">Gültige Werte: 0 bis 100.</span><span class="sxs-lookup"><span data-stu-id="42883-127">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="42883-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="42883-128">Relationships</span></span>
<span data-ttu-id="42883-129">Keine</span><span class="sxs-lookup"><span data-stu-id="42883-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="42883-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="42883-130">JSON Representation</span></span>
<span data-ttu-id="42883-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="42883-131">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedPCAccountManagerPolicy",
  "accountDeletionPolicy": "String",
  "cacheAccountsAboveDiskFreePercentage": 1024,
  "inactiveThresholdDays": 1024,
  "removeAccountsBelowDiskFreePercentage": 1024
}
```








