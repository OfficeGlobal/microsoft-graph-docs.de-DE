# <a name="drive-resource-type"></a><span data-ttu-id="10b66-101">Ressourcentyp drive</span><span class="sxs-lookup"><span data-stu-id="10b66-101">Drive resource type</span></span>

<span data-ttu-id="10b66-102">Die drive-Ressource ist das Objekt der obersten Ebene innerhalb des OneDrive eines Benutzers oder einer Dokumentbibliothek in SharePoint.</span><span class="sxs-lookup"><span data-stu-id="10b66-102">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="10b66-p101">OneDrive-Benutzern steht immer mindestens ein Laufwerk zur Verfügung, das Standardlaufwerk. Benutzern ohne OneDrive-Lizenz steht möglicherweise kein Standardlaufwerk zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="10b66-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="10b66-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="10b66-105">JSON representation</span></span>

<span data-ttu-id="10b66-106">Es folgt eine JSON-Darstellung einer **drive**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="10b66-106">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="10b66-107">Die **drive**-Ressource wird von [ **baseItem** ](baseitem.md) abgeleitet und erbt Eigenschaften von dieser Ressource.</span><span class="sxs-lookup"><span data-stu-id="10b66-107">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "items", "root", "special", "owner", "description" ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.drive"
}-->

```json
{
  "id": "string (identifier)",
  "driveType": "string",
  "owner": {"@odata.type": "microsoft.graph.identitySet"},
  "quota": {"@odata.type": "microsoft.graph.quota"},
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },

  /* relationships */
  "root": {"@odata.type": "microsoft.graph.driveItem" },
  "items": [ {"@odata.type": "microsoft.graph.driveItem" }],
  "special": [ {"@odata.type": "microsoft.graph.driveItem" }],

  /* inherited from baseItem */
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "datetime",
  "description": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "datetime",
  "name": "string",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="10b66-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="10b66-108">Properties</span></span>

| <span data-ttu-id="10b66-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="10b66-109">Property</span></span>             | <span data-ttu-id="10b66-110">Typ</span><span class="sxs-lookup"><span data-stu-id="10b66-110">Type</span></span>                          | <span data-ttu-id="10b66-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="10b66-111">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="10b66-112">id</span><span class="sxs-lookup"><span data-stu-id="10b66-112">id</span></span>                   | <span data-ttu-id="10b66-113">String</span><span class="sxs-lookup"><span data-stu-id="10b66-113">String</span></span>                        | <span data-ttu-id="10b66-p102">Der eindeutige Bezeichner des Laufwerks. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="10b66-p102">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="10b66-116">createdBy</span><span class="sxs-lookup"><span data-stu-id="10b66-116">createdBy</span></span>            | <span data-ttu-id="10b66-117">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="10b66-117">[identitySet][]</span></span>               | <span data-ttu-id="10b66-p103">Die Identität des Benutzers, des Geräts oder der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="10b66-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="10b66-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="10b66-120">createdDateTime</span></span>      | <span data-ttu-id="10b66-121">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10b66-121">dateTimeOffset</span></span>                | <span data-ttu-id="10b66-p104">Datum und Uhrzeit der Elementerstellung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="10b66-p104">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="10b66-124">driveType</span><span class="sxs-lookup"><span data-stu-id="10b66-124">driveType</span></span>            | <span data-ttu-id="10b66-125">String</span><span class="sxs-lookup"><span data-stu-id="10b66-125">String</span></span>                        | <span data-ttu-id="10b66-p105">Beschreibt den Typ des Laufwerks, der durch diese Ressource dargestellt wird. Persönliche OneDrive-Laufwerke geben `personal` zurück. OneDrive for Business gibt `business` zurück. SharePoint-Dokumentbibliotheken geben `documentLibrary` zurück. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="10b66-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="10b66-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="10b66-131">lastModifiedBy</span></span>       | <span data-ttu-id="10b66-132">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="10b66-132">[identitySet][]</span></span>               | <span data-ttu-id="10b66-p106">Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element zuletzt geändert wurde. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="10b66-p106">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="10b66-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="10b66-135">lastModifiedDateTime</span></span> | <span data-ttu-id="10b66-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10b66-136">dateTimeOffset</span></span>                | <span data-ttu-id="10b66-p107">Datum und Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="10b66-p107">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="10b66-139">name</span><span class="sxs-lookup"><span data-stu-id="10b66-139">name</span></span>                 | <span data-ttu-id="10b66-140">string</span><span class="sxs-lookup"><span data-stu-id="10b66-140">string</span></span>                        | <span data-ttu-id="10b66-p108">Der Name des Elements. Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="10b66-p108">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="10b66-143">owner</span><span class="sxs-lookup"><span data-stu-id="10b66-143">owner</span></span>                | [<span data-ttu-id="10b66-144">identitySet</span><span class="sxs-lookup"><span data-stu-id="10b66-144">identitySet</span></span>](identityset.md) | <span data-ttu-id="10b66-p109">Optional.  Das Benutzerkonto, das das Laufwerk besitzt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="10b66-p109">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="10b66-148">quota</span><span class="sxs-lookup"><span data-stu-id="10b66-148">quota</span></span>                | [<span data-ttu-id="10b66-149">quota</span><span class="sxs-lookup"><span data-stu-id="10b66-149">quota</span></span>](quota.md)             | <span data-ttu-id="10b66-p110">Optional.  Informationen zum Speicherkontingent des Laufwerks. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="10b66-p110">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="10b66-153">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="10b66-153">sharepointIds</span></span>        | <span data-ttu-id="10b66-154">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="10b66-154">[sharepointIds][]</span></span>             | <span data-ttu-id="10b66-p111">Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="10b66-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="10b66-157">webUrl</span><span class="sxs-lookup"><span data-stu-id="10b66-157">webUrl</span></span>               | <span data-ttu-id="10b66-158">String (URL)</span><span class="sxs-lookup"><span data-stu-id="10b66-158">string (url)</span></span>                  | <span data-ttu-id="10b66-p112">URL, über die die Ressource im Browser angezeigt werden kann. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="10b66-p112">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

<span data-ttu-id="10b66-161">[identitySet]: identityset.md</span><span class="sxs-lookup"><span data-stu-id="10b66-161">[identitySet]: identityset.md</span></span>
<span data-ttu-id="10b66-162">[sharepointIds]: sharepointids.md</span><span class="sxs-lookup"><span data-stu-id="10b66-162">[sharepointIds]: sharepointids.md</span></span>

## <a name="relationships"></a><span data-ttu-id="10b66-163">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="10b66-163">Relationships</span></span>

| <span data-ttu-id="10b66-164">Beziehung</span><span class="sxs-lookup"><span data-stu-id="10b66-164">Relationship</span></span> | <span data-ttu-id="10b66-165">Typ</span><span class="sxs-lookup"><span data-stu-id="10b66-165">Type</span></span>                                 | <span data-ttu-id="10b66-166">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="10b66-166">Description</span></span>                                                              |
| :----------- | :----------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="10b66-167">items</span><span class="sxs-lookup"><span data-stu-id="10b66-167">items</span></span>        | <span data-ttu-id="10b66-168">[driveitem](driveitem.md) collection</span><span class="sxs-lookup"><span data-stu-id="10b66-168">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="10b66-p113">Alle im Laufwerk enthaltenen Elemente. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="10b66-p113">All items contained in the drive. Read-only. Nullable.</span></span>                   |
| <span data-ttu-id="10b66-172">root</span><span class="sxs-lookup"><span data-stu-id="10b66-172">root</span></span>         | [<span data-ttu-id="10b66-173">driveitem</span><span class="sxs-lookup"><span data-stu-id="10b66-173">driveitem</span></span>](driveitem.md)            | <span data-ttu-id="10b66-p114">Der Stammordner des Laufwerks. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="10b66-p114">The root folder of the drive. Read-only.</span></span>                                 |
| <span data-ttu-id="10b66-176">Sonderfall</span><span class="sxs-lookup"><span data-stu-id="10b66-176">special</span></span>      | <span data-ttu-id="10b66-177">[driveitem](driveitem.md) collection</span><span class="sxs-lookup"><span data-stu-id="10b66-177">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="10b66-p115">Sammlung gemeinsamer Ordner, die  in OneDrive zur Verfügung stehen. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="10b66-p115">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span> |

## <a name="methods"></a><span data-ttu-id="10b66-181">Methoden</span><span class="sxs-lookup"><span data-stu-id="10b66-181">Methods</span></span>

<span data-ttu-id="10b66-182">Die folgenden Methoden stehen für Laufwerksressourcen zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="10b66-182">The following methods are available for drive resources.</span></span>

| <span data-ttu-id="10b66-183">Methode</span><span class="sxs-lookup"><span data-stu-id="10b66-183">Method</span></span>                                                | <span data-ttu-id="10b66-184">REST-Pfad</span><span class="sxs-lookup"><span data-stu-id="10b66-184">REST Path</span></span>                        |
| :---------------------------------------------------- | :------------------------------- |
| [<span data-ttu-id="10b66-185">Abrufen des Standardlaufwerks des Benutzers</span><span class="sxs-lookup"><span data-stu-id="10b66-185">Get user's default drive</span></span>](../api/drive_get.md)       | `GET /me/drive`                  |
| [<span data-ttu-id="10b66-186">Abrufen des Laufwerks eines anderen Benutzers</span><span class="sxs-lookup"><span data-stu-id="10b66-186">Get another user's drive</span></span>](../api/drive_get.md)       | `GET /users/{user-id}/drive`     |
| [<span data-ttu-id="10b66-187">Abrufen des Stammordners für ein Laufwerk</span><span class="sxs-lookup"><span data-stu-id="10b66-187">Get root folder for a drive</span></span>](../api/item_get.md)     | `GET /drives/{drive-id}/root`    |
| [<span data-ttu-id="10b66-188">Auflisten von Elementen auf einem Laufwerk</span><span class="sxs-lookup"><span data-stu-id="10b66-188">List items in a drive</span></span>](../api/item_list_children.md) | `GET /me/drive/root/children`    |
| [<span data-ttu-id="10b66-189">Auflisten von Änderungen auf einem Laufwerk</span><span class="sxs-lookup"><span data-stu-id="10b66-189">List changes in a drive</span></span>](../api/item_delta.md)       | `GET /me/drive/root/delta`       |
| [<span data-ttu-id="10b66-190">Suchen nach Elementen auf einem Laufwerk</span><span class="sxs-lookup"><span data-stu-id="10b66-190">Search items in a drive</span></span>](../api/item_search.md)      | `GET /me/drive/search(q='text')` |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "drive resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive"
}-->
