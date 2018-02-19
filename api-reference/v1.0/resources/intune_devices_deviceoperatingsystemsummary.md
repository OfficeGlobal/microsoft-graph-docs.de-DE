# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="387a8-101">deviceOperatingSystemSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="387a8-101">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="387a8-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="387a8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="387a8-103">Betriebssystem des Geräts – Zusammenfassung.</span><span class="sxs-lookup"><span data-stu-id="387a8-103">Device operating system summary.</span></span>
## <a name="properties"></a><span data-ttu-id="387a8-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="387a8-104">Properties</span></span>
|<span data-ttu-id="387a8-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="387a8-105">Property</span></span>|<span data-ttu-id="387a8-106">Typ</span><span class="sxs-lookup"><span data-stu-id="387a8-106">Type</span></span>|<span data-ttu-id="387a8-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="387a8-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="387a8-108">androidCount</span><span class="sxs-lookup"><span data-stu-id="387a8-108">androidCount</span></span>|<span data-ttu-id="387a8-109">Int32</span><span class="sxs-lookup"><span data-stu-id="387a8-109">Int32</span></span>|<span data-ttu-id="387a8-110">Anzahl der Android-Geräte.</span><span class="sxs-lookup"><span data-stu-id="387a8-110">Number of android device count.</span></span>|
|<span data-ttu-id="387a8-111">iosCount</span><span class="sxs-lookup"><span data-stu-id="387a8-111">iosCount</span></span>|<span data-ttu-id="387a8-112">Int32</span><span class="sxs-lookup"><span data-stu-id="387a8-112">Int32</span></span>|<span data-ttu-id="387a8-113">Anzahl der iOS-Geräte.</span><span class="sxs-lookup"><span data-stu-id="387a8-113">Number of iOS device count.</span></span>|
|<span data-ttu-id="387a8-114">macOSCount</span><span class="sxs-lookup"><span data-stu-id="387a8-114">macOSCount</span></span>|<span data-ttu-id="387a8-115">Int32</span><span class="sxs-lookup"><span data-stu-id="387a8-115">Int32</span></span>|<span data-ttu-id="387a8-116">Anzahl der Mac OS X-Geräte.</span><span class="sxs-lookup"><span data-stu-id="387a8-116">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="387a8-117">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="387a8-117">windowsMobileCount</span></span>|<span data-ttu-id="387a8-118">Int32</span><span class="sxs-lookup"><span data-stu-id="387a8-118">Int32</span></span>|<span data-ttu-id="387a8-119">Anzahl der Windows Mobile-Geräte.</span><span class="sxs-lookup"><span data-stu-id="387a8-119">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="387a8-120">windowsCount</span><span class="sxs-lookup"><span data-stu-id="387a8-120">windowsCount</span></span>|<span data-ttu-id="387a8-121">Int32</span><span class="sxs-lookup"><span data-stu-id="387a8-121">Int32</span></span>|<span data-ttu-id="387a8-122">Anzahl der Windows-Geräte.</span><span class="sxs-lookup"><span data-stu-id="387a8-122">Number of Windows device count.</span></span>|
|<span data-ttu-id="387a8-123">unknownCount</span><span class="sxs-lookup"><span data-stu-id="387a8-123">unknownCount</span></span>|<span data-ttu-id="387a8-124">Int32</span><span class="sxs-lookup"><span data-stu-id="387a8-124">Int32</span></span>|<span data-ttu-id="387a8-125">Anzahl von unbekannten Geräten.</span><span class="sxs-lookup"><span data-stu-id="387a8-125">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="387a8-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="387a8-126">Relationships</span></span>
<span data-ttu-id="387a8-127">Keine</span><span class="sxs-lookup"><span data-stu-id="387a8-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="387a8-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="387a8-128">JSON Representation</span></span>
<span data-ttu-id="387a8-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="387a8-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceOperatingSystemSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceOperatingSystemSummary",
  "androidCount": 1024,
  "iosCount": 1024,
  "macOSCount": 1024,
  "windowsMobileCount": 1024,
  "windowsCount": 1024,
  "unknownCount": 1024
}
```



