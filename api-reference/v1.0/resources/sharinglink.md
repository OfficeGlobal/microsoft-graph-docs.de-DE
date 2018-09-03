---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingLink
ms.openlocfilehash: 7639dab9f63a948b3e9a849d8d320de60f5a0954
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23270489"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="04462-102">SharingLink-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="04462-102">SharingLink resource type</span></span>

<span data-ttu-id="04462-103">Die **SharingLink**-Ressource gruppiert linkbezogene Datenelemente in einer einzelnen Struktur.</span><span class="sxs-lookup"><span data-stu-id="04462-103">The **SharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="04462-104">Wenn eine [**Permission**](permission.md)-Ressource ein **sharingLink**-Facet ungleich Null aufweist, stellt die Berechtigung einen Freigabelink dar (im Gegensatz zu Berechtigungen, die einer Person oder Gruppe erteilten werden).</span><span class="sxs-lookup"><span data-stu-id="04462-104">If a [**Permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="04462-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="04462-105">JSON representation</span></span>

<span data-ttu-id="04462-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="04462-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="04462-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="04462-107">Properties</span></span>

| <span data-ttu-id="04462-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="04462-108">Property</span></span>    | <span data-ttu-id="04462-109">Typ</span><span class="sxs-lookup"><span data-stu-id="04462-109">Type</span></span>          | <span data-ttu-id="04462-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04462-110">Description</span></span>
|:------------|:--------------|:-------------------------------------
| <span data-ttu-id="04462-111">Anwendung</span><span class="sxs-lookup"><span data-stu-id="04462-111">application</span></span> | <span data-ttu-id="04462-112">[Identität][]</span><span class="sxs-lookup"><span data-stu-id="04462-112">[identity][]</span></span>  | <span data-ttu-id="04462-113">Die App, der der Link zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="04462-113">The app the link is associated with.</span></span>
| <span data-ttu-id="04462-114">Typ</span><span class="sxs-lookup"><span data-stu-id="04462-114">type</span></span>        | <span data-ttu-id="04462-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="04462-115">String</span></span>        | <span data-ttu-id="04462-116">Der Typ des erstellten Links.</span><span class="sxs-lookup"><span data-stu-id="04462-116">The type of the link created.</span></span>
| <span data-ttu-id="04462-117">Bereich</span><span class="sxs-lookup"><span data-stu-id="04462-117">scope</span></span>       | <span data-ttu-id="04462-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="04462-118">String</span></span>        | <span data-ttu-id="04462-p101">Der Bereich des Links, der durch diese Berechtigung dargestellt wird. Der Wert `anonymous` gibt an, dass der Link von jedem Benutzer verwendet werden kann. `organization` gibt an, dass der Link von Benutzern verwendet werden kann, die bei dem gleichen Mandanten angemeldet sind.</span><span class="sxs-lookup"><span data-stu-id="04462-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="04462-121">webHtml</span><span class="sxs-lookup"><span data-stu-id="04462-121">webHtml</span></span>     | <span data-ttu-id="04462-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="04462-122">String</span></span>        | <span data-ttu-id="04462-123">Bei `embed` Links enthält diese Eigenschaft den HTML-Code für ein `<iframe>`-Element, das das Element in eine Webseite einbettet.</span><span class="sxs-lookup"><span data-stu-id="04462-123">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="04462-124">webUrl</span><span class="sxs-lookup"><span data-stu-id="04462-124">webUrl</span></span>      | <span data-ttu-id="04462-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="04462-125">String</span></span>        | <span data-ttu-id="04462-126">Eine URL, mit der das Element im Browser auf der OneDrive-Website geöffnet wird.</span><span class="sxs-lookup"><span data-stu-id="04462-126">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identität]: identity.md
[Identity]: identity.md

## <a name="type-options"></a><span data-ttu-id="04462-128">Typ-Optionen</span><span class="sxs-lookup"><span data-stu-id="04462-128">Type options</span></span>

<span data-ttu-id="04462-129">In dieser Tabelle werden zulässige Werte für die **type**-Eigenschaft aufgeführt:</span><span class="sxs-lookup"><span data-stu-id="04462-129">This table defines the possible values for the **type** property:</span></span>

| <span data-ttu-id="04462-130">Wert</span><span class="sxs-lookup"><span data-stu-id="04462-130">Value</span></span>   | <span data-ttu-id="04462-131">Funktion</span><span class="sxs-lookup"><span data-stu-id="04462-131">Role</span></span>    | <span data-ttu-id="04462-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04462-132">Description</span></span>
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | <span data-ttu-id="04462-133">Ein Freigabelink zum Anzeigen für schreibgeschützten Zugriff.</span><span class="sxs-lookup"><span data-stu-id="04462-133">A view-only sharing link, allowing read-only access.</span></span>
| `edit`  | `write` | <span data-ttu-id="04462-134">Ein Freigabelink zum Bearbeiten für Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="04462-134">An edit sharing link, allowing read-write access.</span></span>
| `embed` | `read`  | <span data-ttu-id="04462-135">Ein schreibgeschützter Freigablink, der zum Einbetten von Inhalten in einer Hostwebseite verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="04462-135">A view-only sharing link that can be used to embed content into a host webpage.</span></span> <span data-ttu-id="04462-136">Eingebettete Links sind nicht für OneDrive for Business oder SharePoint verfügbar.</span><span class="sxs-lookup"><span data-stu-id="04462-136">Embed links are not available for OneDrive for Business or SharePoint.</span></span>

## <a name="scope-options"></a><span data-ttu-id="04462-137">Bereichsoptionen</span><span class="sxs-lookup"><span data-stu-id="04462-137">Scope options folder</span></span>

| <span data-ttu-id="04462-138">Wert</span><span class="sxs-lookup"><span data-stu-id="04462-138">Value</span></span>          | <span data-ttu-id="04462-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04462-139">Description</span></span>
|:---------------|:------------------------------------------------------------
| `anonymous`    | <span data-ttu-id="04462-140">Jeder Benutzer mit dem Link hat Zugriff, ohne sich anmelden zu müssen.</span><span class="sxs-lookup"><span data-stu-id="04462-140">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="04462-141">Hierzu können auch Personen außerhalb Ihrer Organisation zählen.</span><span class="sxs-lookup"><span data-stu-id="04462-141">This may include people outside of your organization.</span></span>
| `organization` | <span data-ttu-id="04462-142">Alle Benutzer, die in Ihrer Organisation (Mandant) angemeldet sind, können den Link benutzen, um Zugriff zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="04462-142">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="04462-143">Nur in OneDrivefor Business und SharePoint verfügbar.</span><span class="sxs-lookup"><span data-stu-id="04462-143">Only available in OneDrive for Business and SharePoint.</span></span>

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
