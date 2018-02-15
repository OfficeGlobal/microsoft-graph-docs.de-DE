# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="24105-101">iosHomeScreenItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="24105-101">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="24105-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="24105-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="24105-103">Stellt ein Element auf dem iOS-Startbildschirm dar.</span><span class="sxs-lookup"><span data-stu-id="24105-103">Represents an item on the iOS Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="24105-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="24105-104">Properties</span></span>
|<span data-ttu-id="24105-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="24105-105">Property</span></span>|<span data-ttu-id="24105-106">Typ</span><span class="sxs-lookup"><span data-stu-id="24105-106">Type</span></span>|<span data-ttu-id="24105-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="24105-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24105-108">displayName</span><span class="sxs-lookup"><span data-stu-id="24105-108">displayName</span></span>|<span data-ttu-id="24105-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="24105-109">String</span></span>|<span data-ttu-id="24105-110">Name der App</span><span class="sxs-lookup"><span data-stu-id="24105-110">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="24105-111">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="24105-111">Relationships</span></span>
<span data-ttu-id="24105-112">Keine</span><span class="sxs-lookup"><span data-stu-id="24105-112">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="24105-113">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="24105-113">JSON Representation</span></span>
<span data-ttu-id="24105-114">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="24105-114">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosHomeScreenItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenItem",
  "displayName": "String"
}
```



