# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="2e9db-101">groupAssignmentTarget-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2e9db-101">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="2e9db-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2e9db-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2e9db-103">Stellt eine Zuweisung zu einer Gruppe dar.</span><span class="sxs-lookup"><span data-stu-id="2e9db-103">Represents an assignment to a group.</span></span>

<span data-ttu-id="2e9db-104">Erbt von [deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="2e9db-104">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2e9db-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2e9db-105">Properties</span></span>
|<span data-ttu-id="2e9db-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2e9db-106">Property</span></span>|<span data-ttu-id="2e9db-107">Typ</span><span class="sxs-lookup"><span data-stu-id="2e9db-107">Type</span></span>|<span data-ttu-id="2e9db-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2e9db-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e9db-109">groupId</span><span class="sxs-lookup"><span data-stu-id="2e9db-109">groupId</span></span>|<span data-ttu-id="2e9db-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2e9db-110">String</span></span>|<span data-ttu-id="2e9db-111">Die Gruppen-ID, die das Ziel der Zuweisung ist.</span><span class="sxs-lookup"><span data-stu-id="2e9db-111">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e9db-112">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2e9db-112">Relationships</span></span>
<span data-ttu-id="2e9db-113">Keine</span><span class="sxs-lookup"><span data-stu-id="2e9db-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2e9db-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2e9db-114">JSON Representation</span></span>
<span data-ttu-id="2e9db-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2e9db-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupAssignmentTarget",
  "groupId": "String"
}
```



