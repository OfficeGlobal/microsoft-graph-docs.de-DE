# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="64828-101">windowsUpdateScheduledInstall-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="64828-101">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="64828-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="64828-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="64828-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="64828-103">Not yet documented</span></span>

<span data-ttu-id="64828-104">Erbt von [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="64828-104">Inherits from [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="64828-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="64828-105">Properties</span></span>
|<span data-ttu-id="64828-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="64828-106">Property</span></span>|<span data-ttu-id="64828-107">Typ</span><span class="sxs-lookup"><span data-stu-id="64828-107">Type</span></span>|<span data-ttu-id="64828-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="64828-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64828-109">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="64828-109">scheduledInstallDay</span></span>|[<span data-ttu-id="64828-110">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="64828-110">weeklySchedule</span></span>](../resources/intune_deviceconfig_weeklyschedule.md)|<span data-ttu-id="64828-111">Geplante installieren Tag in der Woche.</span><span class="sxs-lookup"><span data-stu-id="64828-111">Scheduled Install Day in week.</span></span> <span data-ttu-id="64828-112">Mögliche Werte: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="64828-112">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="64828-113">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="64828-113">scheduledInstallTime</span></span>|<span data-ttu-id="64828-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="64828-114">TimeOfDay</span></span>|<span data-ttu-id="64828-115">Geplante Installationszeit während des Tages</span><span class="sxs-lookup"><span data-stu-id="64828-115">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="64828-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="64828-116">Relationships</span></span>
<span data-ttu-id="64828-117">Keine</span><span class="sxs-lookup"><span data-stu-id="64828-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="64828-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="64828-118">JSON Representation</span></span>
<span data-ttu-id="64828-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="64828-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateScheduledInstall",
  "scheduledInstallDay": "String",
  "scheduledInstallTime": "String (time of day)"
}
```



