---
title: Ressourcentyp governanceSubject
description: Stellt Benutzern, Gruppen und Service-Prinzipale in privilegierten Identity Management (PIM) verwaltet werden.
localization_priority: Normal
ms.openlocfilehash: a83825a147429c81b3e83b2f2fb384672d2f527e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519164"
---
# <a name="governancesubject-resource-type"></a><span data-ttu-id="173e8-103">Ressourcentyp governanceSubject</span><span class="sxs-lookup"><span data-stu-id="173e8-103">governanceSubject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="173e8-104">Stellt Benutzern, Gruppen und Service-Prinzipale in privilegierten Identity Management (PIM) verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="173e8-104">Represents users, groups, and service principals being managed in Privileged Identity Management (PIM).</span></span>


## <a name="properties"></a><span data-ttu-id="173e8-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="173e8-105">Properties</span></span>
| <span data-ttu-id="173e8-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="173e8-106">Property</span></span>  | <span data-ttu-id="173e8-107">Typ</span><span class="sxs-lookup"><span data-stu-id="173e8-107">Type</span></span>       |<span data-ttu-id="173e8-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="173e8-108">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="173e8-109">id</span><span class="sxs-lookup"><span data-stu-id="173e8-109">id</span></span>         |<span data-ttu-id="173e8-110">string</span><span class="sxs-lookup"><span data-stu-id="173e8-110">String</span></span>     | <span data-ttu-id="173e8-111">Die Id des Betreffs.</span><span class="sxs-lookup"><span data-stu-id="173e8-111">The id of the subject.</span></span>|
|<span data-ttu-id="173e8-112">type</span><span class="sxs-lookup"><span data-stu-id="173e8-112">type</span></span>       |<span data-ttu-id="173e8-113">String</span><span class="sxs-lookup"><span data-stu-id="173e8-113">String</span></span>     |<span data-ttu-id="173e8-114">Der Typ des Betreffs.</span><span class="sxs-lookup"><span data-stu-id="173e8-114">The type of the subject.</span></span> <span data-ttu-id="173e8-115">Der Wert kann sein ``User``, ``Group``, und ``ServicePrincipal``.</span><span class="sxs-lookup"><span data-stu-id="173e8-115">The value can be ``User``, ``Group``, and ``ServicePrincipal``.</span></span>|
|<span data-ttu-id="173e8-116">displayName</span><span class="sxs-lookup"><span data-stu-id="173e8-116">displayName</span></span>|<span data-ttu-id="173e8-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="173e8-117">String</span></span>     |<span data-ttu-id="173e8-118">Der Anzeigename des Betreffs.</span><span class="sxs-lookup"><span data-stu-id="173e8-118">The display name of the subject.</span></span>|
|<span data-ttu-id="173e8-119">E-Mail</span><span class="sxs-lookup"><span data-stu-id="173e8-119">email</span></span>      |<span data-ttu-id="173e8-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="173e8-120">String</span></span>     |<span data-ttu-id="173e8-121">Die e-Mail-Adresse des Betreffs Benutzer.</span><span class="sxs-lookup"><span data-stu-id="173e8-121">The email address of the user subject.</span></span> <span data-ttu-id="173e8-122">Wenn der Betreff in anderen Typen ist, ist leer.</span><span class="sxs-lookup"><span data-stu-id="173e8-122">If the subject is in other types, it is empty.</span></span>|
|<span data-ttu-id="173e8-123">principalName</span><span class="sxs-lookup"><span data-stu-id="173e8-123">principalName</span></span>|<span data-ttu-id="173e8-124">String</span><span class="sxs-lookup"><span data-stu-id="173e8-124">String</span></span>   |<span data-ttu-id="173e8-125">Den Prinzipalnamen des Benutzers Betreff.</span><span class="sxs-lookup"><span data-stu-id="173e8-125">The principal name of the user subject.</span></span> <span data-ttu-id="173e8-126">Wenn der Betreff in anderen Typen ist, ist leer.</span><span class="sxs-lookup"><span data-stu-id="173e8-126">If the subject is in other types, it is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="173e8-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="173e8-127">Relationships</span></span>
<span data-ttu-id="173e8-128">Keine</span><span class="sxs-lookup"><span data-stu-id="173e8-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="173e8-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="173e8-129">JSON representation</span></span>

<span data-ttu-id="173e8-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="173e8-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceSubject"
}-->

```json
{
  "id": "String",  
  "displayName": "String",
  "email": "String",
  "principalName": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceSubject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governancesubject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
