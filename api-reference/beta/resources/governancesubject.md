---
title: Ressourcentyp governanceSubject
description: Stellt Benutzern, Gruppen und Service-Prinzipale in privilegierten Identity Management (PIM) verwaltet werden.
localization_priority: Normal
ms.openlocfilehash: f3f8762c9136a3ae92269f6c06f52000fb73f710
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832592"
---
# <a name="governancesubject-resource-type"></a><span data-ttu-id="7ca72-103">Ressourcentyp governanceSubject</span><span class="sxs-lookup"><span data-stu-id="7ca72-103">governanceSubject resource type</span></span>

> <span data-ttu-id="7ca72-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7ca72-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ca72-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7ca72-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7ca72-106">Stellt Benutzern, Gruppen und Service-Prinzipale in privilegierten Identity Management (PIM) verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="7ca72-106">Represents users, groups, and service principals being managed in Privileged Identity Management (PIM).</span></span>


## <a name="properties"></a><span data-ttu-id="7ca72-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7ca72-107">Properties</span></span>
| <span data-ttu-id="7ca72-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7ca72-108">Property</span></span>  | <span data-ttu-id="7ca72-109">Typ</span><span class="sxs-lookup"><span data-stu-id="7ca72-109">Type</span></span>       |<span data-ttu-id="7ca72-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7ca72-110">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="7ca72-111">id</span><span class="sxs-lookup"><span data-stu-id="7ca72-111">id</span></span>         |<span data-ttu-id="7ca72-112">String</span><span class="sxs-lookup"><span data-stu-id="7ca72-112">String</span></span>     | <span data-ttu-id="7ca72-113">Die Id des Betreffs.</span><span class="sxs-lookup"><span data-stu-id="7ca72-113">The id of the subject.</span></span>|
|<span data-ttu-id="7ca72-114">type</span><span class="sxs-lookup"><span data-stu-id="7ca72-114">type</span></span>       |<span data-ttu-id="7ca72-115">String</span><span class="sxs-lookup"><span data-stu-id="7ca72-115">String</span></span>     |<span data-ttu-id="7ca72-116">Der Typ des Betreffs.</span><span class="sxs-lookup"><span data-stu-id="7ca72-116">The type of the subject.</span></span> <span data-ttu-id="7ca72-117">Der Wert kann sein ``User``, ``Group``, und ``ServicePrincipal``.</span><span class="sxs-lookup"><span data-stu-id="7ca72-117">The value can be ``User``, ``Group``, and ``ServicePrincipal``.</span></span>|
|<span data-ttu-id="7ca72-118">displayName</span><span class="sxs-lookup"><span data-stu-id="7ca72-118">displayName</span></span>|<span data-ttu-id="7ca72-119">String</span><span class="sxs-lookup"><span data-stu-id="7ca72-119">String</span></span>     |<span data-ttu-id="7ca72-120">Der Anzeigename des Betreffs.</span><span class="sxs-lookup"><span data-stu-id="7ca72-120">The display name of the subject.</span></span>|
|<span data-ttu-id="7ca72-121">E-Mail</span><span class="sxs-lookup"><span data-stu-id="7ca72-121">email</span></span>      |<span data-ttu-id="7ca72-122">String</span><span class="sxs-lookup"><span data-stu-id="7ca72-122">String</span></span>     |<span data-ttu-id="7ca72-123">Die e-Mail-Adresse des Betreffs Benutzer.</span><span class="sxs-lookup"><span data-stu-id="7ca72-123">The email address of the user subject.</span></span> <span data-ttu-id="7ca72-124">Wenn der Betreff in anderen Typen ist, ist leer.</span><span class="sxs-lookup"><span data-stu-id="7ca72-124">If the subject is in other types, it is empty.</span></span>|
|<span data-ttu-id="7ca72-125">principalName</span><span class="sxs-lookup"><span data-stu-id="7ca72-125">principalName</span></span>|<span data-ttu-id="7ca72-126">String</span><span class="sxs-lookup"><span data-stu-id="7ca72-126">String</span></span>   |<span data-ttu-id="7ca72-127">Den Prinzipalnamen des Benutzers Betreff.</span><span class="sxs-lookup"><span data-stu-id="7ca72-127">The principal name of the user subject.</span></span> <span data-ttu-id="7ca72-128">Wenn der Betreff in anderen Typen ist, ist leer.</span><span class="sxs-lookup"><span data-stu-id="7ca72-128">If the subject is in other types, it is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ca72-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7ca72-129">Relationships</span></span>
<span data-ttu-id="7ca72-130">Keine</span><span class="sxs-lookup"><span data-stu-id="7ca72-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="7ca72-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7ca72-131">JSON representation</span></span>

<span data-ttu-id="7ca72-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7ca72-132">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "governanceSubject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
