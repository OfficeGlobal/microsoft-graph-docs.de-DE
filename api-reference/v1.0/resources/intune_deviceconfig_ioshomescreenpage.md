# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="2757c-101">iosHomeScreenPage-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2757c-101">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="2757c-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2757c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2757c-103">Eine Seite mit Apps und Ordnern auf der Startseite.</span><span class="sxs-lookup"><span data-stu-id="2757c-103">A page containing apps and folders on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="2757c-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2757c-104">Properties</span></span>
|<span data-ttu-id="2757c-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2757c-105">Property</span></span>|<span data-ttu-id="2757c-106">Typ</span><span class="sxs-lookup"><span data-stu-id="2757c-106">Type</span></span>|<span data-ttu-id="2757c-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2757c-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2757c-108">displayName</span><span class="sxs-lookup"><span data-stu-id="2757c-108">displayName</span></span>|<span data-ttu-id="2757c-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2757c-109">String</span></span>|<span data-ttu-id="2757c-110">Name der Seite</span><span class="sxs-lookup"><span data-stu-id="2757c-110">Name of the page</span></span>|
|<span data-ttu-id="2757c-111">Symbole</span><span class="sxs-lookup"><span data-stu-id="2757c-111">icons</span></span>|<span data-ttu-id="2757c-112">[iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="2757c-112">[iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="2757c-113">Eine Liste der Apps und Ordner, die auf einer Seite angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="2757c-113">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="2757c-114">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="2757c-114">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2757c-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2757c-115">Relationships</span></span>
<span data-ttu-id="2757c-116">Keine</span><span class="sxs-lookup"><span data-stu-id="2757c-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2757c-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2757c-117">JSON Representation</span></span>
<span data-ttu-id="2757c-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2757c-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenPage",
  "displayName": "String",
  "icons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenItem",
      "displayName": "String",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "String",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "String",
              "bundleID": "String"
            }
          ]
        }
      ]
    }
  ]
}
```



