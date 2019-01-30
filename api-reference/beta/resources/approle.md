---
title: AppRole Ressourcentyp
description: Stellt eine Anwendungsrolle, die von einer Clientanwendung aus einer anderen Anwendung aufrufen angefordert werden kann oder, die verwendet werden kann, eine Anwendung Benutzern oder Gruppen in einer angegebenen Anwendungsrolle zugewiesen. Die **AppRoles** -Eigenschaft der Entität ServicePrincipal und der Anwendung Entität ist eine Auflistung von **AppRole**.
localization_priority: Normal
ms.openlocfilehash: 8a367406c64cf9d0d3da49716aeaf6ca3c1fa687
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640413"
---
# <a name="approle-resource-type"></a><span data-ttu-id="6ba8a-104">AppRole Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6ba8a-104">appRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ba8a-105">Stellt eine Anwendungsrolle, die von einer Clientanwendung aus einer anderen Anwendung aufrufen angefordert werden kann oder, die verwendet werden kann, eine Anwendung Benutzern oder Gruppen in einer angegebenen Anwendungsrolle zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="6ba8a-105">Represents an application role that may be requested by a client application calling another application or that may be used to assign an application to users or groups in a specified application role.</span></span> <span data-ttu-id="6ba8a-106">Die **AppRoles** -Eigenschaft der Entität [ServicePrincipal](serviceprincipal.md) und der [Anwendung](application.md) Entität ist eine Auflistung von **AppRole**.</span><span class="sxs-lookup"><span data-stu-id="6ba8a-106">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **appRole**.</span></span>

> <span data-ttu-id="6ba8a-107">Wichtig: Diese Funktion ist in der aktuellen Version deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="6ba8a-107">Important: This functionality is disabled in the current release.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ba8a-108">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6ba8a-108">JSON representation</span></span>

<span data-ttu-id="6ba8a-109">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6ba8a-109">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="6ba8a-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6ba8a-110">Properties</span></span>
| <span data-ttu-id="6ba8a-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6ba8a-111">Property</span></span>     | <span data-ttu-id="6ba8a-112">Typ</span><span class="sxs-lookup"><span data-stu-id="6ba8a-112">Type</span></span>   |<span data-ttu-id="6ba8a-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ba8a-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ba8a-114">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="6ba8a-114">allowedMemberTypes</span></span>|<span data-ttu-id="6ba8a-115">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6ba8a-115">String collection</span></span>|<span data-ttu-id="6ba8a-116">Gibt an, ob diese app Rollendefinition zugewiesen werden kann, Benutzer und Gruppen mit der Einstellung auf "Benutzer" oder in andere Anwendungen (, die diese Anwendung in Filterdaemon Service Szenarien zugreifen) mit der Einstellung auf "Application" oder beide.</span><span class="sxs-lookup"><span data-stu-id="6ba8a-116">Specifies whether this app role definition can be assigned to users and groups by setting to “User”, or to other applications (that are accessing this application in daemon service scenarios) by setting to “Application”, or to both.</span></span>|
|<span data-ttu-id="6ba8a-117">description</span><span class="sxs-lookup"><span data-stu-id="6ba8a-117">description</span></span>|<span data-ttu-id="6ba8a-118">String</span><span class="sxs-lookup"><span data-stu-id="6ba8a-118">String</span></span>|<span data-ttu-id="6ba8a-119">Berechtigung Hilfetext, die in die Zuordnung der Admin-app angezeigt wird und die Erfahrungen stimmen.</span><span class="sxs-lookup"><span data-stu-id="6ba8a-119">Permission help text that appears in the admin app assignment and consent experiences.</span></span>|
|<span data-ttu-id="6ba8a-120">displayName</span><span class="sxs-lookup"><span data-stu-id="6ba8a-120">displayName</span></span>|<span data-ttu-id="6ba8a-121">String</span><span class="sxs-lookup"><span data-stu-id="6ba8a-121">String</span></span>|<span data-ttu-id="6ba8a-122">Der Anzeigename für die Berechtigung, die in der Admin Zustimmung und app-Zuordnung Erfahrungen angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="6ba8a-122">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="6ba8a-123">id</span><span class="sxs-lookup"><span data-stu-id="6ba8a-123">id</span></span>|<span data-ttu-id="6ba8a-124">Guid</span><span class="sxs-lookup"><span data-stu-id="6ba8a-124">Guid</span></span>|<span data-ttu-id="6ba8a-125">Eindeutiger Rollenbezeichner innerhalb der **AppRoles** -Auflistung.</span><span class="sxs-lookup"><span data-stu-id="6ba8a-125">Unique role identifier inside the **appRoles** collection.</span></span>|
|<span data-ttu-id="6ba8a-126">isEnabled</span><span class="sxs-lookup"><span data-stu-id="6ba8a-126">isEnabled</span></span>|<span data-ttu-id="6ba8a-127">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6ba8a-127">Boolean</span></span>|<span data-ttu-id="6ba8a-128">Beim Erstellen oder Aktualisieren einer Rollendefinition, muss dies auf **true** festgelegt werden (die Standardeinstellung ist).</span><span class="sxs-lookup"><span data-stu-id="6ba8a-128">When creating or updating a role definition, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="6ba8a-129">Um eine Rolle zu löschen, muss dieser zunächst auf **false**festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="6ba8a-129">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="6ba8a-130">An dieser Stelle kann diese Rolle im Gespräch nachfolgende entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="6ba8a-130">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="6ba8a-131">Wert</span><span class="sxs-lookup"><span data-stu-id="6ba8a-131">value</span></span>|<span data-ttu-id="6ba8a-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6ba8a-132">String</span></span>|<span data-ttu-id="6ba8a-133">Gibt den Wert des Anspruchs Rollen, die die Anwendung erwarten in die Authentifizierung und Zugriffsteuerung Token an.</span><span class="sxs-lookup"><span data-stu-id="6ba8a-133">Specifies the value of the roles claim that the application should expect in the authentication and access tokens.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/approle.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
