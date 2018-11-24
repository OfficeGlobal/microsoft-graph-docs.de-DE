# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="fd4da-101">keyValuePair-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fd4da-101">keyValuePair resource type</span></span>

> <span data-ttu-id="fd4da-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fd4da-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd4da-103">Schlüssel-Wert-Paar zum Speichern benutzerdefinierter Einstellungen</span><span class="sxs-lookup"><span data-stu-id="fd4da-103">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="fd4da-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fd4da-104">Properties</span></span>
|<span data-ttu-id="fd4da-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fd4da-105">Property</span></span>|<span data-ttu-id="fd4da-106">Typ</span><span class="sxs-lookup"><span data-stu-id="fd4da-106">Type</span></span>|<span data-ttu-id="fd4da-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd4da-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd4da-108">name</span><span class="sxs-lookup"><span data-stu-id="fd4da-108">name</span></span>|<span data-ttu-id="fd4da-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fd4da-109">String</span></span>|<span data-ttu-id="fd4da-110">Namen für dieses Schlüssel-Wert-Paar</span><span class="sxs-lookup"><span data-stu-id="fd4da-110">Name for this key-value pair</span></span>|
|<span data-ttu-id="fd4da-111">value</span><span class="sxs-lookup"><span data-stu-id="fd4da-111">value</span></span>|<span data-ttu-id="fd4da-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fd4da-112">String</span></span>|<span data-ttu-id="fd4da-113">Wert für dieses Schlüssel-Wert-Paar</span><span class="sxs-lookup"><span data-stu-id="fd4da-113">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd4da-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fd4da-114">Relationships</span></span>
<span data-ttu-id="fd4da-115">Keine</span><span class="sxs-lookup"><span data-stu-id="fd4da-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fd4da-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fd4da-116">JSON Representation</span></span>
<span data-ttu-id="fd4da-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fd4da-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
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



