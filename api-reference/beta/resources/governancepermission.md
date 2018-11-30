---
title: Ressourcentyp governancePermission
description: 'Stellt die Berechtigung, die ein GovernanceSubject hat für eine bestimmte GovernanceResource dar.  '
ms.openlocfilehash: d7b3e1eb70c89c278ccc2a8b3e9a16e265e4ae97
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062738"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="ac24e-103">Ressourcentyp governancePermission</span><span class="sxs-lookup"><span data-stu-id="ac24e-103">governancePermission resource type</span></span>

> <span data-ttu-id="ac24e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ac24e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ac24e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ac24e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ac24e-106">Stellt die Berechtigung, die ein [GovernanceSubject](../resources/governancesubject.md) hat für eine bestimmte [GovernanceResource](../resources/governanceresource.md)dar.</span><span class="sxs-lookup"><span data-stu-id="ac24e-106">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>  


## <a name="properties"></a><span data-ttu-id="ac24e-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ac24e-107">Properties</span></span>
| <span data-ttu-id="ac24e-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ac24e-108">Property</span></span>     | <span data-ttu-id="ac24e-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ac24e-109">Type</span></span>   |<span data-ttu-id="ac24e-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ac24e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac24e-111">accessLevel</span><span class="sxs-lookup"><span data-stu-id="ac24e-111">accessLevel</span></span>|<span data-ttu-id="ac24e-112">String</span><span class="sxs-lookup"><span data-stu-id="ac24e-112">String</span></span>|<span data-ttu-id="ac24e-113">Die Zugriffsebene.</span><span class="sxs-lookup"><span data-stu-id="ac24e-113">The access level.</span></span> <span data-ttu-id="ac24e-114">Gültige Werte: ``None``, ``UserRead``, ``AdminRead``, und ``AdminReadWrite``.</span><span class="sxs-lookup"><span data-stu-id="ac24e-114">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="ac24e-115">isActive</span><span class="sxs-lookup"><span data-stu-id="ac24e-115">isActive</span></span>|<span data-ttu-id="ac24e-116">Boolesch</span><span class="sxs-lookup"><span data-stu-id="ac24e-116">Boolean</span></span>|<span data-ttu-id="ac24e-117">Gibt an, ob der anfordernden Person hat aktiven rollenzuweisung für die Zugriffsebene.</span><span class="sxs-lookup"><span data-stu-id="ac24e-117">Indicate if the the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="ac24e-118">isEligible</span><span class="sxs-lookup"><span data-stu-id="ac24e-118">isEligible</span></span>|<span data-ttu-id="ac24e-119">Boolesch</span><span class="sxs-lookup"><span data-stu-id="ac24e-119">Boolean</span></span>|<span data-ttu-id="ac24e-120">Geben Sie an, ob der Requestor alle qualifizierten rollenzuweisung für die Zugriffsebene hat.</span><span class="sxs-lookup"><span data-stu-id="ac24e-120">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ac24e-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ac24e-121">JSON representation</span></span>

<span data-ttu-id="ac24e-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ac24e-122">Here is a JSON representation of the resource.</span></span>

```json
{
  "accessLevel": "String",
  "isActive": true,
  "isEligible": true
}

```