# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="71505-101">groupAssignmentTarget-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="71505-101">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="71505-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="71505-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71505-103">Stellt eine Zuweisung zu einer Gruppe dar.</span><span class="sxs-lookup"><span data-stu-id="71505-103">Represents an assignment to a group.</span></span>

<span data-ttu-id="71505-104">Erbt von [deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="71505-104">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="71505-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="71505-105">Properties</span></span>
|<span data-ttu-id="71505-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="71505-106">Property</span></span>|<span data-ttu-id="71505-107">Typ</span><span class="sxs-lookup"><span data-stu-id="71505-107">Type</span></span>|<span data-ttu-id="71505-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71505-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71505-109">groupId</span><span class="sxs-lookup"><span data-stu-id="71505-109">groupId</span></span>|<span data-ttu-id="71505-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="71505-110">String</span></span>|<span data-ttu-id="71505-111">Die Gruppen-ID, die das Ziel der Zuweisung ist.</span><span class="sxs-lookup"><span data-stu-id="71505-111">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71505-112">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="71505-112">Relationships</span></span>
<span data-ttu-id="71505-113">Keine</span><span class="sxs-lookup"><span data-stu-id="71505-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="71505-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="71505-114">JSON Representation</span></span>
<span data-ttu-id="71505-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="71505-115">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
  "@odata.type": "microsoft.graph.groupAssignmentTarget"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.groupAssignmentTarget",
  "groupId": "String"
}
```



