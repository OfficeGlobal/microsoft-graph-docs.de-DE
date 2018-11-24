# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="8b753-101">vppLicensingType-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8b753-101">vppLicensingType resource type</span></span>

> <span data-ttu-id="8b753-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8b753-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8b753-103">Enthält Eigenschaften für den iOS-Volume-Purchased Programm (Vpp)-Lizenzierungstyp.</span><span class="sxs-lookup"><span data-stu-id="8b753-103">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>
## <a name="properties"></a><span data-ttu-id="8b753-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8b753-104">Properties</span></span>
|<span data-ttu-id="8b753-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8b753-105">Property</span></span>|<span data-ttu-id="8b753-106">Typ</span><span class="sxs-lookup"><span data-stu-id="8b753-106">Type</span></span>|<span data-ttu-id="8b753-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8b753-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b753-108">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="8b753-108">supportsUserLicensing</span></span>|<span data-ttu-id="8b753-109">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8b753-109">Boolean</span></span>|<span data-ttu-id="8b753-110">Gibt an, ob das Programm den Benutzerlizenzierungstyp unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8b753-110">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="8b753-111">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="8b753-111">supportsDeviceLicensing</span></span>|<span data-ttu-id="8b753-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8b753-112">Boolean</span></span>|<span data-ttu-id="8b753-113">Gibt an, ob das Programm den Gerätelizenzierungstyp unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8b753-113">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b753-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8b753-114">Relationships</span></span>
<span data-ttu-id="8b753-115">Keine</span><span class="sxs-lookup"><span data-stu-id="8b753-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8b753-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8b753-116">JSON Representation</span></span>
<span data-ttu-id="8b753-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8b753-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```



