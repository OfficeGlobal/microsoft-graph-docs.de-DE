# <a name="profilephoto-resource-type"></a><span data-ttu-id="cbba1-101">profilePhoto-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="cbba1-101">profilePhoto resource type</span></span>
<span data-ttu-id="cbba1-p101">Ein Profilfoto eines Benutzers, einer Gruppe oder eines Outlook-Kontakts, auf den bzw. die von Exchange Online zugegriffen wird. Es handelt sich um Binärdaten, die nicht in Base-64 codiert sind.</span><span class="sxs-lookup"><span data-stu-id="cbba1-p101">A profile photo of a user, group or an Outlook contact accessed from Exchange Online. It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="cbba1-104">Die unterstützten Größen der HD-Fotos auf Exchange Online sind wie folgt: „48x48“, „64x64“, „96x96“, „120x120“, „240x240“, „360x360“,“432x432“, „504x504“ und „648x648“.</span><span class="sxs-lookup"><span data-stu-id="cbba1-104">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> 

## <a name="methods"></a><span data-ttu-id="cbba1-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="cbba1-105">Methods</span></span>

| <span data-ttu-id="cbba1-106">Methode</span><span class="sxs-lookup"><span data-stu-id="cbba1-106">Method</span></span>       | <span data-ttu-id="cbba1-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="cbba1-107">Return Type</span></span>  |<span data-ttu-id="cbba1-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cbba1-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cbba1-109">profilePhoto abrufen</span><span class="sxs-lookup"><span data-stu-id="cbba1-109">Get profilePhoto</span></span>](../api/profilephoto_get.md) | [<span data-ttu-id="cbba1-110">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="cbba1-110">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="cbba1-111">Ruft das angegebene **profilePhoto** oder seine Metadaten (profilePhoto-Eigenschaften) ab.</span><span class="sxs-lookup"><span data-stu-id="cbba1-111">Get the specified **profilePhoto** or its metadata (profilePhoto properties).</span></span>|
|[<span data-ttu-id="cbba1-112">Update</span><span class="sxs-lookup"><span data-stu-id="cbba1-112">Update</span></span>](../api/profilephoto_update.md) | [<span data-ttu-id="cbba1-113">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="cbba1-113">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="cbba1-p102">Weist dem angegebenen Benutzer, der angegebenen Gruppe oder dem angegebenen Kontakt ein Foto zu. Das Foto sollte binär sein. Es ersetzt vorhandene Fotos (falls vorhanden).</span><span class="sxs-lookup"><span data-stu-id="cbba1-p102">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span>|

## <a name="properties"></a><span data-ttu-id="cbba1-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cbba1-117">Properties</span></span>
| <span data-ttu-id="cbba1-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cbba1-118">Property</span></span>     | <span data-ttu-id="cbba1-119">Typ</span><span class="sxs-lookup"><span data-stu-id="cbba1-119">Type</span></span>   |<span data-ttu-id="cbba1-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cbba1-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cbba1-121">id</span><span class="sxs-lookup"><span data-stu-id="cbba1-121">id</span></span>|<span data-ttu-id="cbba1-122">string</span><span class="sxs-lookup"><span data-stu-id="cbba1-122">string</span></span>|<span data-ttu-id="cbba1-123">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cbba1-123">Read-only.</span></span>|
|<span data-ttu-id="cbba1-124">height</span><span class="sxs-lookup"><span data-stu-id="cbba1-124">height</span></span>|<span data-ttu-id="cbba1-125">int32</span><span class="sxs-lookup"><span data-stu-id="cbba1-125">int32</span></span>|<span data-ttu-id="cbba1-p103">Die Höhe des Fotos. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cbba1-p103">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="cbba1-128">width</span><span class="sxs-lookup"><span data-stu-id="cbba1-128">width</span></span>|<span data-ttu-id="cbba1-129">int32</span><span class="sxs-lookup"><span data-stu-id="cbba1-129">int32</span></span>|<span data-ttu-id="cbba1-p104">Die Breite des Fotos. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cbba1-p104">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cbba1-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="cbba1-132">Relationships</span></span>
<span data-ttu-id="cbba1-133">Keine</span><span class="sxs-lookup"><span data-stu-id="cbba1-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="cbba1-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cbba1-134">JSON representation</span></span>

<span data-ttu-id="cbba1-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cbba1-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.profilePhoto"
}-->

```json
{
  "id": "240X240",
  "height": 240,
  "width": 240
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profilePhoto resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
