# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="f8547-101">iosHomeScreenFolderPage-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f8547-101">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="f8547-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f8547-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8547-103">Ein Ordner mit Apps auf der Startseite</span><span class="sxs-lookup"><span data-stu-id="f8547-103">A folder containing apps on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="f8547-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f8547-104">Properties</span></span>
|<span data-ttu-id="f8547-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f8547-105">Property</span></span>|<span data-ttu-id="f8547-106">Typ</span><span class="sxs-lookup"><span data-stu-id="f8547-106">Type</span></span>|<span data-ttu-id="f8547-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8547-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8547-108">displayName</span><span class="sxs-lookup"><span data-stu-id="f8547-108">displayName</span></span>|<span data-ttu-id="f8547-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f8547-109">String</span></span>|<span data-ttu-id="f8547-110">Name des Ordnerseite</span><span class="sxs-lookup"><span data-stu-id="f8547-110">Name of the folder page</span></span>|
|<span data-ttu-id="f8547-111">Apps</span><span class="sxs-lookup"><span data-stu-id="f8547-111">apps</span></span>|<span data-ttu-id="f8547-112">[iosHomeScreenApp](../resources/intune_deviceconfig_ioshomescreenapp.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f8547-112">[iosHomeScreenApp](../resources/intune_deviceconfig_ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="f8547-113">Eine Liste der Apps, die auf einer Seite innerhalb eines Ordners angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="f8547-113">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="f8547-114">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="f8547-114">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8547-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f8547-115">Relationships</span></span>
<span data-ttu-id="f8547-116">Keine</span><span class="sxs-lookup"><span data-stu-id="f8547-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f8547-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f8547-117">JSON Representation</span></span>
<span data-ttu-id="f8547-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f8547-118">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolderPage"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolderPage",
  "displayName": "String",
  "apps": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenApp",
      "displayName": "String",
      "bundleID": "String"
    }
  ]
}
```








