---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
ms.openlocfilehash: 7f0ecdbb498ee75133ec9499027f7cfdc6191327
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480418"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="ee86e-102">sharingLink-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ee86e-102">sharingLink resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee86e-103">Die **sharingLink** -Ressource gruppiert Link bezogene Datenelemente in einer einzelnen Struktur.</span><span class="sxs-lookup"><span data-stu-id="ee86e-103">The **sharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="ee86e-104">Wenn eine [**Permission**](permission.md) -Ressource ein **sharingLink** -Facet ungleich NULL aufweist, stellt die Berechtigung einen Freigabe Link dar (im Gegensatz zu Berechtigungen, die einer Person oder Gruppe erteilt wurden).</span><span class="sxs-lookup"><span data-stu-id="ee86e-104">If a [**permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee86e-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ee86e-105">JSON representation</span></span>

<span data-ttu-id="ee86e-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ee86e-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="ee86e-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ee86e-107">Properties</span></span>

| <span data-ttu-id="ee86e-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ee86e-108">Property</span></span>       | <span data-ttu-id="ee86e-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ee86e-109">Type</span></span>          | <span data-ttu-id="ee86e-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ee86e-110">Description</span></span>
|:---------------|:--------------|:-------------------------------------
| <span data-ttu-id="ee86e-111">application</span><span class="sxs-lookup"><span data-stu-id="ee86e-111">application</span></span>    | <span data-ttu-id="ee86e-112">[Identität][]</span><span class="sxs-lookup"><span data-stu-id="ee86e-112">[identity][]</span></span>  | <span data-ttu-id="ee86e-113">Die App, der der Link zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="ee86e-113">The app the link is associated with.</span></span>
| <span data-ttu-id="ee86e-114">type</span><span class="sxs-lookup"><span data-stu-id="ee86e-114">type</span></span>           | <span data-ttu-id="ee86e-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ee86e-115">String</span></span>        | <span data-ttu-id="ee86e-116">Der Typ des erstellten Links.</span><span class="sxs-lookup"><span data-stu-id="ee86e-116">The type of the link created.</span></span>
| <span data-ttu-id="ee86e-117">scope</span><span class="sxs-lookup"><span data-stu-id="ee86e-117">scope</span></span>          | <span data-ttu-id="ee86e-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ee86e-118">String</span></span>        | <span data-ttu-id="ee86e-p101">Der Bereich des Links, der durch diese Berechtigung dargestellt wird. Der Wert `anonymous` gibt an, dass der Link von jedem Benutzer verwendet werden kann. `organization` gibt an, dass der Link von Benutzern verwendet werden kann, die bei dem gleichen Mandanten angemeldet sind.</span><span class="sxs-lookup"><span data-stu-id="ee86e-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="ee86e-121">preventsDownload</span><span class="sxs-lookup"><span data-stu-id="ee86e-121">preventsDownload</span></span> | <span data-ttu-id="ee86e-122">Boolesch</span><span class="sxs-lookup"><span data-stu-id="ee86e-122">Boolean</span></span>       | <span data-ttu-id="ee86e-123">Wenn true, kann der Benutzer diesen Link nur verwenden, um das Element im Web anzuzeigen, und kann es nicht verwenden, um den Inhalt des Elements herunterzuladen.</span><span class="sxs-lookup"><span data-stu-id="ee86e-123">If true then the user can only use this link to view the item on the web, and cannot use it to download the contents of the item.</span></span> <span data-ttu-id="ee86e-124">Nur für OneDrive for Business und SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ee86e-124">Only for OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="ee86e-125">webHtml</span><span class="sxs-lookup"><span data-stu-id="ee86e-125">webHtml</span></span>        | <span data-ttu-id="ee86e-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ee86e-126">String</span></span>        | <span data-ttu-id="ee86e-127">Bei `embed` Links enthält diese Eigenschaft den HTML-Code für ein `<iframe>`-Element, das das Element in eine Webseite einbettet.</span><span class="sxs-lookup"><span data-stu-id="ee86e-127">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="ee86e-128">webUrl</span><span class="sxs-lookup"><span data-stu-id="ee86e-128">webUrl</span></span>         | <span data-ttu-id="ee86e-129">String</span><span class="sxs-lookup"><span data-stu-id="ee86e-129">String</span></span>        | <span data-ttu-id="ee86e-130">Eine URL, mit der das Element im Browser auf der OneDrive-Website geöffnet wird.</span><span class="sxs-lookup"><span data-stu-id="ee86e-130">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identität]: identity.md
[Identity]: identity.md

### <a name="type-options"></a><span data-ttu-id="ee86e-132">Typoptionen</span><span class="sxs-lookup"><span data-stu-id="ee86e-132">Type options</span></span>

<span data-ttu-id="ee86e-133">In der folgenden Tabelle sind die möglichen Werte für die **Type** -Eigenschaft definiert.</span><span class="sxs-lookup"><span data-stu-id="ee86e-133">The following table defines the possible values for the **type** property.</span></span>

| <span data-ttu-id="ee86e-134">Wert</span><span class="sxs-lookup"><span data-stu-id="ee86e-134">Value</span></span>    | <span data-ttu-id="ee86e-135">Funktion</span><span class="sxs-lookup"><span data-stu-id="ee86e-135">Role</span></span>     | <span data-ttu-id="ee86e-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ee86e-136">Description</span></span>
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | <span data-ttu-id="ee86e-137">Ein Freigabelink zum Anzeigen für schreibgeschützten Zugriff.</span><span class="sxs-lookup"><span data-stu-id="ee86e-137">A view-only sharing link, allowing read-only access.</span></span>
| `edit`   | `write`  | <span data-ttu-id="ee86e-138">Ein Freigabelink zum Bearbeiten für Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="ee86e-138">An edit sharing link, allowing read-write access.</span></span>
| `embed`  | `read`   | <span data-ttu-id="ee86e-p103">Ein schreibgeschützter Freigablink, der zum Einbetten von Inhalten in einer Hostwebseite verwendet werden kann. Einbettlinks sind nicht für OneDrive for Business oder SharePoint verfügbar.</span><span class="sxs-lookup"><span data-stu-id="ee86e-p103">A view-only sharing link that can be used to embed content into a host webpage. Embed links are not available for OneDrive for Business or SharePoint.</span></span>

### <a name="scope-options"></a><span data-ttu-id="ee86e-141">Bereichsoptionen</span><span class="sxs-lookup"><span data-stu-id="ee86e-141">Scope options</span></span>

<span data-ttu-id="ee86e-142">In der folgenden Tabelle sind die möglichen Werte für die **Scope** -Eigenschaft definiert.</span><span class="sxs-lookup"><span data-stu-id="ee86e-142">The following table defines the possible values for the **scope** property.</span></span>

| <span data-ttu-id="ee86e-143">Wert</span><span class="sxs-lookup"><span data-stu-id="ee86e-143">Value</span></span>            | <span data-ttu-id="ee86e-144">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ee86e-144">Description</span></span>
|:-----------------|:------------------------------------------------------------
| `anonymous`      | <span data-ttu-id="ee86e-145">Jeder, der über die Verknüpfung verfügt, hat Zugriff, ohne sich anmelden zu müssen.</span><span class="sxs-lookup"><span data-stu-id="ee86e-145">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="ee86e-146">Dies kann Personen außerhalb Ihrer Organisation sein.</span><span class="sxs-lookup"><span data-stu-id="ee86e-146">This may include people outside of your organization.</span></span>
| `organization`   | <span data-ttu-id="ee86e-147">Jeder, der bei Ihrer Organisation (Mandant) angemeldet ist, kann über den Link Zugriff erhalten.</span><span class="sxs-lookup"><span data-stu-id="ee86e-147">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="ee86e-148">Nur in OneDrive for Business und SharePoint verfügbar.</span><span class="sxs-lookup"><span data-stu-id="ee86e-148">Only available in OneDrive for Business and SharePoint.</span></span>
| `existingAccess` | <span data-ttu-id="ee86e-149">Nur Personen, denen bereits auf andere Weise Zugriff auf das Element gewährt wurde, können über diesen Link auf das Element zugreifen.</span><span class="sxs-lookup"><span data-stu-id="ee86e-149">Only people who have already been granted access to the item through other means can access the item using this link.</span></span> <span data-ttu-id="ee86e-150">Nur in OneDrive for Business und SharePoint verfügbar.</span><span class="sxs-lookup"><span data-stu-id="ee86e-150">Only available in OneDrive for Business and SharePoint.</span></span>
| `users`          | <span data-ttu-id="ee86e-151">Der Link gewährt Zugriff nur auf eine bestimmte Personenliste.</span><span class="sxs-lookup"><span data-stu-id="ee86e-151">The link grants access only to a specific list of people.</span></span> <span data-ttu-id="ee86e-152">Nur in OneDrive for Business und SharePoint verfügbar.</span><span class="sxs-lookup"><span data-stu-id="ee86e-152">Only available in OneDrive for Business and SharePoint.</span></span>

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
