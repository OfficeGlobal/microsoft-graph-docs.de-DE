# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="ca18b-101">deviceEnrollmentPlatformRestriction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ca18b-101">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="ca18b-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ca18b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ca18b-103">Plattformspezifische Registrierungseinschränkungen</span><span class="sxs-lookup"><span data-stu-id="ca18b-103">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="ca18b-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ca18b-104">Properties</span></span>
|<span data-ttu-id="ca18b-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ca18b-105">Property</span></span>|<span data-ttu-id="ca18b-106">Typ</span><span class="sxs-lookup"><span data-stu-id="ca18b-106">Type</span></span>|<span data-ttu-id="ca18b-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ca18b-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca18b-108">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="ca18b-108">platformBlocked</span></span>|<span data-ttu-id="ca18b-109">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ca18b-109">Boolean</span></span>|<span data-ttu-id="ca18b-110">Sperren der Plattform für die Registrierung</span><span class="sxs-lookup"><span data-stu-id="ca18b-110">Block the platform from enrolling</span></span>|
|<span data-ttu-id="ca18b-111">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="ca18b-111">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="ca18b-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ca18b-112">Boolean</span></span>|<span data-ttu-id="ca18b-113">Sperren privat genutzter Geräte für die Registrierung</span><span class="sxs-lookup"><span data-stu-id="ca18b-113">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="ca18b-114">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="ca18b-114">osMinimumVersion</span></span>|<span data-ttu-id="ca18b-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca18b-115">String</span></span>|<span data-ttu-id="ca18b-116">Unterstützte mindestens benötigte iOS-Version</span><span class="sxs-lookup"><span data-stu-id="ca18b-116">Min OS version supported</span></span>|
|<span data-ttu-id="ca18b-117">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="ca18b-117">osMaximumVersion</span></span>|<span data-ttu-id="ca18b-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca18b-118">String</span></span>|<span data-ttu-id="ca18b-119">Unterstützte maximal verwendbare iOS-Version</span><span class="sxs-lookup"><span data-stu-id="ca18b-119">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca18b-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ca18b-120">Relationships</span></span>
<span data-ttu-id="ca18b-121">Keine</span><span class="sxs-lookup"><span data-stu-id="ca18b-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ca18b-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ca18b-122">JSON Representation</span></span>
<span data-ttu-id="ca18b-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ca18b-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestriction",
  "platformBlocked": true,
  "personalDeviceEnrollmentBlocked": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String"
}
```



