---
title: Ressourcentyp permissionScope
description: Stellt ein OAuth 2.0 delegiert Berechtigungsbereich. Die angegebene OAuth 2.0-Clientanwendungen (über die **RequiredResourceAccess** -Auflistung für das Application-Objekt) delegierte berechtigungsbereiche angefordert werden können beim Aufruf von einer Anwendung für die Ressource. Die **oauth2Permissions** -Eigenschaft der Entität ServicePrincipal und der Anwendung Entität ist eine Auflistung von **OAuth2Permission**.
localization_priority: Normal
ms.openlocfilehash: a294316f5c6255d0873ce0dbe809c33dad89ae08
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818151"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="c2404-105">Ressourcentyp permissionScope</span><span class="sxs-lookup"><span data-stu-id="c2404-105">permissionScope resource type</span></span>

> <span data-ttu-id="c2404-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c2404-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2404-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c2404-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c2404-108">Stellt ein OAuth 2.0 delegiert Berechtigungsbereich.</span><span class="sxs-lookup"><span data-stu-id="c2404-108">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="c2404-109">Die angegebene OAuth 2.0-Clientanwendungen (über die **RequiredResourceAccess** -Auflistung für das [Application](application.md) -Objekt) delegierte berechtigungsbereiche angefordert werden können beim Aufruf von einer Anwendung für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="c2404-109">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [Application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="c2404-110">Die **oauth2Permissions** -Eigenschaft der Entität [ServicePrincipal](serviceprincipal.md) und der [Anwendung](application.md) Entität ist eine Auflistung von **OAuth2Permission**.</span><span class="sxs-lookup"><span data-stu-id="c2404-110">The **oauth2Permissions** property of the [ServicePrincipal](serviceprincipal.md) entity and of the [Application](application.md) entity is a collection of **OAuth2Permission**.</span></span>

## <a name="properties"></a><span data-ttu-id="c2404-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c2404-111">Properties</span></span>

| <span data-ttu-id="c2404-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c2404-112">Property</span></span> | <span data-ttu-id="c2404-113">Typ</span><span class="sxs-lookup"><span data-stu-id="c2404-113">Type</span></span> | <span data-ttu-id="c2404-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c2404-114">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c2404-115">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="c2404-115">adminConsentDescription</span></span>|<span data-ttu-id="c2404-116">String</span><span class="sxs-lookup"><span data-stu-id="c2404-116">String</span></span>| <span data-ttu-id="c2404-117">Berechtigung Hilfetext, der in der Admin Zustimmung und app-Zuordnung Erfahrungen angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="c2404-117">Permission help text that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="c2404-118">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="c2404-118">adminConsentDisplayName</span></span>|<span data-ttu-id="c2404-119">String</span><span class="sxs-lookup"><span data-stu-id="c2404-119">String</span></span>| <span data-ttu-id="c2404-120">Der Anzeigename für die Berechtigung, die in der Admin Zustimmung und app-Zuordnung Erfahrungen angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="c2404-120">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="c2404-121">id</span><span class="sxs-lookup"><span data-stu-id="c2404-121">id</span></span>|<span data-ttu-id="c2404-122">Guid</span><span class="sxs-lookup"><span data-stu-id="c2404-122">Guid</span></span>| <span data-ttu-id="c2404-123">Eindeutige Berechtigungen Bereichsbezeichner innerhalb der oauth2Permissions-Auflistung.</span><span class="sxs-lookup"><span data-stu-id="c2404-123">Unique scope permission identifier inside the oauth2Permissions collection.</span></span> |
|<span data-ttu-id="c2404-124">isEnabled</span><span class="sxs-lookup"><span data-stu-id="c2404-124">isEnabled</span></span>|<span data-ttu-id="c2404-125">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c2404-125">Boolean</span></span>| <span data-ttu-id="c2404-126">Beim Erstellen oder aktualisieren eine Berechtigung, muss diese Eigenschaft auf **true** festgelegt werden (die Standardeinstellung ist).</span><span class="sxs-lookup"><span data-stu-id="c2404-126">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="c2404-127">Um eine Berechtigung zu löschen, muss zuerst diese Eigenschaft auf **false**festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="c2404-127">To delete a permission, this property must first be set to **false**.</span></span> <span data-ttu-id="c2404-128">An dieser Stelle kann im Gespräch nachfolgende die Berechtigung entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="c2404-128">At that point, in a subsequent call, the permission may be removed.</span></span> |
|<span data-ttu-id="c2404-129">Ursprung</span><span class="sxs-lookup"><span data-stu-id="c2404-129">origin</span></span>|<span data-ttu-id="c2404-130">String</span><span class="sxs-lookup"><span data-stu-id="c2404-130">String</span></span>| <span data-ttu-id="c2404-131">Für die interne Verwendung.</span><span class="sxs-lookup"><span data-stu-id="c2404-131">For internal use.</span></span> |
|<span data-ttu-id="c2404-132">type</span><span class="sxs-lookup"><span data-stu-id="c2404-132">type</span></span>|<span data-ttu-id="c2404-133">String</span><span class="sxs-lookup"><span data-stu-id="c2404-133">String</span></span>| <span data-ttu-id="c2404-134">Gibt an, von einem Endbenutzer gibt an, ob diese Berechtigung Bereich zugestimmt kann oder gibt an, ob eine gesamte Mandanten Berechtigung ist, die von einem Administrator der Firma zugestimmt werden muss.</span><span class="sxs-lookup"><span data-stu-id="c2404-134">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a company administrator.</span></span> <span data-ttu-id="c2404-135">Mögliche Werte sind *Benutzer* oder *Administrator*.</span><span class="sxs-lookup"><span data-stu-id="c2404-135">Possible values are *User* or *Admin*.</span></span> |
|<span data-ttu-id="c2404-136">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="c2404-136">userConsentDescription</span></span>|<span data-ttu-id="c2404-137">String</span><span class="sxs-lookup"><span data-stu-id="c2404-137">String</span></span>| <span data-ttu-id="c2404-138">Berechtigung Hilfetext, die in der Genehmigung durch den Endbenutzer angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="c2404-138">Permission help text that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="c2404-139">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="c2404-139">userConsentDisplayName</span></span>|<span data-ttu-id="c2404-140">String</span><span class="sxs-lookup"><span data-stu-id="c2404-140">String</span></span>| <span data-ttu-id="c2404-141">Der Anzeigename für die Berechtigung, die in der Genehmigung durch den Endbenutzer angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="c2404-141">Display name for the permission that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="c2404-142">Wert</span><span class="sxs-lookup"><span data-stu-id="c2404-142">value</span></span>|<span data-ttu-id="c2404-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c2404-143">String</span></span>| <span data-ttu-id="c2404-144">Der Wert des Bereichs geltend, dass die Anwendung für die Ressource in das OAuth 2.0-Zugriffstoken erwarten.</span><span class="sxs-lookup"><span data-stu-id="c2404-144">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c2404-145">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c2404-145">JSON representation</span></span>
<span data-ttu-id="c2404-146">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c2404-146">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.permissionScope"
}-->

```json
{
  "adminConsentDescription": "String",
  "adminConsentDisplayName": "String",
  "id": "Guid",
  "isEnabled": true,
  "origin": "String",
  "type": "String",
  "userConsentDescription": "String",
  "userConsentDisplayName": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "permissionScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
