---
title: Ressourcentyp oAuth2Permission
description: Stellt ein OAuth 2.0 delegiert Berechtigungsbereich. Die angegebene OAuth 2.0-Clientanwendungen (über die **RequiredResourceAccess** -Auflistung für das Application-Objekt) delegierte berechtigungsbereiche angefordert werden können beim Aufruf von einer Anwendung für die Ressource. Die **AppRoles** -Eigenschaft der Entität ServicePrincipal und der Anwendung Entität ist eine Auflistung von **oAuth2Permission**.
ms.openlocfilehash: 4a790c935dd84fb7bd4e1422ca59914d9a319ae9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063633"
---
# <a name="oauth2permission-resource-type"></a><span data-ttu-id="86ff8-105">Ressourcentyp oAuth2Permission</span><span class="sxs-lookup"><span data-stu-id="86ff8-105">oAuth2Permission resource type</span></span>

> <span data-ttu-id="86ff8-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="86ff8-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="86ff8-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="86ff8-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="86ff8-108">Stellt ein OAuth 2.0 delegiert Berechtigungsbereich.</span><span class="sxs-lookup"><span data-stu-id="86ff8-108">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="86ff8-109">Die angegebene OAuth 2.0-Clientanwendungen (über die **RequiredResourceAccess** -Auflistung für das [Application](application.md) -Objekt) delegierte berechtigungsbereiche angefordert werden können beim Aufruf von einer Anwendung für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="86ff8-109">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="86ff8-110">Die **AppRoles** -Eigenschaft der Entität [ServicePrincipal](serviceprincipal.md) und der [Anwendung](application.md) Entität ist eine Auflistung von **oAuth2Permission**.</span><span class="sxs-lookup"><span data-stu-id="86ff8-110">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **oAuth2Permission**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="86ff8-111">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="86ff8-111">JSON representation</span></span>

<span data-ttu-id="86ff8-112">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="86ff8-112">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="86ff8-113">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="86ff8-113">Properties</span></span>
| <span data-ttu-id="86ff8-114">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="86ff8-114">Property</span></span>     | <span data-ttu-id="86ff8-115">Typ</span><span class="sxs-lookup"><span data-stu-id="86ff8-115">Type</span></span>   |<span data-ttu-id="86ff8-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="86ff8-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86ff8-117">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="86ff8-117">adminConsentDescription</span></span>|<span data-ttu-id="86ff8-118">String</span><span class="sxs-lookup"><span data-stu-id="86ff8-118">String</span></span>|<span data-ttu-id="86ff8-119">Berechtigung Hilfetext, der in der Admin Zustimmung und app-Zuordnung Erfahrungen angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="86ff8-119">Permission help text that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="86ff8-120">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="86ff8-120">adminConsentDisplayName</span></span>|<span data-ttu-id="86ff8-121">String</span><span class="sxs-lookup"><span data-stu-id="86ff8-121">String</span></span>|<span data-ttu-id="86ff8-122">Der Anzeigename für die Berechtigung, die in der Admin Zustimmung und app-Zuordnung Erfahrungen angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="86ff8-122">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="86ff8-123">id</span><span class="sxs-lookup"><span data-stu-id="86ff8-123">id</span></span>|<span data-ttu-id="86ff8-124">Guid</span><span class="sxs-lookup"><span data-stu-id="86ff8-124">Guid</span></span>|<span data-ttu-id="86ff8-125">Eindeutige Berechtigungen Bereichsbezeichner innerhalb der oauth2Permissions-Auflistung.</span><span class="sxs-lookup"><span data-stu-id="86ff8-125">Unique scope permission identifier inside the oauth2Permissions collection.</span></span>|
|<span data-ttu-id="86ff8-126">isEnabled</span><span class="sxs-lookup"><span data-stu-id="86ff8-126">isEnabled</span></span>|<span data-ttu-id="86ff8-127">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="86ff8-127">Boolean</span></span>|<span data-ttu-id="86ff8-128">Beim Erstellen oder aktualisieren eine Berechtigung, muss diese Eigenschaft auf **true** festgelegt werden (die Standardeinstellung ist).</span><span class="sxs-lookup"><span data-stu-id="86ff8-128">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="86ff8-129">Um eine Berechtigung zu löschen, muss zuerst diese Eigenschaft auf **false**festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="86ff8-129">To delete a permission, this property must first be set to **false**.</span></span>  <span data-ttu-id="86ff8-130">An dieser Stelle kann im Gespräch nachfolgende die Berechtigung entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="86ff8-130">At that point, in a subsequent call, the permission may be removed.</span></span>|
|<span data-ttu-id="86ff8-131">Typ</span><span class="sxs-lookup"><span data-stu-id="86ff8-131">type</span></span>|<span data-ttu-id="86ff8-132">String</span><span class="sxs-lookup"><span data-stu-id="86ff8-132">String</span></span>|<span data-ttu-id="86ff8-133">Gibt an, von einem Endbenutzer gibt an, ob diese Berechtigung Bereich zugestimmt kann oder gibt an, ob eine gesamte Mandanten Berechtigung ist, die ein Unternehmensadministrator zugestimmt werden muss.</span><span class="sxs-lookup"><span data-stu-id="86ff8-133">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a Company Administrator.</span></span>  <span data-ttu-id="86ff8-134">Mögliche Werte sind "User" oder "Admin".</span><span class="sxs-lookup"><span data-stu-id="86ff8-134">Possible values are "User" or "Admin".</span></span>|
|<span data-ttu-id="86ff8-135">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="86ff8-135">userConsentDescription</span></span>|<span data-ttu-id="86ff8-136">String</span><span class="sxs-lookup"><span data-stu-id="86ff8-136">String</span></span>|<span data-ttu-id="86ff8-137">Berechtigung Hilfe in Zustimmung des Endbenutzers angezeigte Text.</span><span class="sxs-lookup"><span data-stu-id="86ff8-137">Permission help text that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="86ff8-138">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="86ff8-138">userConsentDisplayName</span></span>|<span data-ttu-id="86ff8-139">String</span><span class="sxs-lookup"><span data-stu-id="86ff8-139">String</span></span>|<span data-ttu-id="86ff8-140">Der Anzeigename für die Berechtigung, die in Zustimmung des Endbenutzers angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="86ff8-140">Display name for the permission that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="86ff8-141">Wert</span><span class="sxs-lookup"><span data-stu-id="86ff8-141">value</span></span>|<span data-ttu-id="86ff8-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="86ff8-142">String</span></span>|<span data-ttu-id="86ff8-143">Der Wert des Bereichs geltend, dass die Anwendung für die Ressource in das OAuth 2.0-Zugriffstoken erwarten.</span><span class="sxs-lookup"><span data-stu-id="86ff8-143">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oAuth2Permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
