# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="7053f-101">managedAppPolicyDeploymentSummaryPerApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7053f-101">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="7053f-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7053f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7053f-103">Zusammenfassung der Richtlinienbereitstellung pro App</span><span class="sxs-lookup"><span data-stu-id="7053f-103">Represents policy deployment summary per app.</span></span>
## <a name="properties"></a><span data-ttu-id="7053f-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7053f-104">Properties</span></span>
|<span data-ttu-id="7053f-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7053f-105">Property</span></span>|<span data-ttu-id="7053f-106">Typ</span><span class="sxs-lookup"><span data-stu-id="7053f-106">Type</span></span>|<span data-ttu-id="7053f-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7053f-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7053f-108">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="7053f-108">mobileAppIdentifier</span></span>|[<span data-ttu-id="7053f-109">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="7053f-109">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="7053f-110">Bereitstellung einer App</span><span class="sxs-lookup"><span data-stu-id="7053f-110">Deployment of an app.</span></span>|
|<span data-ttu-id="7053f-111">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="7053f-111">configurationAppliedUserCount</span></span>|<span data-ttu-id="7053f-112">Int32</span><span class="sxs-lookup"><span data-stu-id="7053f-112">Int32</span></span>|<span data-ttu-id="7053f-113">Die Anzahl der Benutzer, auf die die Richtlinie angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="7053f-113">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7053f-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7053f-114">Relationships</span></span>
<span data-ttu-id="7053f-115">Keine</span><span class="sxs-lookup"><span data-stu-id="7053f-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7053f-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7053f-116">JSON Representation</span></span>
<span data-ttu-id="7053f-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7053f-117">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "configurationAppliedUserCount": 1024
}
```



