# <a name="mimecontent-resource-type"></a><span data-ttu-id="0e657-101">mimeContent-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0e657-101">mimeContent resource type</span></span>

> <span data-ttu-id="0e657-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0e657-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0e657-103">Enthält die Eigenschaften für generischen MIME-Inhalt.</span><span class="sxs-lookup"><span data-stu-id="0e657-103">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="0e657-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0e657-104">Properties</span></span>
|<span data-ttu-id="0e657-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0e657-105">Property</span></span>|<span data-ttu-id="0e657-106">Typ</span><span class="sxs-lookup"><span data-stu-id="0e657-106">Type</span></span>|<span data-ttu-id="0e657-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e657-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e657-108">type</span><span class="sxs-lookup"><span data-stu-id="0e657-108">type</span></span>|<span data-ttu-id="0e657-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0e657-109">String</span></span>|<span data-ttu-id="0e657-110">Gibt den MIME-Typ des Inhalts an.</span><span class="sxs-lookup"><span data-stu-id="0e657-110">Indicates the content mime type.</span></span>|
|<span data-ttu-id="0e657-111">Wert</span><span class="sxs-lookup"><span data-stu-id="0e657-111">value</span></span>|<span data-ttu-id="0e657-112">Binär</span><span class="sxs-lookup"><span data-stu-id="0e657-112">Binary</span></span>|<span data-ttu-id="0e657-113">Das Bytearray, das den tatsächlichen Inhalt enthält.</span><span class="sxs-lookup"><span data-stu-id="0e657-113">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e657-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0e657-114">Relationships</span></span>
<span data-ttu-id="0e657-115">Keine</span><span class="sxs-lookup"><span data-stu-id="0e657-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0e657-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0e657-116">JSON Representation</span></span>
<span data-ttu-id="0e657-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0e657-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mimeContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mimeContent",
  "type": "String",
  "value": "binary"
}
```



