# <a name="auditresource-resource-type"></a><span data-ttu-id="67f93-101">auditResource-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="67f93-101">auditResource resource type</span></span>

> <span data-ttu-id="67f93-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="67f93-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="67f93-103">Eine Klasse, die die Eigenschaften für die Audit-Ressource enthält.</span><span class="sxs-lookup"><span data-stu-id="67f93-103">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="67f93-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="67f93-104">Properties</span></span>
|<span data-ttu-id="67f93-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="67f93-105">Property</span></span>|<span data-ttu-id="67f93-106">Typ</span><span class="sxs-lookup"><span data-stu-id="67f93-106">Type</span></span>|<span data-ttu-id="67f93-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="67f93-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67f93-108">displayName</span><span class="sxs-lookup"><span data-stu-id="67f93-108">displayName</span></span>|<span data-ttu-id="67f93-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="67f93-109">String</span></span>|<span data-ttu-id="67f93-110">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="67f93-110">Display name.</span></span>|
|<span data-ttu-id="67f93-111">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="67f93-111">modifiedProperties</span></span>|<span data-ttu-id="67f93-112">[auditProperty](../resources/intune_auditing_auditproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="67f93-112">[auditProperty](../resources/intune_auditing_auditproperty.md) collection</span></span>|<span data-ttu-id="67f93-113">Liste der geänderten Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="67f93-113">List of modified properties.</span></span>|
|<span data-ttu-id="67f93-114">Typ</span><span class="sxs-lookup"><span data-stu-id="67f93-114">type</span></span>|<span data-ttu-id="67f93-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="67f93-115">String</span></span>|<span data-ttu-id="67f93-116">Typ der Audit-Ressource</span><span class="sxs-lookup"><span data-stu-id="67f93-116">Audit resource's type.</span></span>|
|<span data-ttu-id="67f93-117">resourceId</span><span class="sxs-lookup"><span data-stu-id="67f93-117">resourceId</span></span>|<span data-ttu-id="67f93-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="67f93-118">String</span></span>|<span data-ttu-id="67f93-119">ID der Audit-Ressource</span><span class="sxs-lookup"><span data-stu-id="67f93-119">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="67f93-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="67f93-120">Relationships</span></span>
<span data-ttu-id="67f93-121">Keine</span><span class="sxs-lookup"><span data-stu-id="67f93-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="67f93-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="67f93-122">JSON Representation</span></span>
<span data-ttu-id="67f93-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="67f93-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
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



