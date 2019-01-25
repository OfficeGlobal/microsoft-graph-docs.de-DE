---
title: Ressourcentyp permissionScope
description: Stellt ein OAuth 2.0 delegiert Berechtigungsbereich. Die angegebene OAuth 2.0-Clientanwendungen (über die **RequiredResourceAccess** -Auflistung für das Application-Objekt) delegierte berechtigungsbereiche angefordert werden können beim Aufruf von einer Anwendung für die Ressource. Die **oauth2Permissions** -Eigenschaft der Entität ServicePrincipal und der Anwendung Entität ist eine Auflistung von **OAuth2Permission**.
localization_priority: Normal
ms.openlocfilehash: 00629a6e123ef19290d3c1bd4797e4bab3ce95c0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517078"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="9e0b3-105">Ressourcentyp permissionScope</span><span class="sxs-lookup"><span data-stu-id="9e0b3-105">permissionScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e0b3-106">Stellt ein OAuth 2.0 delegiert Berechtigungsbereich.</span><span class="sxs-lookup"><span data-stu-id="9e0b3-106">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="9e0b3-107">Die angegebene OAuth 2.0-Clientanwendungen (über die **RequiredResourceAccess** -Auflistung für das [Application](application.md) -Objekt) delegierte berechtigungsbereiche angefordert werden können beim Aufruf von einer Anwendung für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="9e0b3-107">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [Application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="9e0b3-108">Die **oauth2Permissions** -Eigenschaft der Entität [ServicePrincipal](serviceprincipal.md) und der [Anwendung](application.md) Entität ist eine Auflistung von **OAuth2Permission**.</span><span class="sxs-lookup"><span data-stu-id="9e0b3-108">The **oauth2Permissions** property of the [ServicePrincipal](serviceprincipal.md) entity and of the [Application](application.md) entity is a collection of **OAuth2Permission**.</span></span>

## <a name="properties"></a><span data-ttu-id="9e0b3-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9e0b3-109">Properties</span></span>

| <span data-ttu-id="9e0b3-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9e0b3-110">Property</span></span> | <span data-ttu-id="9e0b3-111">Typ</span><span class="sxs-lookup"><span data-stu-id="9e0b3-111">Type</span></span> | <span data-ttu-id="9e0b3-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9e0b3-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9e0b3-113">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="9e0b3-113">adminConsentDescription</span></span>|<span data-ttu-id="9e0b3-114">String</span><span class="sxs-lookup"><span data-stu-id="9e0b3-114">String</span></span>| <span data-ttu-id="9e0b3-115">Berechtigung Hilfetext, der in der Admin Zustimmung und app-Zuordnung Erfahrungen angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="9e0b3-115">Permission help text that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="9e0b3-116">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="9e0b3-116">adminConsentDisplayName</span></span>|<span data-ttu-id="9e0b3-117">String</span><span class="sxs-lookup"><span data-stu-id="9e0b3-117">String</span></span>| <span data-ttu-id="9e0b3-118">Der Anzeigename für die Berechtigung, die in der Admin Zustimmung und app-Zuordnung Erfahrungen angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="9e0b3-118">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="9e0b3-119">id</span><span class="sxs-lookup"><span data-stu-id="9e0b3-119">id</span></span>|<span data-ttu-id="9e0b3-120">Guid</span><span class="sxs-lookup"><span data-stu-id="9e0b3-120">Guid</span></span>| <span data-ttu-id="9e0b3-121">Eindeutige Berechtigungen Bereichsbezeichner innerhalb der oauth2Permissions-Auflistung.</span><span class="sxs-lookup"><span data-stu-id="9e0b3-121">Unique scope permission identifier inside the oauth2Permissions collection.</span></span> |
|<span data-ttu-id="9e0b3-122">isEnabled</span><span class="sxs-lookup"><span data-stu-id="9e0b3-122">isEnabled</span></span>|<span data-ttu-id="9e0b3-123">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9e0b3-123">Boolean</span></span>| <span data-ttu-id="9e0b3-124">Beim Erstellen oder aktualisieren eine Berechtigung, muss diese Eigenschaft auf **true** festgelegt werden (die Standardeinstellung ist).</span><span class="sxs-lookup"><span data-stu-id="9e0b3-124">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="9e0b3-125">Um eine Berechtigung zu löschen, muss zuerst diese Eigenschaft auf **false**festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="9e0b3-125">To delete a permission, this property must first be set to **false**.</span></span> <span data-ttu-id="9e0b3-126">An dieser Stelle kann im Gespräch nachfolgende die Berechtigung entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="9e0b3-126">At that point, in a subsequent call, the permission may be removed.</span></span> |
|<span data-ttu-id="9e0b3-127">Okeanos</span><span class="sxs-lookup"><span data-stu-id="9e0b3-127">origin</span></span>|<span data-ttu-id="9e0b3-128">String</span><span class="sxs-lookup"><span data-stu-id="9e0b3-128">String</span></span>| <span data-ttu-id="9e0b3-129">Für die interne Verwendung.</span><span class="sxs-lookup"><span data-stu-id="9e0b3-129">For internal use.</span></span> |
|<span data-ttu-id="9e0b3-130">type</span><span class="sxs-lookup"><span data-stu-id="9e0b3-130">type</span></span>|<span data-ttu-id="9e0b3-131">String</span><span class="sxs-lookup"><span data-stu-id="9e0b3-131">String</span></span>| <span data-ttu-id="9e0b3-132">Gibt an, von einem Endbenutzer gibt an, ob diese Berechtigung Bereich zugestimmt kann oder gibt an, ob eine gesamte Mandanten Berechtigung ist, die von einem Administrator der Firma zugestimmt werden muss.</span><span class="sxs-lookup"><span data-stu-id="9e0b3-132">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a company administrator.</span></span> <span data-ttu-id="9e0b3-133">Mögliche Werte sind *Benutzer* oder *Administrator*.</span><span class="sxs-lookup"><span data-stu-id="9e0b3-133">Possible values are *User* or *Admin*.</span></span> |
|<span data-ttu-id="9e0b3-134">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="9e0b3-134">userConsentDescription</span></span>|<span data-ttu-id="9e0b3-135">String</span><span class="sxs-lookup"><span data-stu-id="9e0b3-135">String</span></span>| <span data-ttu-id="9e0b3-136">Berechtigung Hilfetext, die in der Genehmigung durch den Endbenutzer angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="9e0b3-136">Permission help text that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="9e0b3-137">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="9e0b3-137">userConsentDisplayName</span></span>|<span data-ttu-id="9e0b3-138">String</span><span class="sxs-lookup"><span data-stu-id="9e0b3-138">String</span></span>| <span data-ttu-id="9e0b3-139">Der Anzeigename für die Berechtigung, die in der Genehmigung durch den Endbenutzer angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="9e0b3-139">Display name for the permission that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="9e0b3-140">Wert</span><span class="sxs-lookup"><span data-stu-id="9e0b3-140">value</span></span>|<span data-ttu-id="9e0b3-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9e0b3-141">String</span></span>| <span data-ttu-id="9e0b3-142">Der Wert des Bereichs geltend, dass die Anwendung für die Ressource in das OAuth 2.0-Zugriffstoken erwarten.</span><span class="sxs-lookup"><span data-stu-id="9e0b3-142">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9e0b3-143">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9e0b3-143">JSON representation</span></span>
<span data-ttu-id="9e0b3-144">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9e0b3-144">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "permissionScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/permissionscope.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
