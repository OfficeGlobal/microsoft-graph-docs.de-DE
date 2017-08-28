# <a name="quota-resource-type"></a><span data-ttu-id="d51e4-101">quota-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d51e4-101">Quota resource type</span></span>

<span data-ttu-id="d51e4-102">Die **quota**-Ressource enthält Details zu Leerzeichenbeschränkungen auf einer[Laufwerk](drive.md)-Ressource.</span><span class="sxs-lookup"><span data-stu-id="d51e4-102">The **quota** resource provides details about space constrains on a [Drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d51e4-103">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d51e4-103">JSON representation</span></span>

<span data-ttu-id="d51e4-104">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d51e4-104">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.quota"
}-->

```json
{
  "deleted": 1024,
  "remaining": 1024,
  "state": "normal | nearing | critical | exceeded",
  "total": 1024,
  "used": 1024
}
```

## <a name="properties"></a><span data-ttu-id="d51e4-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d51e4-105">Properties</span></span>

| <span data-ttu-id="d51e4-106">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="d51e4-106">Property name</span></span> | <span data-ttu-id="d51e4-107">Typ</span><span class="sxs-lookup"><span data-stu-id="d51e4-107">Type</span></span>   | <span data-ttu-id="d51e4-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d51e4-108">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="d51e4-109">gesamt</span><span class="sxs-lookup"><span data-stu-id="d51e4-109">total</span></span>         | <span data-ttu-id="d51e4-110">Int64</span><span class="sxs-lookup"><span data-stu-id="d51e4-110">Int64</span></span>  | <span data-ttu-id="d51e4-p101">Zulässige Speicherplatz in Byte. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d51e4-p101">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="d51e4-113">verwendet</span><span class="sxs-lookup"><span data-stu-id="d51e4-113">used</span></span>          | <span data-ttu-id="d51e4-114">Int64</span><span class="sxs-lookup"><span data-stu-id="d51e4-114">Int64</span></span>  | <span data-ttu-id="d51e4-p102">Gesamter verwendeter Speicherplatz in Byte. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d51e4-p102">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="d51e4-117">verbleibende</span><span class="sxs-lookup"><span data-stu-id="d51e4-117">remaining</span></span>     | <span data-ttu-id="d51e4-118">Int64</span><span class="sxs-lookup"><span data-stu-id="d51e4-118">Int64</span></span>  | <span data-ttu-id="d51e4-p103">Gesamter verbleibender Speicherplatz vor dem Erreichen des Speicherkontingents in Byte. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d51e4-p103">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="d51e4-121">gelöscht</span><span class="sxs-lookup"><span data-stu-id="d51e4-121">deleted</span></span>       | <span data-ttu-id="d51e4-122">Int64</span><span class="sxs-lookup"><span data-stu-id="d51e4-122">Int64</span></span>  | <span data-ttu-id="d51e4-p104">Gesamte Dateien genutzter Speicherplatz im Papierkorb in Byte. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d51e4-p104">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="d51e4-125">state</span><span class="sxs-lookup"><span data-stu-id="d51e4-125">state</span></span>         | <span data-ttu-id="d51e4-126">string</span><span class="sxs-lookup"><span data-stu-id="d51e4-126">string</span></span> | <span data-ttu-id="d51e4-p105">Wert der Enumeration, die den Zustand des Speicherplatzes angibt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d51e4-p105">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |

## <a name="state-enumeration"></a><span data-ttu-id="d51e4-129">Status Enumeration</span><span class="sxs-lookup"><span data-stu-id="d51e4-129">State Enumeration</span></span>

| <span data-ttu-id="d51e4-130">Wert</span><span class="sxs-lookup"><span data-stu-id="d51e4-130">Value</span></span>      | <span data-ttu-id="d51e4-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d51e4-131">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="d51e4-132">Das Laufwerk verfügt über ausreichend verbleibendes Kontingent.</span><span class="sxs-lookup"><span data-stu-id="d51e4-132">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="d51e4-133">Verbleibendes Kontingent weniger als 10 % des gesamten Kontingentplatzes.</span><span class="sxs-lookup"><span data-stu-id="d51e4-133">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="d51e4-134">Verbleibendes Kontingent weniger als 1 % des gesamten Kontingentplatzes.</span><span class="sxs-lookup"><span data-stu-id="d51e4-134">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="d51e4-p106">Das verwendete Kontingent hat das gesamte Kontingent überschritten. Neue Dateien oder Ordner können nicht hinzugefügt werden, wenn sie nicht unter dem Betrag für das Gesamtkontingent liegen oder mehr Speicherplatz erworben wird.</span><span class="sxs-lookup"><span data-stu-id="d51e4-p106">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "quota resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
