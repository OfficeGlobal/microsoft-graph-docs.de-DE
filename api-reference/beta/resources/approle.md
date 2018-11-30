---
title: AppRole Ressourcentyp
description: Stellt eine Anwendungsrolle, die von einer Clientanwendung aus einer anderen Anwendung aufrufen angefordert werden kann oder, die verwendet werden kann, eine Anwendung Benutzern oder Gruppen in einer angegebenen Anwendungsrolle zugewiesen. Die **AppRoles** -Eigenschaft der Entität ServicePrincipal und der Anwendung Entität ist eine Auflistung von **AppRole**.
ms.openlocfilehash: f87ef6f40fbeb18ec4b3a2373fb2a19e14da84a4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059589"
---
# <a name="approle-resource-type"></a><span data-ttu-id="3f821-104">AppRole Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3f821-104">appRole resource type</span></span>

> <span data-ttu-id="3f821-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3f821-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3f821-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3f821-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3f821-107">Stellt eine Anwendungsrolle, die von einer Clientanwendung aus einer anderen Anwendung aufrufen angefordert werden kann oder, die verwendet werden kann, eine Anwendung Benutzern oder Gruppen in einer angegebenen Anwendungsrolle zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="3f821-107">Represents an application role that may be requested by a client application calling another application or that may be used to assign an application to users or groups in a specified application role.</span></span> <span data-ttu-id="3f821-108">Die **AppRoles** -Eigenschaft der Entität [ServicePrincipal](serviceprincipal.md) und der [Anwendung](application.md) Entität ist eine Auflistung von **AppRole**.</span><span class="sxs-lookup"><span data-stu-id="3f821-108">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **appRole**.</span></span>

> <span data-ttu-id="3f821-109">Wichtig: Diese Funktion ist in der aktuellen Version deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="3f821-109">Important: This functionality is disabled in the current release.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f821-110">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3f821-110">JSON representation</span></span>

<span data-ttu-id="3f821-111">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3f821-111">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approle"
}-->

```json
{
  "allowedMemberTypes": ["string"],
  "description": "string",
  "displayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "value": "string"
}

```
## <a name="properties"></a><span data-ttu-id="3f821-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3f821-112">Properties</span></span>
| <span data-ttu-id="3f821-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3f821-113">Property</span></span>     | <span data-ttu-id="3f821-114">Typ</span><span class="sxs-lookup"><span data-stu-id="3f821-114">Type</span></span>   |<span data-ttu-id="3f821-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3f821-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f821-116">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="3f821-116">allowedMemberTypes</span></span>|<span data-ttu-id="3f821-117">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="3f821-117">String collection</span></span>|<span data-ttu-id="3f821-118">Gibt an, ob diese app Rollendefinition zugewiesen werden kann, Benutzer und Gruppen mit der Einstellung auf "Benutzer" oder in andere Anwendungen (, die diese Anwendung in Filterdaemon Service Szenarien zugreifen) mit der Einstellung auf "Application" oder beide.</span><span class="sxs-lookup"><span data-stu-id="3f821-118">Specifies whether this app role definition can be assigned to users and groups by setting to “User”, or to other applications (that are accessing this application in daemon service scenarios) by setting to “Application”, or to both.</span></span>|
|<span data-ttu-id="3f821-119">description</span><span class="sxs-lookup"><span data-stu-id="3f821-119">description</span></span>|<span data-ttu-id="3f821-120">String</span><span class="sxs-lookup"><span data-stu-id="3f821-120">String</span></span>|<span data-ttu-id="3f821-121">Berechtigung Hilfetext, die in die Zuordnung der Admin-app angezeigt wird und die Erfahrungen stimmen.</span><span class="sxs-lookup"><span data-stu-id="3f821-121">Permission help text that appears in the admin app assignment and consent experiences.</span></span>|
|<span data-ttu-id="3f821-122">displayName</span><span class="sxs-lookup"><span data-stu-id="3f821-122">displayName</span></span>|<span data-ttu-id="3f821-123">String</span><span class="sxs-lookup"><span data-stu-id="3f821-123">String</span></span>|<span data-ttu-id="3f821-124">Der Anzeigename für die Berechtigung, die in der Admin Zustimmung und app-Zuordnung Erfahrungen angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="3f821-124">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="3f821-125">id</span><span class="sxs-lookup"><span data-stu-id="3f821-125">id</span></span>|<span data-ttu-id="3f821-126">Guid</span><span class="sxs-lookup"><span data-stu-id="3f821-126">Guid</span></span>|<span data-ttu-id="3f821-127">Eindeutiger Rollenbezeichner innerhalb der **AppRoles** -Auflistung.</span><span class="sxs-lookup"><span data-stu-id="3f821-127">Unique role identifier inside the **appRoles** collection.</span></span>|
|<span data-ttu-id="3f821-128">isEnabled</span><span class="sxs-lookup"><span data-stu-id="3f821-128">isEnabled</span></span>|<span data-ttu-id="3f821-129">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3f821-129">Boolean</span></span>|<span data-ttu-id="3f821-130">Beim Erstellen oder Aktualisieren einer Rollendefinition, muss dies auf **true** festgelegt werden (die Standardeinstellung ist).</span><span class="sxs-lookup"><span data-stu-id="3f821-130">When creating or updating a role definition, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="3f821-131">Um eine Rolle zu löschen, muss dieser zunächst auf **false**festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="3f821-131">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="3f821-132">An dieser Stelle kann diese Rolle im Gespräch nachfolgende entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="3f821-132">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="3f821-133">Wert</span><span class="sxs-lookup"><span data-stu-id="3f821-133">value</span></span>|<span data-ttu-id="3f821-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3f821-134">String</span></span>|<span data-ttu-id="3f821-135">Gibt den Wert des Anspruchs Rollen, die die Anwendung erwarten in die Authentifizierung und Zugriffsteuerung Token an.</span><span class="sxs-lookup"><span data-stu-id="3f821-135">Specifies the value of the roles claim that the application should expect in the authentication and access tokens.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->