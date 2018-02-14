# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="d25c6-101">exclusionGroupAssignmentTarget-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d25c6-101">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="d25c6-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d25c6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d25c6-103">Steht für eine Gruppe, die aus einer Zuweisung ausgeschlossen werden sollte.</span><span class="sxs-lookup"><span data-stu-id="d25c6-103">Represents a group that should be excluded from an assignment.</span></span>

<span data-ttu-id="d25c6-104">Erbt von [groupAssignmentTarget](../resources/intune_onboarding_groupassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="d25c6-104">Inherits from [groupAssignmentTarget](../resources/intune_onboarding_groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d25c6-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d25c6-105">Properties</span></span>
|<span data-ttu-id="d25c6-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d25c6-106">Property</span></span>|<span data-ttu-id="d25c6-107">Typ</span><span class="sxs-lookup"><span data-stu-id="d25c6-107">Type</span></span>|<span data-ttu-id="d25c6-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d25c6-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d25c6-109">groupId</span><span class="sxs-lookup"><span data-stu-id="d25c6-109">groupId</span></span>|<span data-ttu-id="d25c6-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d25c6-110">String</span></span>|<span data-ttu-id="d25c6-111">Die Gruppen-ID, die das Ziel der Zuweisung ist.</span><span class="sxs-lookup"><span data-stu-id="d25c6-111">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="d25c6-112">Vererbt von [groupAssignmentTarget](../resources/intune_onboarding_groupassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="d25c6-112">Inherited from [groupAssignmentTarget](../resources/intune_onboarding_groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="d25c6-113">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d25c6-113">Relationships</span></span>
<span data-ttu-id="d25c6-114">Keine</span><span class="sxs-lookup"><span data-stu-id="d25c6-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d25c6-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d25c6-115">JSON Representation</span></span>
<span data-ttu-id="d25c6-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d25c6-116">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.exclusionGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exclusionGroupAssignmentTarget",
  "groupId": "String"
}
```



