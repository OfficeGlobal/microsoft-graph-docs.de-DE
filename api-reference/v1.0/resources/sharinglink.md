---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
ms.openlocfilehash: 02a4c0251a5484edc7ba5e07095f44043c269ae5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863553"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="93ac7-102">SharingLink-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="93ac7-102">SharingLink resource type</span></span>

<span data-ttu-id="93ac7-103">Die **SharingLink**-Ressource gruppiert linkbezogene Datenelemente in einer einzelnen Struktur.</span><span class="sxs-lookup"><span data-stu-id="93ac7-103">The **SharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="93ac7-104">Wenn eine [**Permission**](permission.md)-Ressource ein **sharingLink**-Facet ungleich Null aufweist, stellt die Berechtigung einen Freigabelink dar (im Gegensatz zu Berechtigungen, die einer Person oder Gruppe erteilten werden).</span><span class="sxs-lookup"><span data-stu-id="93ac7-104">If a [**Permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="93ac7-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="93ac7-105">JSON representation</span></span>

<span data-ttu-id="93ac7-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="93ac7-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "application", "scope" ],
  "@odata.type": "microsoft.graph.sharingLink"
}-->

```json
{
  "application": { "@odata.type": "microsoft.graph.identity" },
  "type": "view | edit | embed",
  "scope": "anonymous | organization",
  "webHtml": "string",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="93ac7-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="93ac7-107">Properties</span></span>

| <span data-ttu-id="93ac7-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="93ac7-108">Property</span></span>    | <span data-ttu-id="93ac7-109">Typ</span><span class="sxs-lookup"><span data-stu-id="93ac7-109">Type</span></span>          | <span data-ttu-id="93ac7-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="93ac7-110">Description</span></span>
|:------------|:--------------|:-------------------------------------
| <span data-ttu-id="93ac7-111">application</span><span class="sxs-lookup"><span data-stu-id="93ac7-111">application</span></span> | <span data-ttu-id="93ac7-112">[Identität][]</span><span class="sxs-lookup"><span data-stu-id="93ac7-112">[identity][]</span></span>  | <span data-ttu-id="93ac7-113">Die App, der der Link zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="93ac7-113">The app the link is associated with.</span></span>
| <span data-ttu-id="93ac7-114">type</span><span class="sxs-lookup"><span data-stu-id="93ac7-114">type</span></span>        | <span data-ttu-id="93ac7-115">String</span><span class="sxs-lookup"><span data-stu-id="93ac7-115">String</span></span>        | <span data-ttu-id="93ac7-116">Der Typ des erstellten Links.</span><span class="sxs-lookup"><span data-stu-id="93ac7-116">The type of the link created.</span></span>
| <span data-ttu-id="93ac7-117">scope</span><span class="sxs-lookup"><span data-stu-id="93ac7-117">scope</span></span>       | <span data-ttu-id="93ac7-118">String</span><span class="sxs-lookup"><span data-stu-id="93ac7-118">String</span></span>        | <span data-ttu-id="93ac7-p101">Der Bereich des Links, der durch diese Berechtigung dargestellt wird. Der Wert `anonymous` gibt an, dass der Link von jedem Benutzer verwendet werden kann. `organization` gibt an, dass der Link von Benutzern verwendet werden kann, die bei dem gleichen Mandanten angemeldet sind.</span><span class="sxs-lookup"><span data-stu-id="93ac7-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="93ac7-121">webHtml</span><span class="sxs-lookup"><span data-stu-id="93ac7-121">webHtml</span></span>     | <span data-ttu-id="93ac7-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93ac7-122">String</span></span>        | <span data-ttu-id="93ac7-123">Bei `embed` Links enthält diese Eigenschaft den HTML-Code für ein `<iframe>`-Element, das das Element in eine Webseite einbettet.</span><span class="sxs-lookup"><span data-stu-id="93ac7-123">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="93ac7-124">webUrl</span><span class="sxs-lookup"><span data-stu-id="93ac7-124">webUrl</span></span>      | <span data-ttu-id="93ac7-125">String</span><span class="sxs-lookup"><span data-stu-id="93ac7-125">String</span></span>        | <span data-ttu-id="93ac7-126">Eine URL, mit der das Element im Browser auf der OneDrive-Website geöffnet wird.</span><span class="sxs-lookup"><span data-stu-id="93ac7-126">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identität]: identity.md
[Identity]: identity.md

## <a name="type-options"></a><span data-ttu-id="93ac7-128">Typ-Optionen</span><span class="sxs-lookup"><span data-stu-id="93ac7-128">Type options</span></span>

<span data-ttu-id="93ac7-129">In dieser Tabelle werden zulässige Werte für die **type**-Eigenschaft aufgeführt:</span><span class="sxs-lookup"><span data-stu-id="93ac7-129">This table defines the possible values for the **type** property:</span></span>

| <span data-ttu-id="93ac7-130">Wert</span><span class="sxs-lookup"><span data-stu-id="93ac7-130">Value</span></span>   | <span data-ttu-id="93ac7-131">Funktion</span><span class="sxs-lookup"><span data-stu-id="93ac7-131">Role</span></span>    | <span data-ttu-id="93ac7-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="93ac7-132">Description</span></span>
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | <span data-ttu-id="93ac7-133">Ein Freigabelink zum Anzeigen für schreibgeschützten Zugriff.</span><span class="sxs-lookup"><span data-stu-id="93ac7-133">A view-only sharing link, allowing read-only access.</span></span>
| `edit`  | `write` | <span data-ttu-id="93ac7-134">Ein Freigabelink zum Bearbeiten für Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="93ac7-134">An edit sharing link, allowing read-write access.</span></span>
| `embed` | `read`  | <span data-ttu-id="93ac7-135">Ein schreibgeschützter Freigablink, der zum Einbetten von Inhalten in einer Hostwebseite verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="93ac7-135">A view-only sharing link that can be used to embed content into a host webpage.</span></span> <span data-ttu-id="93ac7-136">Einbettlinks sind nicht für OneDrive for Business oder SharePoint verfügbar.</span><span class="sxs-lookup"><span data-stu-id="93ac7-136">Embed links are not available for OneDrive for Business or SharePoint.</span></span>

## <a name="scope-options"></a><span data-ttu-id="93ac7-137">Bereichsoptionen</span><span class="sxs-lookup"><span data-stu-id="93ac7-137">Scope options</span></span>

| <span data-ttu-id="93ac7-138">Wert</span><span class="sxs-lookup"><span data-stu-id="93ac7-138">Value</span></span>          | <span data-ttu-id="93ac7-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="93ac7-139">Description</span></span>
|:---------------|:------------------------------------------------------------
| `anonymous`    | <span data-ttu-id="93ac7-140">Jeder Benutzer mit den Link hat Zugriff, ohne Anmeldung.</span><span class="sxs-lookup"><span data-stu-id="93ac7-140">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="93ac7-141">Dies kann Personen außerhalb Ihrer Organisation enthalten.</span><span class="sxs-lookup"><span data-stu-id="93ac7-141">This may include people outside of your organization.</span></span>
| `organization` | <span data-ttu-id="93ac7-142">Den Link können alle Benutzer in Ihrer Organisation (Mandant) signiert um Zugriff zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="93ac7-142">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="93ac7-143">Nur in OneDrive für Unternehmen und SharePoint verfügbar.</span><span class="sxs-lookup"><span data-stu-id="93ac7-143">Only available in OneDrive for Business and SharePoint.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/sharinglink.md:
      Found potential enums in resource example that weren't defined in a table:(view,edit,embed) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/sharinglink.md:
      Found potential enums in resource example that weren't defined in a table:(anonymous,organization) are in resource, but () are in table"
  ],
  "tocPath": "Facets/SharingLink"
} -->
