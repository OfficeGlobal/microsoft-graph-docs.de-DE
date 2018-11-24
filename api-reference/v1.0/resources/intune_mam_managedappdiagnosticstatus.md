# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="2bd48-101">managedAppDiagnosticStatus-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2bd48-101">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="2bd48-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2bd48-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2bd48-103">Stellt den Diagnosestatus dar.</span><span class="sxs-lookup"><span data-stu-id="2bd48-103">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="2bd48-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2bd48-104">Properties</span></span>
|<span data-ttu-id="2bd48-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2bd48-105">Property</span></span>|<span data-ttu-id="2bd48-106">Typ</span><span class="sxs-lookup"><span data-stu-id="2bd48-106">Type</span></span>|<span data-ttu-id="2bd48-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2bd48-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bd48-108">validationName</span><span class="sxs-lookup"><span data-stu-id="2bd48-108">validationName</span></span>|<span data-ttu-id="2bd48-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2bd48-109">String</span></span>|<span data-ttu-id="2bd48-110">Der leicht zu prüfende Name</span><span class="sxs-lookup"><span data-stu-id="2bd48-110">The validation friendly name</span></span>|
|<span data-ttu-id="2bd48-111">state</span><span class="sxs-lookup"><span data-stu-id="2bd48-111">state</span></span>|<span data-ttu-id="2bd48-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2bd48-112">String</span></span>|<span data-ttu-id="2bd48-113">Der Status des Vorgangs</span><span class="sxs-lookup"><span data-stu-id="2bd48-113">The state of the operation</span></span>|
|<span data-ttu-id="2bd48-114">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="2bd48-114">mitigationInstruction</span></span>|<span data-ttu-id="2bd48-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2bd48-115">String</span></span>|<span data-ttu-id="2bd48-116">Anweisungen zum Umgehen einer fehlgeschlagenen Validierung</span><span class="sxs-lookup"><span data-stu-id="2bd48-116">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="2bd48-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2bd48-117">Relationships</span></span>
<span data-ttu-id="2bd48-118">Keine</span><span class="sxs-lookup"><span data-stu-id="2bd48-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2bd48-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2bd48-119">JSON Representation</span></span>
<span data-ttu-id="2bd48-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2bd48-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppDiagnosticStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppDiagnosticStatus",
  "validationName": "String",
  "state": "String",
  "mitigationInstruction": "String"
}
```



