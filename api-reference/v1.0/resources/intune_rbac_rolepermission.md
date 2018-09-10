# <a name="rolepermission-resource-type"></a><span data-ttu-id="2da11-101">rolePermission-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2da11-101">rolePermission resource type</span></span>

> <span data-ttu-id="2da11-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2da11-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2da11-103">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="2da11-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="2da11-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2da11-104">Properties</span></span>
|<span data-ttu-id="2da11-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2da11-105">Property</span></span>|<span data-ttu-id="2da11-106">Typ</span><span class="sxs-lookup"><span data-stu-id="2da11-106">Type</span></span>|<span data-ttu-id="2da11-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2da11-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2da11-108">resourceActions</span><span class="sxs-lookup"><span data-stu-id="2da11-108">resourceActions</span></span>|<span data-ttu-id="2da11-109">[resourceAction](../resources/intune_rbac_resourceaction.md)-Auflistung</span><span class="sxs-lookup"><span data-stu-id="2da11-109">[resourceAction](../resources/intune_rbac_resourceaction.md) collection</span></span>|<span data-ttu-id="2da11-110">Aktionen</span><span class="sxs-lookup"><span data-stu-id="2da11-110">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="2da11-111">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2da11-111">Relationships</span></span>
<span data-ttu-id="2da11-112">Keine</span><span class="sxs-lookup"><span data-stu-id="2da11-112">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2da11-113">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2da11-113">JSON Representation</span></span>
<span data-ttu-id="2da11-114">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2da11-114">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rolePermission"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.rolePermission",
  "resourceActions": [
    {
      "@odata.type": "microsoft.graph.resourceAction",
      "allowedResourceActions": [
        "String"
      ],
      "notAllowedResourceActions": [
        "String"
      ]
    }
  ]
}
```








