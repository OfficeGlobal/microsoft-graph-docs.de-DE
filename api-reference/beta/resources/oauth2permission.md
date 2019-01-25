---
title: Ressourcentyp oAuth2Permission
description: Stellt ein OAuth 2.0 delegiert Berechtigungsbereich. Die angegebene OAuth 2.0-Clientanwendungen (über die **RequiredResourceAccess** -Auflistung für das Application-Objekt) delegierte berechtigungsbereiche angefordert werden können beim Aufruf von einer Anwendung für die Ressource. Die **AppRoles** -Eigenschaft der Entität ServicePrincipal und der Anwendung Entität ist eine Auflistung von **oAuth2Permission**.
localization_priority: Normal
ms.openlocfilehash: 8d8bb0bb5af17b7322bd6be37ac48ae9edbeba42
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510813"
---
# <a name="oauth2permission-resource-type"></a><span data-ttu-id="b4aa6-105">Ressourcentyp oAuth2Permission</span><span class="sxs-lookup"><span data-stu-id="b4aa6-105">oAuth2Permission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4aa6-106">Stellt ein OAuth 2.0 delegiert Berechtigungsbereich.</span><span class="sxs-lookup"><span data-stu-id="b4aa6-106">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="b4aa6-107">Die angegebene OAuth 2.0-Clientanwendungen (über die **RequiredResourceAccess** -Auflistung für das [Application](application.md) -Objekt) delegierte berechtigungsbereiche angefordert werden können beim Aufruf von einer Anwendung für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="b4aa6-107">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="b4aa6-108">Die **AppRoles** -Eigenschaft der Entität [ServicePrincipal](serviceprincipal.md) und der [Anwendung](application.md) Entität ist eine Auflistung von **oAuth2Permission**.</span><span class="sxs-lookup"><span data-stu-id="b4aa6-108">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **oAuth2Permission**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="b4aa6-109">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b4aa6-109">JSON representation</span></span>

<span data-ttu-id="b4aa6-110">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b4aa6-110">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="b4aa6-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b4aa6-111">Properties</span></span>
| <span data-ttu-id="b4aa6-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b4aa6-112">Property</span></span>     | <span data-ttu-id="b4aa6-113">Typ</span><span class="sxs-lookup"><span data-stu-id="b4aa6-113">Type</span></span>   |<span data-ttu-id="b4aa6-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4aa6-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4aa6-115">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="b4aa6-115">adminConsentDescription</span></span>|<span data-ttu-id="b4aa6-116">String</span><span class="sxs-lookup"><span data-stu-id="b4aa6-116">String</span></span>|<span data-ttu-id="b4aa6-117">Berechtigung Hilfetext, der in der Admin Zustimmung und app-Zuordnung Erfahrungen angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="b4aa6-117">Permission help text that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="b4aa6-118">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="b4aa6-118">adminConsentDisplayName</span></span>|<span data-ttu-id="b4aa6-119">String</span><span class="sxs-lookup"><span data-stu-id="b4aa6-119">String</span></span>|<span data-ttu-id="b4aa6-120">Der Anzeigename für die Berechtigung, die in der Admin Zustimmung und app-Zuordnung Erfahrungen angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="b4aa6-120">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="b4aa6-121">id</span><span class="sxs-lookup"><span data-stu-id="b4aa6-121">id</span></span>|<span data-ttu-id="b4aa6-122">Guid</span><span class="sxs-lookup"><span data-stu-id="b4aa6-122">Guid</span></span>|<span data-ttu-id="b4aa6-123">Eindeutige Berechtigungen Bereichsbezeichner innerhalb der oauth2Permissions-Auflistung.</span><span class="sxs-lookup"><span data-stu-id="b4aa6-123">Unique scope permission identifier inside the oauth2Permissions collection.</span></span>|
|<span data-ttu-id="b4aa6-124">isEnabled</span><span class="sxs-lookup"><span data-stu-id="b4aa6-124">isEnabled</span></span>|<span data-ttu-id="b4aa6-125">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4aa6-125">Boolean</span></span>|<span data-ttu-id="b4aa6-126">Beim Erstellen oder aktualisieren eine Berechtigung, muss diese Eigenschaft auf **true** festgelegt werden (die Standardeinstellung ist).</span><span class="sxs-lookup"><span data-stu-id="b4aa6-126">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="b4aa6-127">Um eine Berechtigung zu löschen, muss zuerst diese Eigenschaft auf **false**festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="b4aa6-127">To delete a permission, this property must first be set to **false**.</span></span>  <span data-ttu-id="b4aa6-128">An dieser Stelle kann im Gespräch nachfolgende die Berechtigung entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="b4aa6-128">At that point, in a subsequent call, the permission may be removed.</span></span>|
|<span data-ttu-id="b4aa6-129">type</span><span class="sxs-lookup"><span data-stu-id="b4aa6-129">type</span></span>|<span data-ttu-id="b4aa6-130">String</span><span class="sxs-lookup"><span data-stu-id="b4aa6-130">String</span></span>|<span data-ttu-id="b4aa6-131">Gibt an, von einem Endbenutzer gibt an, ob diese Berechtigung Bereich zugestimmt kann oder gibt an, ob eine gesamte Mandanten Berechtigung ist, die ein Unternehmensadministrator zugestimmt werden muss.</span><span class="sxs-lookup"><span data-stu-id="b4aa6-131">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a Company Administrator.</span></span>  <span data-ttu-id="b4aa6-132">Mögliche Werte sind "User" oder "Admin".</span><span class="sxs-lookup"><span data-stu-id="b4aa6-132">Possible values are "User" or "Admin".</span></span>|
|<span data-ttu-id="b4aa6-133">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="b4aa6-133">userConsentDescription</span></span>|<span data-ttu-id="b4aa6-134">String</span><span class="sxs-lookup"><span data-stu-id="b4aa6-134">String</span></span>|<span data-ttu-id="b4aa6-135">Berechtigung Hilfe in Zustimmung des Endbenutzers angezeigte Text.</span><span class="sxs-lookup"><span data-stu-id="b4aa6-135">Permission help text that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="b4aa6-136">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="b4aa6-136">userConsentDisplayName</span></span>|<span data-ttu-id="b4aa6-137">String</span><span class="sxs-lookup"><span data-stu-id="b4aa6-137">String</span></span>|<span data-ttu-id="b4aa6-138">Der Anzeigename für die Berechtigung, die in Zustimmung des Endbenutzers angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="b4aa6-138">Display name for the permission that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="b4aa6-139">Wert</span><span class="sxs-lookup"><span data-stu-id="b4aa6-139">value</span></span>|<span data-ttu-id="b4aa6-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4aa6-140">String</span></span>|<span data-ttu-id="b4aa6-141">Der Wert des Bereichs geltend, dass die Anwendung für die Ressource in das OAuth 2.0-Zugriffstoken erwarten.</span><span class="sxs-lookup"><span data-stu-id="b4aa6-141">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2Permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/oauth2permission.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
