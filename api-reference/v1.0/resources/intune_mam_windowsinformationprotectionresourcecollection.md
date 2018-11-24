# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="ff50e-101">windowsInformationProtectionResourceCollection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ff50e-101">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="ff50e-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ff50e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff50e-103">Windows Information Protection – Ressourcensammlung</span><span class="sxs-lookup"><span data-stu-id="ff50e-103">Windows Information Protection Resource Collection</span></span>
## <a name="properties"></a><span data-ttu-id="ff50e-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ff50e-104">Properties</span></span>
|<span data-ttu-id="ff50e-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ff50e-105">Property</span></span>|<span data-ttu-id="ff50e-106">Typ</span><span class="sxs-lookup"><span data-stu-id="ff50e-106">Type</span></span>|<span data-ttu-id="ff50e-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ff50e-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff50e-108">displayName</span><span class="sxs-lookup"><span data-stu-id="ff50e-108">displayName</span></span>|<span data-ttu-id="ff50e-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ff50e-109">String</span></span>|<span data-ttu-id="ff50e-110">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="ff50e-110">Display name</span></span>|
|<span data-ttu-id="ff50e-111">Ressourcen</span><span class="sxs-lookup"><span data-stu-id="ff50e-111">resources</span></span>|<span data-ttu-id="ff50e-112">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="ff50e-112">String collection</span></span>|<span data-ttu-id="ff50e-113">Sammlung von Ressourcen</span><span class="sxs-lookup"><span data-stu-id="ff50e-113">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff50e-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ff50e-114">Relationships</span></span>
<span data-ttu-id="ff50e-115">Keine</span><span class="sxs-lookup"><span data-stu-id="ff50e-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ff50e-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ff50e-116">JSON Representation</span></span>
<span data-ttu-id="ff50e-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ff50e-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionResourceCollection",
  "displayName": "String",
  "resources": [
    "String"
  ]
}
```



