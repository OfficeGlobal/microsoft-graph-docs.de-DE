# <a name="auditresource-resource-type"></a><span data-ttu-id="a63de-101">auditResource-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a63de-101">auditResource resource type</span></span>

> <span data-ttu-id="a63de-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a63de-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a63de-103">Eine Klasse, die die Eigenschaften für die Audit-Ressource enthält.</span><span class="sxs-lookup"><span data-stu-id="a63de-103">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="a63de-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a63de-104">Properties</span></span>
|<span data-ttu-id="a63de-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a63de-105">Property</span></span>|<span data-ttu-id="a63de-106">Typ</span><span class="sxs-lookup"><span data-stu-id="a63de-106">Type</span></span>|<span data-ttu-id="a63de-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a63de-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a63de-108">displayName</span><span class="sxs-lookup"><span data-stu-id="a63de-108">displayName</span></span>|<span data-ttu-id="a63de-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a63de-109">String</span></span>|<span data-ttu-id="a63de-110">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="a63de-110">Display Name</span></span>|
|<span data-ttu-id="a63de-111">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="a63de-111">modifiedProperties</span></span>|<span data-ttu-id="a63de-112">[auditProperty](../resources/intune_auditing_auditproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a63de-112">[auditProperty](../resources/intune_auditing_auditproperty.md) collection</span></span>|<span data-ttu-id="a63de-113">Liste der geänderten Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a63de-113">List of managed properties</span></span>|
|<span data-ttu-id="a63de-114">Typ</span><span class="sxs-lookup"><span data-stu-id="a63de-114">type</span></span>|<span data-ttu-id="a63de-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a63de-115">String</span></span>|<span data-ttu-id="a63de-116">Typ der Audit-Ressource</span><span class="sxs-lookup"><span data-stu-id="a63de-116">Audit resource's type.</span></span>|
|<span data-ttu-id="a63de-117">resourceId</span><span class="sxs-lookup"><span data-stu-id="a63de-117">resourceId</span></span>|<span data-ttu-id="a63de-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a63de-118">String</span></span>|<span data-ttu-id="a63de-119">ID der Audit-Ressource</span><span class="sxs-lookup"><span data-stu-id="a63de-119">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a63de-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a63de-120">Relationships</span></span>
<span data-ttu-id="a63de-121">Keine</span><span class="sxs-lookup"><span data-stu-id="a63de-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a63de-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a63de-122">JSON Representation</span></span>
<span data-ttu-id="a63de-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a63de-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.auditResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditResource",
  "displayName": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.auditProperty",
      "displayName": "String",
      "oldValue": "String",
      "newValue": "String"
    }
  ],
  "type": "String",
  "resourceId": "String"
}
```



