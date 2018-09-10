# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="b8def-101">windowsUpdateActiveHoursInstall-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b8def-101">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="b8def-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b8def-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8def-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b8def-103">Not yet documented</span></span>

<span data-ttu-id="b8def-104">Erbt von [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="b8def-104">Inherits from [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b8def-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b8def-105">Properties</span></span>
|<span data-ttu-id="b8def-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b8def-106">Property</span></span>|<span data-ttu-id="b8def-107">Typ</span><span class="sxs-lookup"><span data-stu-id="b8def-107">Type</span></span>|<span data-ttu-id="b8def-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8def-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8def-109">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="b8def-109">activeHoursStart</span></span>|<span data-ttu-id="b8def-110">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b8def-110">TimeOfDay</span></span>|<span data-ttu-id="b8def-111">Beginn der aktiven Stunden</span><span class="sxs-lookup"><span data-stu-id="b8def-111">Active Hours Start</span></span>|
|<span data-ttu-id="b8def-112">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="b8def-112">activeHoursEnd</span></span>|<span data-ttu-id="b8def-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b8def-113">TimeOfDay</span></span>|<span data-ttu-id="b8def-114">Ende der aktiven Stunden</span><span class="sxs-lookup"><span data-stu-id="b8def-114">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8def-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b8def-115">Relationships</span></span>
<span data-ttu-id="b8def-116">Keine</span><span class="sxs-lookup"><span data-stu-id="b8def-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b8def-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b8def-117">JSON Representation</span></span>
<span data-ttu-id="b8def-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b8def-118">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateActiveHoursInstall"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateActiveHoursInstall",
  "activeHoursStart": "String (time of day)",
  "activeHoursEnd": "String (time of day)"
}
```








