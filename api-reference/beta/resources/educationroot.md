---
title: educationRoot-Ressourcentyp
description: 'Der `/education`-Namespace macht spezielle Funktionen für den Ausbildungsbereich verfügbar. '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: c268c7b910bd9f6f14763f3a7b5445af0ac12826
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890657"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="34dfc-103">educationRoot-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="34dfc-103">educationRoot resource type</span></span>

> <span data-ttu-id="34dfc-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="34dfc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34dfc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34dfc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="34dfc-106">Der `/education`-Namespace macht spezielle Funktionen für den Ausbildungsbereich verfügbar.</span><span class="sxs-lookup"><span data-stu-id="34dfc-106">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="34dfc-107">Einige Objekte im `/education`-Namespace finden Sie in anderen Bereichen von Microsoft Graph (z. B. [Benutzer](user.md)).</span><span class="sxs-lookup"><span data-stu-id="34dfc-107">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="34dfc-108">Der Education-Namespace bietet ausbildungsspezifische Eigenschaften und Features für diese Objekte.</span><span class="sxs-lookup"><span data-stu-id="34dfc-108">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="34dfc-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="34dfc-109">Methods</span></span>

| <span data-ttu-id="34dfc-110">Methode</span><span class="sxs-lookup"><span data-stu-id="34dfc-110">Method</span></span>           | <span data-ttu-id="34dfc-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="34dfc-111">Return Type</span></span>    |<span data-ttu-id="34dfc-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="34dfc-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="34dfc-113">EducationClass erstellen</span><span class="sxs-lookup"><span data-stu-id="34dfc-113">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="34dfc-114">educationClass</span><span class="sxs-lookup"><span data-stu-id="34dfc-114">educationClass</span></span>](educationclass.md)| <span data-ttu-id="34dfc-115">Erstellen eines neuen **educationClass**-Objekts durch Bereitstellen in die Klassensammlung.</span><span class="sxs-lookup"><span data-stu-id="34dfc-115">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="34dfc-116">Klassen auflisten</span><span class="sxs-lookup"><span data-stu-id="34dfc-116">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="34dfc-117">[educationClass](educationclass.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="34dfc-117">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="34dfc-118">Abrufen einer **educationClass**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="34dfc-118">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="34dfc-119">EducationSchool erstellen</span><span class="sxs-lookup"><span data-stu-id="34dfc-119">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="34dfc-120">educationSchool</span><span class="sxs-lookup"><span data-stu-id="34dfc-120">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="34dfc-121">Erstellen eines neuen **educationSchool**-Objekts durch Bereitstellen in der Sammlung der Schulen.</span><span class="sxs-lookup"><span data-stu-id="34dfc-121">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="34dfc-122">Schulen auflisten</span><span class="sxs-lookup"><span data-stu-id="34dfc-122">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="34dfc-123">[educationSchool](educationschool.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="34dfc-123">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="34dfc-124">Abrufen einer **educationSchool**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="34dfc-124">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="34dfc-125">EducationUser erstellen</span><span class="sxs-lookup"><span data-stu-id="34dfc-125">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="34dfc-126">educationUser</span><span class="sxs-lookup"><span data-stu-id="34dfc-126">educationUser</span></span>](educationuser.md)| <span data-ttu-id="34dfc-127">Erstellen eines neuen **educationUser**-Objekts durch Bereitstellen in der Benutzersammlung.</span><span class="sxs-lookup"><span data-stu-id="34dfc-127">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="34dfc-128">Benutzer auflisten</span><span class="sxs-lookup"><span data-stu-id="34dfc-128">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="34dfc-129">[educationUser](educationuser.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="34dfc-129">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="34dfc-130">Abrufen einer **educationUser**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="34dfc-130">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="34dfc-131">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="34dfc-131">Properties</span></span>
<span data-ttu-id="34dfc-132">Keine.</span><span class="sxs-lookup"><span data-stu-id="34dfc-132">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="34dfc-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="34dfc-133">Relationships</span></span>
| <span data-ttu-id="34dfc-134">Beziehung</span><span class="sxs-lookup"><span data-stu-id="34dfc-134">Relationship</span></span> | <span data-ttu-id="34dfc-135">Typ</span><span class="sxs-lookup"><span data-stu-id="34dfc-135">Type</span></span>   |<span data-ttu-id="34dfc-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="34dfc-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34dfc-137">classes</span><span class="sxs-lookup"><span data-stu-id="34dfc-137">classes</span></span>|<span data-ttu-id="34dfc-138">[educationClass](educationclass.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="34dfc-138">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="34dfc-p103">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="34dfc-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="34dfc-141">me</span><span class="sxs-lookup"><span data-stu-id="34dfc-141">me</span></span>|[<span data-ttu-id="34dfc-142">educationUser</span><span class="sxs-lookup"><span data-stu-id="34dfc-142">educationUser</span></span>](educationuser.md)| <span data-ttu-id="34dfc-p104">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="34dfc-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="34dfc-145">schools</span><span class="sxs-lookup"><span data-stu-id="34dfc-145">schools</span></span>|<span data-ttu-id="34dfc-146">[educationSchool](educationschool.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="34dfc-146">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="34dfc-p105">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="34dfc-p105">Read-only. Nullable.</span></span>|
|<span data-ttu-id="34dfc-149">users</span><span class="sxs-lookup"><span data-stu-id="34dfc-149">users</span></span>|<span data-ttu-id="34dfc-150">[educationUser](educationuser.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="34dfc-150">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="34dfc-p106">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="34dfc-p106">Read-only. Nullable.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
