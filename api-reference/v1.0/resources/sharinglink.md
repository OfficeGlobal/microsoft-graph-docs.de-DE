# <a name="sharinglink-resource-type"></a><span data-ttu-id="4c70f-101">SharingLink-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4c70f-101">SharingLink resource type</span></span>

<span data-ttu-id="4c70f-102">Die **SharingLink**-Ressource gruppiert linkbezogene Datenelemente in einer einzelnen Struktur.</span><span class="sxs-lookup"><span data-stu-id="4c70f-102">The **SharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="4c70f-103">Wenn eine [**Permission**](permission.md)-Ressource ein **sharingLink**-Facet ungleich Null aufweist, stellt die Berechtigung einen Freigabelink dar (im Gegensatz zu Berechtigungen, die einer Person oder Gruppe erteilten werden).</span><span class="sxs-lookup"><span data-stu-id="4c70f-103">If a [**Permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c70f-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4c70f-104">JSON representation</span></span>

<span data-ttu-id="4c70f-105">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4c70f-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "application", "scope" ],
  "@odata.type": "microsoft.graph.sharingLink"
}-->

```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "type": "view | edit",
  "scope": "anonymous | organization",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="4c70f-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4c70f-106">Properties</span></span>

| <span data-ttu-id="4c70f-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4c70f-107">Property</span></span>    | <span data-ttu-id="4c70f-108">Typ</span><span class="sxs-lookup"><span data-stu-id="4c70f-108">Type</span></span>                    | <span data-ttu-id="4c70f-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4c70f-109">Description</span></span>                                                                                                                                                                                             |
|:------------|:------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4c70f-110">application</span><span class="sxs-lookup"><span data-stu-id="4c70f-110">application</span></span> | [<span data-ttu-id="4c70f-111">Identität</span><span class="sxs-lookup"><span data-stu-id="4c70f-111">identity</span></span>](identity.md) | <span data-ttu-id="4c70f-112">Die App, der der Link zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="4c70f-112">The app the link is associated with.</span></span>                                                                                                                                                                    |
| <span data-ttu-id="4c70f-113">type</span><span class="sxs-lookup"><span data-stu-id="4c70f-113">type</span></span>        | <span data-ttu-id="4c70f-114">String</span><span class="sxs-lookup"><span data-stu-id="4c70f-114">String</span></span>                  | <span data-ttu-id="4c70f-115">Der Typ des erstellten Links.</span><span class="sxs-lookup"><span data-stu-id="4c70f-115">The type of the link created.</span></span>                                                                                                                                                                           |
| <span data-ttu-id="4c70f-116">scope</span><span class="sxs-lookup"><span data-stu-id="4c70f-116">scope</span></span>       | <span data-ttu-id="4c70f-117">String</span><span class="sxs-lookup"><span data-stu-id="4c70f-117">String</span></span>                  | <span data-ttu-id="4c70f-p101">Der Bereich des Links, der durch diese Berechtigung dargestellt wird. Der Wert `anonymous` gibt an, dass der Link von jedem Benutzer verwendet werden kann. `organization` gibt an, dass der Link von Benutzern verwendet werden kann, die bei dem gleichen Mandanten angemeldet sind.</span><span class="sxs-lookup"><span data-stu-id="4c70f-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span> |
| <span data-ttu-id="4c70f-120">webUrl</span><span class="sxs-lookup"><span data-stu-id="4c70f-120">webUrl</span></span>      | <span data-ttu-id="4c70f-121">String</span><span class="sxs-lookup"><span data-stu-id="4c70f-121">String</span></span>                  | <span data-ttu-id="4c70f-122">Eine URL, mit der das Element im Browser auf der OneDrive-Website geöffnet wird.</span><span class="sxs-lookup"><span data-stu-id="4c70f-122">A URL that opens the item in the browser on the OneDrive website.</span></span>                                                                                                                                       |

## <a name="type-enumeration"></a><span data-ttu-id="4c70f-123">Type-Enumeration</span><span class="sxs-lookup"><span data-stu-id="4c70f-123">Type enumeration</span></span>

<span data-ttu-id="4c70f-124">In dieser Tabelle werden zulässige Werte für die **type**-Eigenschaft aufgeführt:</span><span class="sxs-lookup"><span data-stu-id="4c70f-124">This table defines the possible values for the **type** property:</span></span>

| <span data-ttu-id="4c70f-125">Wert</span><span class="sxs-lookup"><span data-stu-id="4c70f-125">Value</span></span>   | <span data-ttu-id="4c70f-126">Funktion</span><span class="sxs-lookup"><span data-stu-id="4c70f-126">Role</span></span>    | <span data-ttu-id="4c70f-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4c70f-127">Description</span></span>                                                                     |
|:--------|:--------|:--------------------------------------------------------------------------------|
| `view`  | `read`  | <span data-ttu-id="4c70f-128">Ein Freigabelink zum Anzeigen für schreibgeschützten Zugriff.</span><span class="sxs-lookup"><span data-stu-id="4c70f-128">A view-only sharing link, allowing read-only access.</span></span>                            |
| `edit`  | `write` | <span data-ttu-id="4c70f-129">Ein Freigabelink zum Bearbeiten für Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="4c70f-129">An edit sharing link, allowing read-write access.</span></span>                               |

## <a name="scope-enumeration"></a><span data-ttu-id="4c70f-130">Scope-Enumeration</span><span class="sxs-lookup"><span data-stu-id="4c70f-130">Scope enumeration</span></span>

| <span data-ttu-id="4c70f-131">Wert</span><span class="sxs-lookup"><span data-stu-id="4c70f-131">Value</span></span>          | <span data-ttu-id="4c70f-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4c70f-132">Description</span></span>                                                                                                                 |
|:---------------|:----------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="4c70f-133">Der Freigabelink steht für alle Benutzer zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="4c70f-133">The sharing link is available for anyone to use.</span></span>                                                                            |
| `organization` | <span data-ttu-id="4c70f-p102">Der Freigabelink steht für Benutzer in derselben Organisation (Mandant) zur Verfügung. Nicht für OneDrive Personal verfügbar.</span><span class="sxs-lookup"><span data-stu-id="4c70f-p102">The sharing link is available for anyone within the same organization (tenant) to use. Not available for OneDrive Personal.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sharingLink resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
