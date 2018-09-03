# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="6cf9e-101">windowsUpdateScheduledInstall-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6cf9e-101">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="6cf9e-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6cf9e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6cf9e-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="6cf9e-103">Not yet documented</span></span>

<span data-ttu-id="6cf9e-104">Erbt von [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="6cf9e-104">Inherits from [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6cf9e-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6cf9e-105">Properties</span></span>
|<span data-ttu-id="6cf9e-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6cf9e-106">Property</span></span>|<span data-ttu-id="6cf9e-107">Typ</span><span class="sxs-lookup"><span data-stu-id="6cf9e-107">Type</span></span>|<span data-ttu-id="6cf9e-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6cf9e-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cf9e-109">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="6cf9e-109">scheduledInstallDay</span></span>|[<span data-ttu-id="6cf9e-110">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="6cf9e-110">weeklySchedule</span></span>](../resources/intune_deviceconfig_weeklyschedule.md)|<span data-ttu-id="6cf9e-111">Geplanter Installationstag in der Woche.</span><span class="sxs-lookup"><span data-stu-id="6cf9e-111">Scheduled Install Day in week Possible values are: , , , , , , , , .</span></span> <span data-ttu-id="6cf9e-112">Die möglichen Werte sind: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="6cf9e-112">The possible values are `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, , , or .</span></span>|
|<span data-ttu-id="6cf9e-113">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="6cf9e-113">scheduledInstallTime</span></span>|<span data-ttu-id="6cf9e-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6cf9e-114">TimeOfDay</span></span>|<span data-ttu-id="6cf9e-115">Geplante Installationszeit während des Tages</span><span class="sxs-lookup"><span data-stu-id="6cf9e-115">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="6cf9e-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6cf9e-116">Relationships</span></span>
<span data-ttu-id="6cf9e-117">Keine</span><span class="sxs-lookup"><span data-stu-id="6cf9e-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6cf9e-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6cf9e-118">JSON Representation</span></span>
<span data-ttu-id="6cf9e-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6cf9e-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.windowsUpdateInstallScheduleType",
  "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateScheduledInstall",
  "scheduledInstallDay": "String",
  "scheduledInstallTime": "String (time of day)"
}
```



