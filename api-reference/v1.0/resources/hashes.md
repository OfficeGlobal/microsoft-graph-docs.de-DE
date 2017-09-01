# <a name="hashes-resource-type"></a><span data-ttu-id="e2843-101">Hash-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e2843-101">Hashes resource type</span></span>

<span data-ttu-id="e2843-102">Die **Hashes**-Ressourcengruppen machen Hashes in einer einzelnen Struktur für ein Element verfügbar.</span><span class="sxs-lookup"><span data-stu-id="e2843-102">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="e2843-103">**Hinweis:** Nicht alle Dienste geben einen Wert für alle aufgeführten Hash-Eigenschaften an.</span><span class="sxs-lookup"><span data-stu-id="e2843-103">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2843-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e2843-104">JSON representation</span></span>

<span data-ttu-id="e2843-105">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e2843-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "sha1Hash", "crc32Hash", "quickXorHash" ],
  "@odata.type": "microsoft.graph.hashes"
}-->

```json
{
  "crc32Hash": "string",
  "sha1Hash": "string",
  "quickXorHash": "string"
}
```


## <a name="properties"></a><span data-ttu-id="e2843-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e2843-106">Properties</span></span>

| <span data-ttu-id="e2843-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e2843-107">Property</span></span>         | <span data-ttu-id="e2843-108">Typ</span><span class="sxs-lookup"><span data-stu-id="e2843-108">Type</span></span>   | <span data-ttu-id="e2843-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e2843-109">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="e2843-110">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="e2843-110">**sha1Hash**</span></span>     | <span data-ttu-id="e2843-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e2843-111">String</span></span> | <span data-ttu-id="e2843-p101">SHA1-Hash für den Inhalt der Datei (sofern zutreffend). Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e2843-p101">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="e2843-114">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="e2843-114">**crc32Hash**</span></span>    | <span data-ttu-id="e2843-115">String</span><span class="sxs-lookup"><span data-stu-id="e2843-115">String</span></span> | <span data-ttu-id="e2843-p102">Der Wert der CRC32 der Datei (sofern zutreffend). Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e2843-p102">The CRC32 value of the file (if available). Read-only.</span></span>            |
| <span data-ttu-id="e2843-118">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="e2843-118">**quickXorHash**</span></span> | <span data-ttu-id="e2843-119">String</span><span class="sxs-lookup"><span data-stu-id="e2843-119">String</span></span> | <span data-ttu-id="e2843-p103">Ein proprietärer Hash der Datei, die verwendet werden kann, um festzustellen, ob sich der Inhalt der Datei (sofern zutreffend) geändert hat. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e2843-p103">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

<span data-ttu-id="e2843-p104">**Hinweis:** In einigen Fällen stehen möglicherweise keine Hash-Werte zur Verfügung. Wenn dies der Fall ist, werden die Hash-Werte für ein Element nach dem Download des Elements aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="e2843-p104">**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>


## <a name="remarks"></a><span data-ttu-id="e2843-124">Hinweise</span><span class="sxs-lookup"><span data-stu-id="e2843-124">Remarks</span></span>

<span data-ttu-id="e2843-p105">In OneDrive for Business stehen **sha1Hash** und **crc32Hash** nicht zur Verfügung. In OneDrive Personal steht **QuickXorHash** nicht zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="e2843-p105">In OneDrive for Business, **sha1Hash** and **crc32Hash** are not available. In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="e2843-127">Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="e2843-127">For more information about the facets on a [driveItem](driveitem.md), see driveItem.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "hashes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
