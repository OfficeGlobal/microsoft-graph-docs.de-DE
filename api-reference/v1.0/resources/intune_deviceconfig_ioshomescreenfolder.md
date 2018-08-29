# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="7a6ca-101">iosHomeScreenFolder-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7a6ca-101">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="7a6ca-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7a6ca-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7a6ca-103">Ein Ordner mit App-Seiten auf der Startseite</span><span class="sxs-lookup"><span data-stu-id="7a6ca-103">A folder containing pages of apps on the Home Screen</span></span>

<span data-ttu-id="7a6ca-104">Erbt von [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="7a6ca-104">Inherits from [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7a6ca-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7a6ca-105">Properties</span></span>
|<span data-ttu-id="7a6ca-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7a6ca-106">Property</span></span>|<span data-ttu-id="7a6ca-107">Typ</span><span class="sxs-lookup"><span data-stu-id="7a6ca-107">Type</span></span>|<span data-ttu-id="7a6ca-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7a6ca-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a6ca-109">displayName</span><span class="sxs-lookup"><span data-stu-id="7a6ca-109">displayName</span></span>|<span data-ttu-id="7a6ca-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7a6ca-110">String</span></span>|<span data-ttu-id="7a6ca-111">Name der von [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md) geerbten App</span><span class="sxs-lookup"><span data-stu-id="7a6ca-111">Name of the app Inherited from [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="7a6ca-112">Seiten</span><span class="sxs-lookup"><span data-stu-id="7a6ca-112">pages</span></span>|<span data-ttu-id="7a6ca-113">[iosHomeScreenFolderPage](../resources/intune_deviceconfig_ioshomescreenfolderpage.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="7a6ca-113">[iosHomeScreenFolderPage](../resources/intune_deviceconfig_ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="7a6ca-114">Seiten mit Startbildschirm-Layout-Symbolen, die dem Anwendungstyp entsprechen müssen.</span><span class="sxs-lookup"><span data-stu-id="7a6ca-114">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="7a6ca-115">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="7a6ca-115">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a6ca-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7a6ca-116">Relationships</span></span>
<span data-ttu-id="7a6ca-117">Keine</span><span class="sxs-lookup"><span data-stu-id="7a6ca-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7a6ca-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7a6ca-118">JSON Representation</span></span>
<span data-ttu-id="7a6ca-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7a6ca-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.iosHomeScreenItem",
  "@odata.type": "microsoft.graph.iosHomeScreenFolder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolder",
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
```



