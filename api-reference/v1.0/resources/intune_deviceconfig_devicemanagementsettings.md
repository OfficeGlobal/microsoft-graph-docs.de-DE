# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="d8251-101">deviceManagementSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d8251-101">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="d8251-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d8251-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8251-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="d8251-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="d8251-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d8251-104">Properties</span></span>
|<span data-ttu-id="d8251-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d8251-105">Property</span></span>|<span data-ttu-id="d8251-106">Typ</span><span class="sxs-lookup"><span data-stu-id="d8251-106">Type</span></span>|<span data-ttu-id="d8251-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d8251-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8251-108">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="d8251-108">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="d8251-109">Int32</span><span class="sxs-lookup"><span data-stu-id="d8251-109">Int32</span></span>|<span data-ttu-id="d8251-110">Die Anzahl von Tagen, die ein Gerät ohne Einchecken konform bleiben kann.</span><span class="sxs-lookup"><span data-stu-id="d8251-110">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="d8251-111">Gültige Werte: 0 bis 120</span><span class="sxs-lookup"><span data-stu-id="d8251-111">Valid values 0 to 120</span></span>|
|<span data-ttu-id="d8251-112">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="d8251-112">isScheduledActionEnabled</span></span>|<span data-ttu-id="d8251-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8251-113">Boolean</span></span>|<span data-ttu-id="d8251-114">Gibt an, ob das Feature für eine geplante Aktion für die Regel aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="d8251-114">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="d8251-115">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="d8251-115">secureByDefault</span></span>|<span data-ttu-id="d8251-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8251-116">Boolean</span></span>|<span data-ttu-id="d8251-117">Ist dies auf „true“ gesetzt, sollte das Gerät als nicht konform gelten, wenn keine Konformitätsrichtlinie verfolgt wird.</span><span class="sxs-lookup"><span data-stu-id="d8251-117">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8251-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d8251-118">Relationships</span></span>
<span data-ttu-id="d8251-119">Keine</span><span class="sxs-lookup"><span data-stu-id="d8251-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d8251-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d8251-120">JSON Representation</span></span>
<span data-ttu-id="d8251-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d8251-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettings",
  "deviceComplianceCheckinThresholdDays": 1024,
  "isScheduledActionEnabled": true,
  "secureByDefault": true
}
```



