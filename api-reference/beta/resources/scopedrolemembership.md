---
title: Ressourcentyp scopedRoleMembership
description: Ein Bereich Rollenmitgliedschaften beschreibt eines Benutzers Mitgliedschaft einer Directory-Rolle, die weiter an eine Administrative Einheit (AU) begrenzt ist.  Dies bietet einen Mechanismus, um einen Mandanten gesamte Unternehmen Adminsistrator zum Delegieren der administrativer Berechtigungen zu einem Benutzer das Verwalten von Benutzern und Gruppen in einer Teilmenge der Organisation (der Teilmenge von einer AU definiert wird) zu ermöglichen.
localization_priority: Normal
ms.openlocfilehash: c3af7a44221c4cf2822440a6025706c8bd4a93ac
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575660"
---
# <a name="scopedrolemembership-resource-type"></a><span data-ttu-id="cfd9c-104">Ressourcentyp scopedRoleMembership</span><span class="sxs-lookup"><span data-stu-id="cfd9c-104">scopedRoleMembership resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfd9c-105">Ein Bereich Rollenmitgliedschaften beschreibt eines Benutzers Mitgliedschaft einer Directory-Rolle, die weiter an eine Administrative Einheit (AU) begrenzt ist.</span><span class="sxs-lookup"><span data-stu-id="cfd9c-105">A scoped-role membership describes a user's membership of a directory role, that is further scoped to an Administrative Unit (AU).</span></span>  <span data-ttu-id="cfd9c-106">Dies bietet einen Mechanismus, um einen Mandanten gesamte Unternehmen Adminsistrator zum Delegieren der administrativer Berechtigungen zu einem Benutzer das Verwalten von Benutzern und Gruppen in einer Teilmenge der Organisation (der Teilmenge von einer AU definiert wird) zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="cfd9c-106">This provides a mechanism to allow a tenant-wide company adminsistrator to delegate administrative privileges to a user to manage users and groups in a subset of the organization (the subset being defined by an AU).</span></span>

## <a name="methods"></a><span data-ttu-id="cfd9c-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="cfd9c-107">Methods</span></span>
<span data-ttu-id="cfd9c-108">Direkte Abfragen an diese Ressource werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cfd9c-108">Direct queries to this resource are not supported.</span></span>  <span data-ttu-id="cfd9c-109">Finden Sie im Thema [Administrative Einheiten](administrativeunit.md) zu Informationen zum Abfrage für bezogenen Rollenmitgliedschaften sowie hinzufügen und Entfernen von bezogenen-Rollenmitgliedschaften finden Sie unter.</span><span class="sxs-lookup"><span data-stu-id="cfd9c-109">Please see the [adminstrative units](administrativeunit.md) topic to see information on how to query for scoped-role memberships, as well as adding and removing scoped-role memberships.</span></span> 

## <a name="properties"></a><span data-ttu-id="cfd9c-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cfd9c-110">Properties</span></span>
| <span data-ttu-id="cfd9c-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cfd9c-111">Property</span></span>   | <span data-ttu-id="cfd9c-112">Typ</span><span class="sxs-lookup"><span data-stu-id="cfd9c-112">Type</span></span> | <span data-ttu-id="cfd9c-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cfd9c-113">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="cfd9c-114">administrativeUnitId</span><span class="sxs-lookup"><span data-stu-id="cfd9c-114">administrativeUnitId</span></span>|<span data-ttu-id="cfd9c-115">string</span><span class="sxs-lookup"><span data-stu-id="cfd9c-115">string</span></span>|<span data-ttu-id="cfd9c-116">Eindeutiger Bezeichner für die administrative Einheit, der die Directory-Rolle zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="cfd9c-116">Unique identifier for the administrative unit that the directory role is scoped to</span></span>|
|<span data-ttu-id="cfd9c-117">id</span><span class="sxs-lookup"><span data-stu-id="cfd9c-117">id</span></span>|<span data-ttu-id="cfd9c-118">string</span><span class="sxs-lookup"><span data-stu-id="cfd9c-118">string</span></span>| <span data-ttu-id="cfd9c-119">Eindeutiger Bezeichner für den Gültigkeitsbereich Rollenmitgliedschaften.</span><span class="sxs-lookup"><span data-stu-id="cfd9c-119">Unique identifier for the scoped-role membership.</span></span> <span data-ttu-id="cfd9c-120">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="cfd9c-120">Read-only.</span></span>|
|<span data-ttu-id="cfd9c-121">roleId</span><span class="sxs-lookup"><span data-stu-id="cfd9c-121">roleId</span></span>|<span data-ttu-id="cfd9c-122">string</span><span class="sxs-lookup"><span data-stu-id="cfd9c-122">string</span></span>| <span data-ttu-id="cfd9c-123">Eindeutiger Bezeichner für die Directory-Rolle, der in der Member ist.</span><span class="sxs-lookup"><span data-stu-id="cfd9c-123">Unique identifier for the directory role that the member is in.</span></span>|
|<span data-ttu-id="cfd9c-124">roleMemberInfo</span><span class="sxs-lookup"><span data-stu-id="cfd9c-124">roleMemberInfo</span></span>|[<span data-ttu-id="cfd9c-125">identity</span><span class="sxs-lookup"><span data-stu-id="cfd9c-125">identity</span></span>](identity.md)| <span data-ttu-id="cfd9c-126">Rolle Mitglied Identitätsinformationen.</span><span class="sxs-lookup"><span data-stu-id="cfd9c-126">Role member identity information.</span></span> <span data-ttu-id="cfd9c-127">Stellt den Benutzer, der Mitglied dieser bezogenen-Rolle ist.</span><span class="sxs-lookup"><span data-stu-id="cfd9c-127">Represents the user that is a member of this scoped-role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cfd9c-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="cfd9c-128">Relationships</span></span>
<span data-ttu-id="cfd9c-129">Keine</span><span class="sxs-lookup"><span data-stu-id="cfd9c-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="cfd9c-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cfd9c-130">JSON representation</span></span>

<span data-ttu-id="cfd9c-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cfd9c-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scopedRoleMembership"
}-->

```json
{
  "administrativeUnitId": "string",
  "id": "string (identifier)",
  "roleId": "string",
  "roleMemberInfo": {"@odata.type": "microsoft.graph.identity"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scopedRoleMembership resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/scopedrolemembership.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
