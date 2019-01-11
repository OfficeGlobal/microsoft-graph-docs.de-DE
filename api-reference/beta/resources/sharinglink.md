---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
ms.openlocfilehash: c303436aafbdbb5167a992f405036b5e00e4d635
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856392"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="a8362-102">Ressourcentyp sharingLink</span><span class="sxs-lookup"><span data-stu-id="a8362-102">sharingLink resource type</span></span>

> <span data-ttu-id="a8362-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a8362-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8362-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a8362-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a8362-105">Die Ressource **SharingLink** gruppiert Link-bezogene Datenelemente in eine einzelne Struktur.</span><span class="sxs-lookup"><span data-stu-id="a8362-105">The **sharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="a8362-106">Wenn eine [**Berechtigung**](permission.md) Ressource ein nicht-Null- **SharingLink** Aspekt ist, stellt die Berechtigung sharing Link (im Gegensatz zu einer Person oder Gruppe gewährten Berechtigungen) dar.</span><span class="sxs-lookup"><span data-stu-id="a8362-106">If a [**permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8362-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a8362-107">JSON representation</span></span>

<span data-ttu-id="a8362-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a8362-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="a8362-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a8362-109">Properties</span></span>

| <span data-ttu-id="a8362-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a8362-110">Property</span></span>       | <span data-ttu-id="a8362-111">Typ</span><span class="sxs-lookup"><span data-stu-id="a8362-111">Type</span></span>          | <span data-ttu-id="a8362-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8362-112">Description</span></span>
|:---------------|:--------------|:-------------------------------------
| <span data-ttu-id="a8362-113">application</span><span class="sxs-lookup"><span data-stu-id="a8362-113">application</span></span>    | <span data-ttu-id="a8362-114">[Identität][]</span><span class="sxs-lookup"><span data-stu-id="a8362-114">[identity][]</span></span>  | <span data-ttu-id="a8362-115">Die App, der der Link zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="a8362-115">The app the link is associated with.</span></span>
| <span data-ttu-id="a8362-116">type</span><span class="sxs-lookup"><span data-stu-id="a8362-116">type</span></span>           | <span data-ttu-id="a8362-117">String</span><span class="sxs-lookup"><span data-stu-id="a8362-117">String</span></span>        | <span data-ttu-id="a8362-118">Der Typ des erstellten Links.</span><span class="sxs-lookup"><span data-stu-id="a8362-118">The type of the link created.</span></span>
| <span data-ttu-id="a8362-119">scope</span><span class="sxs-lookup"><span data-stu-id="a8362-119">scope</span></span>          | <span data-ttu-id="a8362-120">String</span><span class="sxs-lookup"><span data-stu-id="a8362-120">String</span></span>        | <span data-ttu-id="a8362-p102">Der Bereich des Links, der durch diese Berechtigung dargestellt wird. Der Wert `anonymous` gibt an, dass der Link von jedem Benutzer verwendet werden kann. `organization` gibt an, dass der Link von Benutzern verwendet werden kann, die bei dem gleichen Mandanten angemeldet sind.</span><span class="sxs-lookup"><span data-stu-id="a8362-p102">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="a8362-123">preventsDownload</span><span class="sxs-lookup"><span data-stu-id="a8362-123">preventsDownload</span></span> | <span data-ttu-id="a8362-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8362-124">Boolean</span></span>       | <span data-ttu-id="a8362-125">Wenn True, klicken Sie dann der Benutzer kann nur dieser Link zum Anzeigen des Elements im Web verwenden, und nicht verwenden, um den Inhalt des Artikels herunterladen.</span><span class="sxs-lookup"><span data-stu-id="a8362-125">If true then the user can only use this link to view the item on the web, and cannot use it to download the contents of the item.</span></span> <span data-ttu-id="a8362-126">Nur für OneDrive für Unternehmen und SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a8362-126">Only for OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="a8362-127">webHtml</span><span class="sxs-lookup"><span data-stu-id="a8362-127">webHtml</span></span>        | <span data-ttu-id="a8362-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a8362-128">String</span></span>        | <span data-ttu-id="a8362-129">Bei `embed` Links enthält diese Eigenschaft den HTML-Code für ein `<iframe>`-Element, das das Element in eine Webseite einbettet.</span><span class="sxs-lookup"><span data-stu-id="a8362-129">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="a8362-130">webUrl</span><span class="sxs-lookup"><span data-stu-id="a8362-130">webUrl</span></span>         | <span data-ttu-id="a8362-131">String</span><span class="sxs-lookup"><span data-stu-id="a8362-131">String</span></span>        | <span data-ttu-id="a8362-132">Eine URL, mit der das Element im Browser auf der OneDrive-Website geöffnet wird.</span><span class="sxs-lookup"><span data-stu-id="a8362-132">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

### <a name="type-options"></a><span data-ttu-id="a8362-134">Typ-Optionen</span><span class="sxs-lookup"><span data-stu-id="a8362-134">Type options</span></span>

<span data-ttu-id="a8362-135">Die folgende Tabelle zeigt die möglichen Werte für die **Type** -Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="a8362-135">The following table defines the possible values for the **type** property.</span></span>

| <span data-ttu-id="a8362-136">Wert</span><span class="sxs-lookup"><span data-stu-id="a8362-136">Value</span></span>    | <span data-ttu-id="a8362-137">Funktion</span><span class="sxs-lookup"><span data-stu-id="a8362-137">Role</span></span>     | <span data-ttu-id="a8362-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8362-138">Description</span></span>
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | <span data-ttu-id="a8362-139">Ein Freigabelink zum Anzeigen für schreibgeschützten Zugriff.</span><span class="sxs-lookup"><span data-stu-id="a8362-139">A view-only sharing link, allowing read-only access.</span></span>
| `edit`   | `write`  | <span data-ttu-id="a8362-140">Ein Freigabelink zum Bearbeiten für Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="a8362-140">An edit sharing link, allowing read-write access.</span></span>
| `embed`  | `read`   | <span data-ttu-id="a8362-141">Ein schreibgeschützter Freigablink, der zum Einbetten von Inhalten in einer Hostwebseite verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="a8362-141">A view-only sharing link that can be used to embed content into a host webpage.</span></span> <span data-ttu-id="a8362-142">Einbettlinks sind nicht für OneDrive for Business oder SharePoint verfügbar.</span><span class="sxs-lookup"><span data-stu-id="a8362-142">Embed links are not available for OneDrive for Business or SharePoint.</span></span>

### <a name="scope-options"></a><span data-ttu-id="a8362-143">Bereichsoptionen</span><span class="sxs-lookup"><span data-stu-id="a8362-143">Scope options</span></span>

<span data-ttu-id="a8362-144">Die folgende Tabelle zeigt die möglichen Werte für die Eigenschaft **Bereich** .</span><span class="sxs-lookup"><span data-stu-id="a8362-144">The following table defines the possible values for the **scope** property.</span></span>

| <span data-ttu-id="a8362-145">Wert</span><span class="sxs-lookup"><span data-stu-id="a8362-145">Value</span></span>            | <span data-ttu-id="a8362-146">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8362-146">Description</span></span>
|:-----------------|:------------------------------------------------------------
| `anonymous`      | <span data-ttu-id="a8362-147">Jeder Benutzer mit den Link hat Zugriff, ohne Anmeldung.</span><span class="sxs-lookup"><span data-stu-id="a8362-147">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="a8362-148">Dies kann Personen außerhalb Ihrer Organisation enthalten.</span><span class="sxs-lookup"><span data-stu-id="a8362-148">This may include people outside of your organization.</span></span>
| `organization`   | <span data-ttu-id="a8362-149">Den Link können alle Benutzer in Ihrer Organisation (Mandant) signiert um Zugriff zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="a8362-149">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="a8362-150">Nur in OneDrive für Unternehmen und SharePoint verfügbar.</span><span class="sxs-lookup"><span data-stu-id="a8362-150">Only available in OneDrive for Business and SharePoint.</span></span>
| `existingAccess` | <span data-ttu-id="a8362-151">Nur Personen, die bereits Zugriff auf das Element mit anderen Mitteln gewährt wurde, können das Element mit diesem Link zugreifen.</span><span class="sxs-lookup"><span data-stu-id="a8362-151">Only people who have already been granted access to the item through other means can access the item using this link.</span></span> <span data-ttu-id="a8362-152">Nur in OneDrive für Unternehmen und SharePoint verfügbar.</span><span class="sxs-lookup"><span data-stu-id="a8362-152">Only available in OneDrive for Business and SharePoint.</span></span>
| `users`          | <span data-ttu-id="a8362-153">Der Link gewährt Zugriff nur für eine bestimmte Liste von Personen.</span><span class="sxs-lookup"><span data-stu-id="a8362-153">The link grants access only to a specific list of people.</span></span> <span data-ttu-id="a8362-154">Nur in OneDrive für Unternehmen und SharePoint verfügbar.</span><span class="sxs-lookup"><span data-stu-id="a8362-154">Only available in OneDrive for Business and SharePoint.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "tocPath": ""
}-->
