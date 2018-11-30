---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingLink
ms.openlocfilehash: 7b7729899d134fa1d5de7debb1f209ec5aadd70d
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="df7dd-102">SharingLink-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="df7dd-102">SharingLink resource type</span></span>

<span data-ttu-id="df7dd-103">Die **SharingLink**-Ressource gruppiert linkbezogene Datenelemente in einer einzelnen Struktur.</span><span class="sxs-lookup"><span data-stu-id="df7dd-103">The **SharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="df7dd-104">Wenn eine [**Permission**](permission.md)-Ressource ein **sharingLink**-Facet ungleich Null aufweist, stellt die Berechtigung einen Freigabelink dar (im Gegensatz zu Berechtigungen, die einer Person oder Gruppe erteilten werden).</span><span class="sxs-lookup"><span data-stu-id="df7dd-104">If a [**Permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="df7dd-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="df7dd-105">JSON representation</span></span>

<span data-ttu-id="df7dd-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="df7dd-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="df7dd-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="df7dd-107">Properties</span></span>

| <span data-ttu-id="df7dd-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="df7dd-108">Property</span></span>    | <span data-ttu-id="df7dd-109">Typ</span><span class="sxs-lookup"><span data-stu-id="df7dd-109">Type</span></span>          | <span data-ttu-id="df7dd-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="df7dd-110">Description</span></span>
|:------------|:--------------|:-------------------------------------
| <span data-ttu-id="df7dd-111">application</span><span class="sxs-lookup"><span data-stu-id="df7dd-111">application</span></span> | <span data-ttu-id="df7dd-112">[Identität][]</span><span class="sxs-lookup"><span data-stu-id="df7dd-112">[identity][]</span></span>  | <span data-ttu-id="df7dd-113">Die App, der der Link zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="df7dd-113">The app the link is associated with.</span></span>
| <span data-ttu-id="df7dd-114">type</span><span class="sxs-lookup"><span data-stu-id="df7dd-114">type</span></span>        | <span data-ttu-id="df7dd-115">String</span><span class="sxs-lookup"><span data-stu-id="df7dd-115">String</span></span>        | <span data-ttu-id="df7dd-116">Der Typ des erstellten Links.</span><span class="sxs-lookup"><span data-stu-id="df7dd-116">The type of the link created.</span></span>
| <span data-ttu-id="df7dd-117">scope</span><span class="sxs-lookup"><span data-stu-id="df7dd-117">scope</span></span>       | <span data-ttu-id="df7dd-118">String</span><span class="sxs-lookup"><span data-stu-id="df7dd-118">String</span></span>        | <span data-ttu-id="df7dd-p101">Der Bereich des Links, der durch diese Berechtigung dargestellt wird. Der Wert `anonymous` gibt an, dass der Link von jedem Benutzer verwendet werden kann. `organization` gibt an, dass der Link von Benutzern verwendet werden kann, die bei dem gleichen Mandanten angemeldet sind.</span><span class="sxs-lookup"><span data-stu-id="df7dd-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="df7dd-121">webHtml</span><span class="sxs-lookup"><span data-stu-id="df7dd-121">webHtml</span></span>     | <span data-ttu-id="df7dd-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="df7dd-122">String</span></span>        | <span data-ttu-id="df7dd-123">Bei `embed` Links enthält diese Eigenschaft den HTML-Code für ein `<iframe>`-Element, das das Element in eine Webseite einbettet.</span><span class="sxs-lookup"><span data-stu-id="df7dd-123">For embeddable links, this property contains the HTML code for an  element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="df7dd-124">webUrl</span><span class="sxs-lookup"><span data-stu-id="df7dd-124">webUrl</span></span>      | <span data-ttu-id="df7dd-125">String</span><span class="sxs-lookup"><span data-stu-id="df7dd-125">String</span></span>        | <span data-ttu-id="df7dd-126">Eine URL, mit der das Element im Browser auf der OneDrive-Website geöffnet wird.</span><span class="sxs-lookup"><span data-stu-id="df7dd-126">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

## <a name="type-enumeration"></a><span data-ttu-id="df7dd-128">Type-Enumeration</span><span class="sxs-lookup"><span data-stu-id="df7dd-128">Type enumeration</span></span>

<span data-ttu-id="df7dd-129">In dieser Tabelle werden zulässige Werte für die **type**-Eigenschaft aufgeführt:</span><span class="sxs-lookup"><span data-stu-id="df7dd-129">This table defines the possible values for the **type** property:</span></span>

| <span data-ttu-id="df7dd-130">Wert</span><span class="sxs-lookup"><span data-stu-id="df7dd-130">Value</span></span>   | <span data-ttu-id="df7dd-131">Funktion</span><span class="sxs-lookup"><span data-stu-id="df7dd-131">Role</span></span>    | <span data-ttu-id="df7dd-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="df7dd-132">Description</span></span>
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | <span data-ttu-id="df7dd-133">Ein Freigabelink zum Anzeigen für schreibgeschützten Zugriff.</span><span class="sxs-lookup"><span data-stu-id="df7dd-133">A view-only sharing link, allowing read-only access.</span></span>
| `edit`  | `write` | <span data-ttu-id="df7dd-134">Ein Freigabelink zum Bearbeiten für Lese-/Schreibzugriff.</span><span class="sxs-lookup"><span data-stu-id="df7dd-134">An edit sharing link, allowing read-write access.</span></span>
| `embed` | `read`  | <span data-ttu-id="df7dd-135">Ein schreibgeschützter Freigablink, der zum Einbetten von Inhalten in einer Hostwebseite verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="df7dd-135">A view-only sharing link that can be used to embed content into a host webpage.</span></span> <span data-ttu-id="df7dd-136">Einbettlinks sind nicht für OneDrive for Business oder SharePoint verfügbar.</span><span class="sxs-lookup"><span data-stu-id="df7dd-136">Embed links are not available for OneDrive for Business or SharePoint.</span></span>

## <a name="scope-enumeration"></a><span data-ttu-id="df7dd-137">Scope-Enumeration</span><span class="sxs-lookup"><span data-stu-id="df7dd-137">Scope enumeration</span></span>

| <span data-ttu-id="df7dd-138">Wert</span><span class="sxs-lookup"><span data-stu-id="df7dd-138">Value</span></span>          | <span data-ttu-id="df7dd-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="df7dd-139">Description</span></span>                                                                                                                 |
|:---------------|:----------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="df7dd-140">Der Freigabelink steht für alle Benutzer zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="df7dd-140">The sharing link is available for anyone to use.</span></span>                                                                            |
| `organization` | <span data-ttu-id="df7dd-p103">Der Freigabelink steht für Benutzer in derselben Organisation (Mandant) zur Verfügung. Nicht für OneDrive Personal verfügbar.</span><span class="sxs-lookup"><span data-stu-id="df7dd-p103">The sharing link is available for anyone within the same organization (tenant) to use. Not available for OneDrive Personal.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "tocPath": "Facets/SharingLink"
} -->
