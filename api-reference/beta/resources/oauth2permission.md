---
title: Ressourcentyp oAuth2Permission
description: Stellt ein OAuth 2.0 delegiert Berechtigungsbereich. Die angegebene OAuth 2.0-Clientanwendungen (über die **RequiredResourceAccess** -Auflistung für das Application-Objekt) delegierte berechtigungsbereiche angefordert werden können beim Aufruf von einer Anwendung für die Ressource. Die **AppRoles** -Eigenschaft der Entität ServicePrincipal und der Anwendung Entität ist eine Auflistung von **oAuth2Permission**.
localization_priority: Normal
ms.openlocfilehash: 420a7b181aa2590d3c5bc8eaa7f104251915ae0f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829708"
---
# <a name="oauth2permission-resource-type"></a><span data-ttu-id="e5186-105">Ressourcentyp oAuth2Permission</span><span class="sxs-lookup"><span data-stu-id="e5186-105">oAuth2Permission resource type</span></span>

> <span data-ttu-id="e5186-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e5186-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5186-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e5186-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e5186-108">Stellt ein OAuth 2.0 delegiert Berechtigungsbereich.</span><span class="sxs-lookup"><span data-stu-id="e5186-108">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="e5186-109">Die angegebene OAuth 2.0-Clientanwendungen (über die **RequiredResourceAccess** -Auflistung für das [Application](application.md) -Objekt) delegierte berechtigungsbereiche angefordert werden können beim Aufruf von einer Anwendung für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="e5186-109">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="e5186-110">Die **AppRoles** -Eigenschaft der Entität [ServicePrincipal](serviceprincipal.md) und der [Anwendung](application.md) Entität ist eine Auflistung von **oAuth2Permission**.</span><span class="sxs-lookup"><span data-stu-id="e5186-110">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **oAuth2Permission**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e5186-111">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e5186-111">JSON representation</span></span>

<span data-ttu-id="e5186-112">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e5186-112">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2Permission"
}-->

```json
{
  "adminConsentDescription": "string",
  "adminConsentDisplayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "type": "string",
  "userConsentDescription": "string",
  "userConsentDisplayName": "string",
  "value": "string"
}

```
## <a name="properties"></a><span data-ttu-id="e5186-113">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e5186-113">Properties</span></span>
| <span data-ttu-id="e5186-114">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e5186-114">Property</span></span>     | <span data-ttu-id="e5186-115">Typ</span><span class="sxs-lookup"><span data-stu-id="e5186-115">Type</span></span>   |<span data-ttu-id="e5186-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e5186-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5186-117">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="e5186-117">adminConsentDescription</span></span>|<span data-ttu-id="e5186-118">String</span><span class="sxs-lookup"><span data-stu-id="e5186-118">String</span></span>|<span data-ttu-id="e5186-119">Berechtigung Hilfetext, der in der Admin Zustimmung und app-Zuordnung Erfahrungen angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="e5186-119">Permission help text that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="e5186-120">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="e5186-120">adminConsentDisplayName</span></span>|<span data-ttu-id="e5186-121">String</span><span class="sxs-lookup"><span data-stu-id="e5186-121">String</span></span>|<span data-ttu-id="e5186-122">Der Anzeigename für die Berechtigung, die in der Admin Zustimmung und app-Zuordnung Erfahrungen angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="e5186-122">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="e5186-123">id</span><span class="sxs-lookup"><span data-stu-id="e5186-123">id</span></span>|<span data-ttu-id="e5186-124">Guid</span><span class="sxs-lookup"><span data-stu-id="e5186-124">Guid</span></span>|<span data-ttu-id="e5186-125">Eindeutige Berechtigungen Bereichsbezeichner innerhalb der oauth2Permissions-Auflistung.</span><span class="sxs-lookup"><span data-stu-id="e5186-125">Unique scope permission identifier inside the oauth2Permissions collection.</span></span>|
|<span data-ttu-id="e5186-126">isEnabled</span><span class="sxs-lookup"><span data-stu-id="e5186-126">isEnabled</span></span>|<span data-ttu-id="e5186-127">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e5186-127">Boolean</span></span>|<span data-ttu-id="e5186-128">Beim Erstellen oder aktualisieren eine Berechtigung, muss diese Eigenschaft auf **true** festgelegt werden (die Standardeinstellung ist).</span><span class="sxs-lookup"><span data-stu-id="e5186-128">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="e5186-129">Um eine Berechtigung zu löschen, muss zuerst diese Eigenschaft auf **false**festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="e5186-129">To delete a permission, this property must first be set to **false**.</span></span>  <span data-ttu-id="e5186-130">An dieser Stelle kann im Gespräch nachfolgende die Berechtigung entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="e5186-130">At that point, in a subsequent call, the permission may be removed.</span></span>|
|<span data-ttu-id="e5186-131">type</span><span class="sxs-lookup"><span data-stu-id="e5186-131">type</span></span>|<span data-ttu-id="e5186-132">String</span><span class="sxs-lookup"><span data-stu-id="e5186-132">String</span></span>|<span data-ttu-id="e5186-133">Gibt an, von einem Endbenutzer gibt an, ob diese Berechtigung Bereich zugestimmt kann oder gibt an, ob eine gesamte Mandanten Berechtigung ist, die ein Unternehmensadministrator zugestimmt werden muss.</span><span class="sxs-lookup"><span data-stu-id="e5186-133">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a Company Administrator.</span></span>  <span data-ttu-id="e5186-134">Mögliche Werte sind "User" oder "Admin".</span><span class="sxs-lookup"><span data-stu-id="e5186-134">Possible values are "User" or "Admin".</span></span>|
|<span data-ttu-id="e5186-135">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="e5186-135">userConsentDescription</span></span>|<span data-ttu-id="e5186-136">String</span><span class="sxs-lookup"><span data-stu-id="e5186-136">String</span></span>|<span data-ttu-id="e5186-137">Berechtigung Hilfe in Zustimmung des Endbenutzers angezeigte Text.</span><span class="sxs-lookup"><span data-stu-id="e5186-137">Permission help text that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="e5186-138">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="e5186-138">userConsentDisplayName</span></span>|<span data-ttu-id="e5186-139">String</span><span class="sxs-lookup"><span data-stu-id="e5186-139">String</span></span>|<span data-ttu-id="e5186-140">Der Anzeigename für die Berechtigung, die in Zustimmung des Endbenutzers angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="e5186-140">Display name for the permission that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="e5186-141">Wert</span><span class="sxs-lookup"><span data-stu-id="e5186-141">value</span></span>|<span data-ttu-id="e5186-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e5186-142">String</span></span>|<span data-ttu-id="e5186-143">Der Wert des Bereichs geltend, dass die Anwendung für die Ressource in das OAuth 2.0-Zugriffstoken erwarten.</span><span class="sxs-lookup"><span data-stu-id="e5186-143">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oAuth2Permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
