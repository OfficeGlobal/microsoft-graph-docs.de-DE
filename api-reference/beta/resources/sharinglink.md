---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
ms.openlocfilehash: c21c891981106faa4b631bb2713913bfa8ed0713
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521453"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="5d934-102">SharingLink-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5d934-102">sharingLink resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d934-103">Die **SharingLink**-Ressource gruppiert linkbezogene Datenelemente in einer einzelnen Struktur.</span><span class="sxs-lookup"><span data-stu-id="5d934-103">The **sharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="5d934-104">Wenn eine [**Permission**](permission.md)-Ressource ein **sharingLink**-Facet ungleich Null aufweist, stellt die Berechtigung einen Freigabelink dar (im Gegensatz zu Berechtigungen, die einer Person oder Gruppe erteilten werden).</span><span class="sxs-lookup"><span data-stu-id="5d934-104">If a [**permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="5d934-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5d934-105">JSON representation</span></span>

<span data-ttu-id="5d934-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5d934-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "application", "scope" ],
  "@odata.type": "microsoft.graph.sharingLink"
}-->

```json
{
  "application": { "@odata.type": "microsoft.graph.identity" },
  "preventsDownload": false,
  "type": "view | edit | embed",
  "scope": "anonymous | organization",
  "webHtml": "string",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="5d934-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5d934-107">Properties</span></span>

| <span data-ttu-id="5d934-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5d934-108">Property</span></span>       | <span data-ttu-id="5d934-109">Typ</span><span class="sxs-lookup"><span data-stu-id="5d934-109">Type</span></span>          | <span data-ttu-id="5d934-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5d934-110">Description</span></span>
|:---------------|:--------------|:-------------------------------------
| <span data-ttu-id="5d934-111">application</span><span class="sxs-lookup"><span data-stu-id="5d934-111">application</span></span>    | <span data-ttu-id="5d934-112">[Identität][]</span><span class="sxs-lookup"><span data-stu-id="5d934-112">[identity][]</span></span>  | <span data-ttu-id="5d934-113">Die App, der der Link zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="5d934-113">The app the link is associated with.</span></span>
| <span data-ttu-id="5d934-114">type</span><span class="sxs-lookup"><span data-stu-id="5d934-114">type</span></span>           | <span data-ttu-id="5d934-115">String</span><span class="sxs-lookup"><span data-stu-id="5d934-115">String</span></span>        | <span data-ttu-id="5d934-116">Der Typ des erstellten Links.</span><span class="sxs-lookup"><span data-stu-id="5d934-116">The type of the link created.</span></span>
| <span data-ttu-id="5d934-117">scope</span><span class="sxs-lookup"><span data-stu-id="5d934-117">scope</span></span>          | <span data-ttu-id="5d934-118">String</span><span class="sxs-lookup"><span data-stu-id="5d934-118">String</span></span>        | <span data-ttu-id="5d934-p101">Der Bereich des Links, der durch diese Berechtigung dargestellt wird. Der Wert `anonymous` gibt an, dass der Link von jedem Benutzer verwendet werden kann. `organization` gibt an, dass der Link von Benutzern verwendet werden kann, die bei dem gleichen Mandanten angemeldet sind.</span><span class="sxs-lookup"><span data-stu-id="5d934-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="5d934-121">preventsDownload</span><span class="sxs-lookup"><span data-stu-id="5d934-121">preventsDownload</span></span> | <span data-ttu-id="5d934-122">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="5d934-122">Boolean</span></span>       | <span data-ttu-id="5d934-123">Wenn True, klicken Sie dann der Benutzer kann nur dieser Link zum Anzeigen des Elements im Web verwenden, und nicht verwenden, um den Inhalt des Artikels herunterladen.</span><span class="sxs-lookup"><span data-stu-id="5d934-123">If true then the user can only use this link to view the item on the web, and cannot use it to download the contents of the item.</span></span> <span data-ttu-id="5d934-124">Nur für OneDrive für Unternehmen und SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5d934-124">Only for OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="5d934-125">webHtml</span><span class="sxs-lookup"><span data-stu-id="5d934-125">webHtml</span></span>        | <span data-ttu-id="5d934-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5d934-126">String</span></span>        | <span data-ttu-id="5d934-127">Bei `embed` Links enthält diese Eigenschaft den HTML-Code für ein `<iframe>`-Element, das das Element in eine Webseite einbettet.</span><span class="sxs-lookup"><span data-stu-id="5d934-127">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="5d934-128">webUrl</span><span class="sxs-lookup"><span data-stu-id="5d934-128">webUrl</span></span>         | <span data-ttu-id="5d934-129">String</span><span class="sxs-lookup"><span data-stu-id="5d934-129">String</span></span>        | <span data-ttu-id="5d934-130">Eine URL, mit der das Element im Browser auf der OneDrive-Website geöffnet wird.</span><span class="sxs-lookup"><span data-stu-id="5d934-130">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

### <a name="type-options"></a><span data-ttu-id="5d934-132">Typ-Optionen</span><span class="sxs-lookup"><span data-stu-id="5d934-132">Type options</span></span>

<span data-ttu-id="5d934-133">Die folgende Tabelle zeigt die möglichen Werte für die **Type** -Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="5d934-133">The following table defines the possible values for the **type** property.</span></span>

| <span data-ttu-id="5d934-134">Wert</span><span class="sxs-lookup"><span data-stu-id="5d934-134">Value</span></span>    | <span data-ttu-id="5d934-135">Funktion</span><span class="sxs-lookup"><span data-stu-id="5d934-135">Role</span></span>     | <span data-ttu-id="5d934-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5d934-136">Description</span></span>
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | <span data-ttu-id="5d934-137">Ein Freigabelink zum Anzeigen für schreibgeschützten Zugriff.</span><span class="sxs-lookup"><span data-stu-id="5d934-137">A view-only sharing link, allowing read-only access.</span></span>
| `edit`   | `write`  | <span data-ttu-id="5d934-138">Ein Freigabelink zum Bearbeiten für Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="5d934-138">An edit sharing link, allowing read-write access.</span></span>
| `embed`  | `read`   | <span data-ttu-id="5d934-139">Ein schreibgeschützter Freigablink, der zum Einbetten von Inhalten in einer Hostwebseite verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="5d934-139">A view-only sharing link that can be used to embed content into a host webpage.</span></span> <span data-ttu-id="5d934-140">Einbettlinks sind nicht für OneDrive for Business oder SharePoint verfügbar.</span><span class="sxs-lookup"><span data-stu-id="5d934-140">Embed links are not available for OneDrive for Business or SharePoint.</span></span>

### <a name="scope-options"></a><span data-ttu-id="5d934-141">Bereichsoptionen</span><span class="sxs-lookup"><span data-stu-id="5d934-141">Scope options</span></span>

<span data-ttu-id="5d934-142">Die folgende Tabelle zeigt die möglichen Werte für die Eigenschaft **Bereich** .</span><span class="sxs-lookup"><span data-stu-id="5d934-142">The following table defines the possible values for the **scope** property.</span></span>

| <span data-ttu-id="5d934-143">Wert</span><span class="sxs-lookup"><span data-stu-id="5d934-143">Value</span></span>            | <span data-ttu-id="5d934-144">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5d934-144">Description</span></span>
|:-----------------|:------------------------------------------------------------
| `anonymous`      | <span data-ttu-id="5d934-145">Jeder Benutzer mit den Link hat Zugriff, ohne Anmeldung.</span><span class="sxs-lookup"><span data-stu-id="5d934-145">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="5d934-146">Dies kann Personen außerhalb Ihrer Organisation enthalten.</span><span class="sxs-lookup"><span data-stu-id="5d934-146">This may include people outside of your organization.</span></span>
| `organization`   | <span data-ttu-id="5d934-147">Den Link können alle Benutzer in Ihrer Organisation (Mandant) signiert um Zugriff zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="5d934-147">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="5d934-148">Nur in OneDrive für Unternehmen und SharePoint verfügbar.</span><span class="sxs-lookup"><span data-stu-id="5d934-148">Only available in OneDrive for Business and SharePoint.</span></span>
| `existingAccess` | <span data-ttu-id="5d934-149">Nur Personen, die bereits Zugriff auf das Element mit anderen Mitteln gewährt wurde, können das Element mit diesem Link zugreifen.</span><span class="sxs-lookup"><span data-stu-id="5d934-149">Only people who have already been granted access to the item through other means can access the item using this link.</span></span> <span data-ttu-id="5d934-150">Nur in OneDrive für Unternehmen und SharePoint verfügbar.</span><span class="sxs-lookup"><span data-stu-id="5d934-150">Only available in OneDrive for Business and SharePoint.</span></span>
| `users`          | <span data-ttu-id="5d934-151">Der Link gewährt Zugriff nur für eine bestimmte Liste von Personen.</span><span class="sxs-lookup"><span data-stu-id="5d934-151">The link grants access only to a specific list of people.</span></span> <span data-ttu-id="5d934-152">Nur in OneDrive für Unternehmen und SharePoint verfügbar.</span><span class="sxs-lookup"><span data-stu-id="5d934-152">Only available in OneDrive for Business and SharePoint.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sharinglink.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
