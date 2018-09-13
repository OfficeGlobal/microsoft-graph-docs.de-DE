# <a name="filehash-resource-type"></a><span data-ttu-id="21a2a-101">Ressourcentyp fileHash</span><span class="sxs-lookup"><span data-stu-id="21a2a-101">fileHash resource type</span></span>

<span data-ttu-id="21a2a-102">Enthält Statusinformationen zu Dateihashes (kryptographisch und ortsabhängig).</span><span class="sxs-lookup"><span data-stu-id="21a2a-102">Contains stateful information about file hashes (cryptographic and location-sensitive).</span></span>

## <a name="properties"></a><span data-ttu-id="21a2a-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="21a2a-103">Properties</span></span>

| <span data-ttu-id="21a2a-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="21a2a-104">Property</span></span>     | <span data-ttu-id="21a2a-105">Typ</span><span class="sxs-lookup"><span data-stu-id="21a2a-105">Type</span></span>        | <span data-ttu-id="21a2a-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="21a2a-106">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="21a2a-107">hashType</span><span class="sxs-lookup"><span data-stu-id="21a2a-107">hashType</span></span>|<span data-ttu-id="21a2a-108">fileHashType</span><span class="sxs-lookup"><span data-stu-id="21a2a-108">fileHashType</span></span>|<span data-ttu-id="21a2a-109">Hash-Dateityp.</span><span class="sxs-lookup"><span data-stu-id="21a2a-109">File hash type.</span></span> <span data-ttu-id="21a2a-110">Mögliche Werte: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span><span class="sxs-lookup"><span data-stu-id="21a2a-110">Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span></span>|
|<span data-ttu-id="21a2a-111">hashValue</span><span class="sxs-lookup"><span data-stu-id="21a2a-111">hashValue</span></span>|<span data-ttu-id="21a2a-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21a2a-112">String</span></span>|<span data-ttu-id="21a2a-113">Der Wert des Dateihash.</span><span class="sxs-lookup"><span data-stu-id="21a2a-113">Value of the file hash.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21a2a-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="21a2a-114">JSON representation</span></span>

<span data-ttu-id="21a2a-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="21a2a-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileHash"
}-->

```json
{
  "hashType": "@odata.type: microsoft.graph.fileHashType",
  "hashValue": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileHash resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->