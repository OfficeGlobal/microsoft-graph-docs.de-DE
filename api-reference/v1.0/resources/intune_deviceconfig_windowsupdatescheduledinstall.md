# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="4f2d7-101">windowsUpdateScheduledInstall-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4f2d7-101">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="4f2d7-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4f2d7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4f2d7-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="4f2d7-103">Not yet documented</span></span>

<span data-ttu-id="4f2d7-104">Erbt von [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="4f2d7-104">Inherits from [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4f2d7-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4f2d7-105">Properties</span></span>
|<span data-ttu-id="4f2d7-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4f2d7-106">Property</span></span>|<span data-ttu-id="4f2d7-107">Typ</span><span class="sxs-lookup"><span data-stu-id="4f2d7-107">Type</span></span>|<span data-ttu-id="4f2d7-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4f2d7-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f2d7-109">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="4f2d7-109">scheduledInstallDay</span></span>|<span data-ttu-id="4f2d7-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4f2d7-110">String</span></span>|<span data-ttu-id="4f2d7-111">Geplanter Installationstag in der Woche; mögliche Werte sind: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="4f2d7-111">Scheduled Install Day in week Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="4f2d7-112">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="4f2d7-112">scheduledInstallTime</span></span>|<span data-ttu-id="4f2d7-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="4f2d7-113">TimeOfDay</span></span>|<span data-ttu-id="4f2d7-114">Geplante Installationszeit während des Tages</span><span class="sxs-lookup"><span data-stu-id="4f2d7-114">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f2d7-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4f2d7-115">Relationships</span></span>
<span data-ttu-id="4f2d7-116">Keine</span><span class="sxs-lookup"><span data-stu-id="4f2d7-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4f2d7-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4f2d7-117">JSON Representation</span></span>
<span data-ttu-id="4f2d7-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4f2d7-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



