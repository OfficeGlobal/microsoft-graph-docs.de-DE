# <a name="resourceaction-resource-type"></a><span data-ttu-id="df138-101">resourceAction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="df138-101">resourceAction resource type</span></span>

> <span data-ttu-id="df138-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="df138-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df138-103">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="df138-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="df138-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="df138-104">Properties</span></span>
|<span data-ttu-id="df138-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="df138-105">Property</span></span>|<span data-ttu-id="df138-106">Typ</span><span class="sxs-lookup"><span data-stu-id="df138-106">Type</span></span>|<span data-ttu-id="df138-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="df138-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df138-108">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="df138-108">allowedResourceActions</span></span>|<span data-ttu-id="df138-109">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="df138-109">String collection</span></span>|<span data-ttu-id="df138-110">Zulässige Aktionen</span><span class="sxs-lookup"><span data-stu-id="df138-110">Allowed Actions</span></span>|
|<span data-ttu-id="df138-111">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="df138-111">notAllowedResourceActions</span></span>|<span data-ttu-id="df138-112">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="df138-112">String collection</span></span>|<span data-ttu-id="df138-113">Nicht zulässige Aktionen</span><span class="sxs-lookup"><span data-stu-id="df138-113">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="df138-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="df138-114">Relationships</span></span>
<span data-ttu-id="df138-115">Keine</span><span class="sxs-lookup"><span data-stu-id="df138-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="df138-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="df138-116">JSON Representation</span></span>
<span data-ttu-id="df138-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="df138-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```



