---
title: educationRoot-Ressourcentyp
description: 'Der `/education`-Namespace macht spezielle Funktionen für den Ausbildungsbereich verfügbar. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 91f0162402b8c87042fab622710d314f27d6f4e0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523512"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="6d1e3-103">educationRoot-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6d1e3-103">educationRoot resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d1e3-104">Der `/education`-Namespace macht spezielle Funktionen für den Ausbildungsbereich verfügbar.</span><span class="sxs-lookup"><span data-stu-id="6d1e3-104">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="6d1e3-105">Einige Objekte im `/education`-Namespace finden Sie in anderen Bereichen von Microsoft Graph (z. B. [Benutzer](user.md)).</span><span class="sxs-lookup"><span data-stu-id="6d1e3-105">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="6d1e3-106">Der Education-Namespace bietet ausbildungsspezifische Eigenschaften und Features für diese Objekte.</span><span class="sxs-lookup"><span data-stu-id="6d1e3-106">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="6d1e3-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="6d1e3-107">Methods</span></span>

| <span data-ttu-id="6d1e3-108">Methode</span><span class="sxs-lookup"><span data-stu-id="6d1e3-108">Method</span></span>           | <span data-ttu-id="6d1e3-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="6d1e3-109">Return Type</span></span>    |<span data-ttu-id="6d1e3-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6d1e3-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6d1e3-111">EducationClass erstellen</span><span class="sxs-lookup"><span data-stu-id="6d1e3-111">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="6d1e3-112">educationClass</span><span class="sxs-lookup"><span data-stu-id="6d1e3-112">educationClass</span></span>](educationclass.md)| <span data-ttu-id="6d1e3-113">Erstellen eines neuen **educationClass**-Objekts durch Bereitstellen in die Klassensammlung.</span><span class="sxs-lookup"><span data-stu-id="6d1e3-113">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="6d1e3-114">Klassen auflisten</span><span class="sxs-lookup"><span data-stu-id="6d1e3-114">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="6d1e3-115">[educationClass](educationclass.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6d1e3-115">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="6d1e3-116">Abrufen einer **educationClass**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="6d1e3-116">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="6d1e3-117">EducationSchool erstellen</span><span class="sxs-lookup"><span data-stu-id="6d1e3-117">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="6d1e3-118">educationSchool</span><span class="sxs-lookup"><span data-stu-id="6d1e3-118">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="6d1e3-119">Erstellen eines neuen **educationSchool**-Objekts durch Bereitstellen in der Sammlung der Schulen.</span><span class="sxs-lookup"><span data-stu-id="6d1e3-119">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="6d1e3-120">Schulen auflisten</span><span class="sxs-lookup"><span data-stu-id="6d1e3-120">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="6d1e3-121">[educationSchool](educationschool.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6d1e3-121">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="6d1e3-122">Abrufen einer **educationSchool**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="6d1e3-122">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="6d1e3-123">EducationUser erstellen</span><span class="sxs-lookup"><span data-stu-id="6d1e3-123">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="6d1e3-124">educationUser</span><span class="sxs-lookup"><span data-stu-id="6d1e3-124">educationUser</span></span>](educationuser.md)| <span data-ttu-id="6d1e3-125">Erstellen eines neuen **educationUser**-Objekts durch Bereitstellen in der Benutzersammlung.</span><span class="sxs-lookup"><span data-stu-id="6d1e3-125">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="6d1e3-126">Benutzer auflisten</span><span class="sxs-lookup"><span data-stu-id="6d1e3-126">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="6d1e3-127">[educationUser](educationuser.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6d1e3-127">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="6d1e3-128">Abrufen einer **educationUser**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="6d1e3-128">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="6d1e3-129">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6d1e3-129">Properties</span></span>
<span data-ttu-id="6d1e3-130">Keine.</span><span class="sxs-lookup"><span data-stu-id="6d1e3-130">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="6d1e3-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6d1e3-131">Relationships</span></span>
| <span data-ttu-id="6d1e3-132">Beziehung</span><span class="sxs-lookup"><span data-stu-id="6d1e3-132">Relationship</span></span> | <span data-ttu-id="6d1e3-133">Typ</span><span class="sxs-lookup"><span data-stu-id="6d1e3-133">Type</span></span>   |<span data-ttu-id="6d1e3-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6d1e3-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d1e3-135">classes</span><span class="sxs-lookup"><span data-stu-id="6d1e3-135">classes</span></span>|<span data-ttu-id="6d1e3-136">[educationClass](educationclass.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6d1e3-136">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="6d1e3-p102">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="6d1e3-p102">Read-only. Nullable.</span></span>|
|<span data-ttu-id="6d1e3-139">me</span><span class="sxs-lookup"><span data-stu-id="6d1e3-139">me</span></span>|[<span data-ttu-id="6d1e3-140">educationUser</span><span class="sxs-lookup"><span data-stu-id="6d1e3-140">educationUser</span></span>](educationuser.md)| <span data-ttu-id="6d1e3-p103">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="6d1e3-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="6d1e3-143">schools</span><span class="sxs-lookup"><span data-stu-id="6d1e3-143">schools</span></span>|<span data-ttu-id="6d1e3-144">[educationSchool](educationschool.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6d1e3-144">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="6d1e3-p104">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="6d1e3-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="6d1e3-147">users</span><span class="sxs-lookup"><span data-stu-id="6d1e3-147">users</span></span>|<span data-ttu-id="6d1e3-148">[educationUser](educationuser.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6d1e3-148">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="6d1e3-p105">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="6d1e3-p105">Read-only. Nullable.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationroot.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
