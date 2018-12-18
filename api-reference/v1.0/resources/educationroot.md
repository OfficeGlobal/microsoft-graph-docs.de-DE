---
title: educationRoot-Ressourcentyp
description: 'Der `/education`-Namespace macht spezielle Funktionen für den Ausbildungsbereich verfügbar. '
author: mmast-msft
ms.openlocfilehash: 11aaaec20ccd688b16b74224d1a8c6937e52c5cd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342469"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="06f82-103">educationRoot-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="06f82-103">educationRoot resource type</span></span>

<span data-ttu-id="06f82-104">Der `/education`-Namespace macht spezielle Funktionen für den Ausbildungsbereich verfügbar.</span><span class="sxs-lookup"><span data-stu-id="06f82-104">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="06f82-105">Einige Objekte im `/education`-Namespace finden Sie in anderen Bereichen von Microsoft Graph (z. B. [Benutzer](user.md)).</span><span class="sxs-lookup"><span data-stu-id="06f82-105">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="06f82-106">Der Education-Namespace bietet ausbildungsspezifische Eigenschaften und Features für diese Objekte.</span><span class="sxs-lookup"><span data-stu-id="06f82-106">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="06f82-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="06f82-107">Methods</span></span>

| <span data-ttu-id="06f82-108">Methode</span><span class="sxs-lookup"><span data-stu-id="06f82-108">Method</span></span>           | <span data-ttu-id="06f82-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="06f82-109">Return Type</span></span>    |<span data-ttu-id="06f82-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06f82-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="06f82-111">EducationClass erstellen</span><span class="sxs-lookup"><span data-stu-id="06f82-111">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="06f82-112">educationClass</span><span class="sxs-lookup"><span data-stu-id="06f82-112">educationClass</span></span>](educationclass.md)| <span data-ttu-id="06f82-113">Erstellen eines neuen **educationClass**-Objekts durch Bereitstellen in die Klassensammlung.</span><span class="sxs-lookup"><span data-stu-id="06f82-113">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="06f82-114">Klassen auflisten</span><span class="sxs-lookup"><span data-stu-id="06f82-114">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="06f82-115">[educationClass](educationclass.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="06f82-115">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="06f82-116">Abrufen einer **educationClass**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="06f82-116">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="06f82-117">EducationSchool erstellen</span><span class="sxs-lookup"><span data-stu-id="06f82-117">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="06f82-118">educationSchool</span><span class="sxs-lookup"><span data-stu-id="06f82-118">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="06f82-119">Erstellen eines neuen **educationSchool**-Objekts durch Bereitstellen in der Sammlung der Schulen.</span><span class="sxs-lookup"><span data-stu-id="06f82-119">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="06f82-120">Schulen auflisten</span><span class="sxs-lookup"><span data-stu-id="06f82-120">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="06f82-121">[educationSchool](educationschool.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="06f82-121">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="06f82-122">Abrufen einer **educationSchool**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="06f82-122">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="06f82-123">EducationUser erstellen</span><span class="sxs-lookup"><span data-stu-id="06f82-123">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="06f82-124">educationUser</span><span class="sxs-lookup"><span data-stu-id="06f82-124">educationUser</span></span>](educationuser.md)| <span data-ttu-id="06f82-125">Erstellen eines neuen **educationUser**-Objekts durch Bereitstellen in der Benutzersammlung.</span><span class="sxs-lookup"><span data-stu-id="06f82-125">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="06f82-126">Benutzer auflisten</span><span class="sxs-lookup"><span data-stu-id="06f82-126">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="06f82-127">[educationUser](educationuser.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="06f82-127">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="06f82-128">Abrufen einer **educationUser**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="06f82-128">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="06f82-129">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="06f82-129">Properties</span></span>
<span data-ttu-id="06f82-130">Keine.</span><span class="sxs-lookup"><span data-stu-id="06f82-130">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="06f82-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="06f82-131">Relationships</span></span>
| <span data-ttu-id="06f82-132">Beziehung</span><span class="sxs-lookup"><span data-stu-id="06f82-132">Relationship</span></span> | <span data-ttu-id="06f82-133">Typ</span><span class="sxs-lookup"><span data-stu-id="06f82-133">Type</span></span>   |<span data-ttu-id="06f82-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06f82-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06f82-135">classes</span><span class="sxs-lookup"><span data-stu-id="06f82-135">classes</span></span>|<span data-ttu-id="06f82-136">[educationClass](educationclass.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="06f82-136">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="06f82-p102">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="06f82-p102">Read-only. Nullable.</span></span>|
|<span data-ttu-id="06f82-139">me</span><span class="sxs-lookup"><span data-stu-id="06f82-139">me</span></span>|[<span data-ttu-id="06f82-140">educationUser</span><span class="sxs-lookup"><span data-stu-id="06f82-140">educationUser</span></span>](educationuser.md)| <span data-ttu-id="06f82-p103">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="06f82-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="06f82-143">schools</span><span class="sxs-lookup"><span data-stu-id="06f82-143">schools</span></span>|<span data-ttu-id="06f82-144">[educationSchool](educationschool.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="06f82-144">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="06f82-p104">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="06f82-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="06f82-147">users</span><span class="sxs-lookup"><span data-stu-id="06f82-147">users</span></span>|<span data-ttu-id="06f82-148">[educationUser](educationuser.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="06f82-148">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="06f82-p105">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="06f82-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="06f82-151">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="06f82-151">JSON representation</span></span>
<span data-ttu-id="06f82-152">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="06f82-152">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationRoot"
}-->

```json
{
}
```

<!-- {
  "blockType": "request",
  "name": "get_education"
}-->
```http
GET https://graph.microsoft.com/v1.0/education
```

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRoot"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->