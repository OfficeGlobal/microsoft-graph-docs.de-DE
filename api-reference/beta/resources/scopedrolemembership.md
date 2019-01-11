---
title: Ressourcentyp scopedRoleMembership
description: Ein Bereich Rollenmitgliedschaften beschreibt eines Benutzers Mitgliedschaft einer Directory-Rolle, die weiter an eine Administrative Einheit (AU) begrenzt ist.  Dies bietet einen Mechanismus, um einen Mandanten gesamte Unternehmen Adminsistrator zum Delegieren der administrativer Berechtigungen zu einem Benutzer das Verwalten von Benutzern und Gruppen in einer Teilmenge der Organisation (der Teilmenge von einer AU definiert wird) zu ermöglichen.
localization_priority: Normal
ms.openlocfilehash: a83acf82eadd9798a86a1a6456d5b2c4ca60be73
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884798"
---
# <a name="scopedrolemembership-resource-type"></a><span data-ttu-id="6f5d4-104">Ressourcentyp scopedRoleMembership</span><span class="sxs-lookup"><span data-stu-id="6f5d4-104">scopedRoleMembership resource type</span></span>

> <span data-ttu-id="6f5d4-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6f5d4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f5d4-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6f5d4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6f5d4-107">Ein Bereich Rollenmitgliedschaften beschreibt eines Benutzers Mitgliedschaft einer Directory-Rolle, die weiter an eine Administrative Einheit (AU) begrenzt ist.</span><span class="sxs-lookup"><span data-stu-id="6f5d4-107">A scoped-role membership describes a user's membership of a directory role, that is further scoped to an Administrative Unit (AU).</span></span>  <span data-ttu-id="6f5d4-108">Dies bietet einen Mechanismus, um einen Mandanten gesamte Unternehmen Adminsistrator zum Delegieren der administrativer Berechtigungen zu einem Benutzer das Verwalten von Benutzern und Gruppen in einer Teilmenge der Organisation (der Teilmenge von einer AU definiert wird) zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="6f5d4-108">This provides a mechanism to allow a tenant-wide company adminsistrator to delegate administrative privileges to a user to manage users and groups in a subset of the organization (the subset being defined by an AU).</span></span>

## <a name="methods"></a><span data-ttu-id="6f5d4-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="6f5d4-109">Methods</span></span>
<span data-ttu-id="6f5d4-110">Direkte Abfragen an diese Ressource werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6f5d4-110">Direct queries to this resource are not supported.</span></span>  <span data-ttu-id="6f5d4-111">Finden Sie im Thema [Administrative Einheiten](administrativeunit.md) zu Informationen zum Abfrage für bezogenen Rollenmitgliedschaften sowie hinzufügen und Entfernen von bezogenen-Rollenmitgliedschaften finden Sie unter.</span><span class="sxs-lookup"><span data-stu-id="6f5d4-111">Please see the [adminstrative units](administrativeunit.md) topic to see information on how to query for scoped-role memberships, as well as adding and removing scoped-role memberships.</span></span> 

## <a name="properties"></a><span data-ttu-id="6f5d4-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6f5d4-112">Properties</span></span>
| <span data-ttu-id="6f5d4-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6f5d4-113">Property</span></span>   | <span data-ttu-id="6f5d4-114">Typ</span><span class="sxs-lookup"><span data-stu-id="6f5d4-114">Type</span></span> | <span data-ttu-id="6f5d4-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6f5d4-115">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="6f5d4-116">administrativeUnitId</span><span class="sxs-lookup"><span data-stu-id="6f5d4-116">administrativeUnitId</span></span>|<span data-ttu-id="6f5d4-117">string</span><span class="sxs-lookup"><span data-stu-id="6f5d4-117">string</span></span>|<span data-ttu-id="6f5d4-118">Eindeutiger Bezeichner für die administrative Einheit, der die Directory-Rolle zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="6f5d4-118">Unique identifier for the administrative unit that the directory role is scoped to</span></span>|
|<span data-ttu-id="6f5d4-119">id</span><span class="sxs-lookup"><span data-stu-id="6f5d4-119">id</span></span>|<span data-ttu-id="6f5d4-120">string</span><span class="sxs-lookup"><span data-stu-id="6f5d4-120">string</span></span>| <span data-ttu-id="6f5d4-121">Eindeutiger Bezeichner für den Gültigkeitsbereich Rollenmitgliedschaften.</span><span class="sxs-lookup"><span data-stu-id="6f5d4-121">Unique identifier for the scoped-role membership.</span></span> <span data-ttu-id="6f5d4-122">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6f5d4-122">Read-only.</span></span>|
|<span data-ttu-id="6f5d4-123">roleId</span><span class="sxs-lookup"><span data-stu-id="6f5d4-123">roleId</span></span>|<span data-ttu-id="6f5d4-124">string</span><span class="sxs-lookup"><span data-stu-id="6f5d4-124">string</span></span>| <span data-ttu-id="6f5d4-125">Eindeutiger Bezeichner für die Directory-Rolle, der in der Member ist.</span><span class="sxs-lookup"><span data-stu-id="6f5d4-125">Unique identifier for the directory role that the member is in.</span></span>|
|<span data-ttu-id="6f5d4-126">roleMemberInfo</span><span class="sxs-lookup"><span data-stu-id="6f5d4-126">roleMemberInfo</span></span>|[<span data-ttu-id="6f5d4-127">identity</span><span class="sxs-lookup"><span data-stu-id="6f5d4-127">identity</span></span>](identity.md)| <span data-ttu-id="6f5d4-128">Rolle Mitglied Identitätsinformationen.</span><span class="sxs-lookup"><span data-stu-id="6f5d4-128">Role member identity information.</span></span> <span data-ttu-id="6f5d4-129">Stellt den Benutzer, der Mitglied dieser bezogenen-Rolle ist.</span><span class="sxs-lookup"><span data-stu-id="6f5d4-129">Represents the user that is a member of this scoped-role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f5d4-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6f5d4-130">Relationships</span></span>
<span data-ttu-id="6f5d4-131">Keine</span><span class="sxs-lookup"><span data-stu-id="6f5d4-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6f5d4-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6f5d4-132">JSON representation</span></span>

<span data-ttu-id="6f5d4-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6f5d4-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scopedrolemembership"
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
<!-- {
  "type": "#page.annotation",
  "description": "scopedRoleMembership resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
