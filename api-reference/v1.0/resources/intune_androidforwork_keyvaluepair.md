# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="d0873-101">keyValuePair-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d0873-101">keyValuePair resource type</span></span>

> <span data-ttu-id="d0873-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d0873-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d0873-103">Schlüssel-Wert-Paar zum Speichern benutzerdefinierter Einstellungen</span><span class="sxs-lookup"><span data-stu-id="d0873-103">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="d0873-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d0873-104">Properties</span></span>
|<span data-ttu-id="d0873-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d0873-105">Property</span></span>|<span data-ttu-id="d0873-106">Typ</span><span class="sxs-lookup"><span data-stu-id="d0873-106">Type</span></span>|<span data-ttu-id="d0873-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d0873-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0873-108">name</span><span class="sxs-lookup"><span data-stu-id="d0873-108">name</span></span>|<span data-ttu-id="d0873-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d0873-109">String</span></span>|<span data-ttu-id="d0873-110">Name für dieses Schlüssel-Wert-Paar</span><span class="sxs-lookup"><span data-stu-id="d0873-110">Name for this key-value pair</span></span>|
|<span data-ttu-id="d0873-111">Wert</span><span class="sxs-lookup"><span data-stu-id="d0873-111">value</span></span>|<span data-ttu-id="d0873-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d0873-112">String</span></span>|<span data-ttu-id="d0873-113">Wert für dieses Schlüssel-Wert-Paar</span><span class="sxs-lookup"><span data-stu-id="d0873-113">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0873-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d0873-114">Relationships</span></span>
<span data-ttu-id="d0873-115">Keine</span><span class="sxs-lookup"><span data-stu-id="d0873-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d0873-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d0873-116">JSON Representation</span></span>
<span data-ttu-id="d0873-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d0873-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.keyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValuePair",
  "name": "String",
  "value": "String"
}
```



