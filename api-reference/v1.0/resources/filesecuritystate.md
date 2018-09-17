# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="e2358-101">Ressourcentyp fileSecurityState</span><span class="sxs-lookup"><span data-stu-id="e2358-101">fileSecurityState resource type</span></span>

<span data-ttu-id="e2358-102">Enthält Informationen über die Datei (nicht den Vorgang) im Zusammenhang mit der Warnung.</span><span class="sxs-lookup"><span data-stu-id="e2358-102">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="e2358-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e2358-103">Properties</span></span>

| <span data-ttu-id="e2358-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e2358-104">Property</span></span>   | <span data-ttu-id="e2358-105">Typ</span><span class="sxs-lookup"><span data-stu-id="e2358-105">Type</span></span>|<span data-ttu-id="e2358-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e2358-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2358-107">fileHash</span><span class="sxs-lookup"><span data-stu-id="e2358-107">fileHash</span></span>|[<span data-ttu-id="e2358-108">fileHash</span><span class="sxs-lookup"><span data-stu-id="e2358-108">fileHash</span></span>](filehash.md)|<span data-ttu-id="e2358-109">Komplexer Typ mit Datei-Hashes (kryptographisch und der ortsabhängig).</span><span class="sxs-lookup"><span data-stu-id="e2358-109">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="e2358-110">Name</span><span class="sxs-lookup"><span data-stu-id="e2358-110">name</span></span>|<span data-ttu-id="e2358-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e2358-111">String</span></span>|<span data-ttu-id="e2358-112">Der Dateiname (ohne Pfad).</span><span class="sxs-lookup"><span data-stu-id="e2358-112">File name (without path).</span></span>|
|<span data-ttu-id="e2358-113">Pfad</span><span class="sxs-lookup"><span data-stu-id="e2358-113">path</span></span>|<span data-ttu-id="e2358-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e2358-114">String</span></span>|<span data-ttu-id="e2358-115">Dateiname (ohne Pfad)</span><span class="sxs-lookup"><span data-stu-id="e2358-115">Full file path of the stencil file</span></span>|
|<span data-ttu-id="e2358-116">riskScore</span><span class="sxs-lookup"><span data-stu-id="e2358-116">riskScore</span></span>|<span data-ttu-id="e2358-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e2358-117">String</span></span>|<span data-ttu-id="e2358-118">Vom Anbieter generierte/berechnete Risikobewertung der Warnungs-Datei.</span><span class="sxs-lookup"><span data-stu-id="e2358-118">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="e2358-119">Empfohlener Wertebereich von 0-1, was einem Prozentsatz entspricht.</span><span class="sxs-lookup"><span data-stu-id="e2358-119">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e2358-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e2358-120">JSON representation</span></span>

<span data-ttu-id="e2358-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e2358-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileSecurityState"
}-->

```json
{
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "name": "String",
  "path": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->