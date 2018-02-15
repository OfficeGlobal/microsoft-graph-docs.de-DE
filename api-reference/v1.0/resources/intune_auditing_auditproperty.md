# <a name="auditproperty-resource-type"></a><span data-ttu-id="e1233-101">auditProperty-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e1233-101">auditProperty resource type</span></span>

> <span data-ttu-id="e1233-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e1233-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1233-103">Eine Klasse, die die Eigenschaften für die Audit-Eigenschaft enthält.</span><span class="sxs-lookup"><span data-stu-id="e1233-103">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="e1233-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e1233-104">Properties</span></span>
|<span data-ttu-id="e1233-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e1233-105">Property</span></span>|<span data-ttu-id="e1233-106">Typ</span><span class="sxs-lookup"><span data-stu-id="e1233-106">Type</span></span>|<span data-ttu-id="e1233-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e1233-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1233-108">displayName</span><span class="sxs-lookup"><span data-stu-id="e1233-108">displayName</span></span>|<span data-ttu-id="e1233-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e1233-109">String</span></span>|<span data-ttu-id="e1233-110">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="e1233-110">Display Name</span></span>|
|<span data-ttu-id="e1233-111">oldValue</span><span class="sxs-lookup"><span data-stu-id="e1233-111">OldValue</span></span>|<span data-ttu-id="e1233-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e1233-112">String</span></span>|<span data-ttu-id="e1233-113">Alter Wert</span><span class="sxs-lookup"><span data-stu-id="e1233-113">Old value.</span></span>|
|<span data-ttu-id="e1233-114">newValue</span><span class="sxs-lookup"><span data-stu-id="e1233-114">newvalue</span></span>|<span data-ttu-id="e1233-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e1233-115">String</span></span>|<span data-ttu-id="e1233-116">Neuer Wert</span><span class="sxs-lookup"><span data-stu-id="e1233-116">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1233-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e1233-117">Relationships</span></span>
<span data-ttu-id="e1233-118">Keine</span><span class="sxs-lookup"><span data-stu-id="e1233-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e1233-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e1233-119">JSON Representation</span></span>
<span data-ttu-id="e1233-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e1233-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.auditProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditProperty",
  "displayName": "String",
  "oldValue": "String",
  "newValue": "String"
}
```



