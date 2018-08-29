# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="3dfce-101">eBookInstallSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3dfce-101">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="3dfce-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3dfce-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3dfce-103">Enthält Eigenschaften für die Installationszusammenfassung eines Buchs für ein Gerät.</span><span class="sxs-lookup"><span data-stu-id="3dfce-103">Contains properties for the installation summary of a book for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="3dfce-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="3dfce-104">Methods</span></span>
|<span data-ttu-id="3dfce-105">Methode</span><span class="sxs-lookup"><span data-stu-id="3dfce-105">Method</span></span>|<span data-ttu-id="3dfce-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="3dfce-106">Return Type</span></span>|<span data-ttu-id="3dfce-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3dfce-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3dfce-108">eBookInstallSummary abrufen</span><span class="sxs-lookup"><span data-stu-id="3dfce-108">Get eBookInstallSummary</span></span>](../api/intune_books_ebookinstallsummary_get.md)|[<span data-ttu-id="3dfce-109">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="3dfce-109">eBookInstallSummary</span></span>](../resources/intune_books_ebookinstallsummary.md)|<span data-ttu-id="3dfce-110">Lesen der Eigenschaften und Beziehungen von [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md)-Objekten.</span><span class="sxs-lookup"><span data-stu-id="3dfce-110">Read properties and relationships of the [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="3dfce-111">eBookInstallSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3dfce-111">Update eBookInstallSummary</span></span>](../api/intune_books_ebookinstallsummary_update.md)|[<span data-ttu-id="3dfce-112">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="3dfce-112">eBookInstallSummary</span></span>](../resources/intune_books_ebookinstallsummary.md)|<span data-ttu-id="3dfce-113">Aktualisieren der Eigenschaften des [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3dfce-113">Update the properties of a [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3dfce-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3dfce-114">Properties</span></span>
|<span data-ttu-id="3dfce-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3dfce-115">Property</span></span>|<span data-ttu-id="3dfce-116">Typ</span><span class="sxs-lookup"><span data-stu-id="3dfce-116">Type</span></span>|<span data-ttu-id="3dfce-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3dfce-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3dfce-118">id</span><span class="sxs-lookup"><span data-stu-id="3dfce-118">id</span></span>|<span data-ttu-id="3dfce-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3dfce-119">String</span></span>|<span data-ttu-id="3dfce-120">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="3dfce-120">Key of the entity.</span></span>|
|<span data-ttu-id="3dfce-121">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3dfce-121">installedDeviceCount</span></span>|<span data-ttu-id="3dfce-122">Int32</span><span class="sxs-lookup"><span data-stu-id="3dfce-122">Int32</span></span>|<span data-ttu-id="3dfce-123">Die Anzahl der Geräte, auf denen das Buch erfolgreich installiert wurde.</span><span class="sxs-lookup"><span data-stu-id="3dfce-123">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="3dfce-124">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3dfce-124">failedDeviceCount</span></span>|<span data-ttu-id="3dfce-125">Int32</span><span class="sxs-lookup"><span data-stu-id="3dfce-125">Int32</span></span>|<span data-ttu-id="3dfce-126">Die Anzahl der Geräte, auf denen die Installation des Buchs fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="3dfce-126">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="3dfce-127">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3dfce-127">notInstalledDeviceCount</span></span>|<span data-ttu-id="3dfce-128">Int32</span><span class="sxs-lookup"><span data-stu-id="3dfce-128">Int32</span></span>|<span data-ttu-id="3dfce-129">Die Anzahl von Geräten, auf denen das Buch nicht installiert ist.</span><span class="sxs-lookup"><span data-stu-id="3dfce-129">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="3dfce-130">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="3dfce-130">installedUserCount</span></span>|<span data-ttu-id="3dfce-131">Int32</span><span class="sxs-lookup"><span data-stu-id="3dfce-131">Int32</span></span>|<span data-ttu-id="3dfce-132">Die Anzahl der Benutzer, deren Geräte das Buch erfolgreich installiert haben.</span><span class="sxs-lookup"><span data-stu-id="3dfce-132">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="3dfce-133">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="3dfce-133">failedUserCount</span></span>|<span data-ttu-id="3dfce-134">Int32</span><span class="sxs-lookup"><span data-stu-id="3dfce-134">Int32</span></span>|<span data-ttu-id="3dfce-135">Die Anzahl der Benutzer, die mindestens ein Gerät besitzen, auf dem die Installation des Buchs fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="3dfce-135">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="3dfce-136">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="3dfce-136">notInstalledUserCount</span></span>|<span data-ttu-id="3dfce-137">Int32</span><span class="sxs-lookup"><span data-stu-id="3dfce-137">Int32</span></span>|<span data-ttu-id="3dfce-138">Die Anzahl der Benutzer, die das Buch nicht installiert haben.</span><span class="sxs-lookup"><span data-stu-id="3dfce-138">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3dfce-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3dfce-139">Relationships</span></span>
<span data-ttu-id="3dfce-140">Keine</span><span class="sxs-lookup"><span data-stu-id="3dfce-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3dfce-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3dfce-141">JSON Representation</span></span>
<span data-ttu-id="3dfce-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3dfce-142">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.eBookInstallSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024,
  "installedUserCount": 1024,
  "failedUserCount": 1024,
  "notInstalledUserCount": 1024
}
```



