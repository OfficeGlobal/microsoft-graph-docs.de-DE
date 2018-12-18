---
title: educationRoot-Ressourcentyp
description: 'Der `/education`-Namespace macht spezielle Funktionen für den Ausbildungsbereich verfügbar. '
author: mmast-msft
ms.openlocfilehash: 2a9eac02552e62e7bfb889e9e87efe47fa5f88f9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307434"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="aeece-103">educationRoot-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="aeece-103">educationRoot resource type</span></span>

> <span data-ttu-id="aeece-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="aeece-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aeece-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aeece-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aeece-106">Der `/education`-Namespace macht spezielle Funktionen für den Ausbildungsbereich verfügbar.</span><span class="sxs-lookup"><span data-stu-id="aeece-106">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="aeece-107">Einige Objekte im `/education`-Namespace finden Sie in anderen Bereichen von Microsoft Graph (z. B. [Benutzer](user.md)).</span><span class="sxs-lookup"><span data-stu-id="aeece-107">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="aeece-108">Der Education-Namespace bietet ausbildungsspezifische Eigenschaften und Features für diese Objekte.</span><span class="sxs-lookup"><span data-stu-id="aeece-108">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="aeece-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="aeece-109">Methods</span></span>

| <span data-ttu-id="aeece-110">Methode</span><span class="sxs-lookup"><span data-stu-id="aeece-110">Method</span></span>           | <span data-ttu-id="aeece-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="aeece-111">Return Type</span></span>    |<span data-ttu-id="aeece-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aeece-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aeece-113">EducationClass erstellen</span><span class="sxs-lookup"><span data-stu-id="aeece-113">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="aeece-114">educationClass</span><span class="sxs-lookup"><span data-stu-id="aeece-114">educationClass</span></span>](educationclass.md)| <span data-ttu-id="aeece-115">Erstellen eines neuen **educationClass**-Objekts durch Bereitstellen in die Klassensammlung.</span><span class="sxs-lookup"><span data-stu-id="aeece-115">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="aeece-116">Klassen auflisten</span><span class="sxs-lookup"><span data-stu-id="aeece-116">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="aeece-117">[educationClass](educationclass.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="aeece-117">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="aeece-118">Abrufen einer **educationClass**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="aeece-118">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="aeece-119">EducationSchool erstellen</span><span class="sxs-lookup"><span data-stu-id="aeece-119">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="aeece-120">educationSchool</span><span class="sxs-lookup"><span data-stu-id="aeece-120">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="aeece-121">Erstellen eines neuen **educationSchool**-Objekts durch Bereitstellen in der Sammlung der Schulen.</span><span class="sxs-lookup"><span data-stu-id="aeece-121">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="aeece-122">Schulen auflisten</span><span class="sxs-lookup"><span data-stu-id="aeece-122">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="aeece-123">[educationSchool](educationschool.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="aeece-123">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="aeece-124">Abrufen einer **educationSchool**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="aeece-124">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="aeece-125">EducationUser erstellen</span><span class="sxs-lookup"><span data-stu-id="aeece-125">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="aeece-126">educationUser</span><span class="sxs-lookup"><span data-stu-id="aeece-126">educationUser</span></span>](educationuser.md)| <span data-ttu-id="aeece-127">Erstellen eines neuen **educationUser**-Objekts durch Bereitstellen in der Benutzersammlung.</span><span class="sxs-lookup"><span data-stu-id="aeece-127">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="aeece-128">Benutzer auflisten</span><span class="sxs-lookup"><span data-stu-id="aeece-128">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="aeece-129">[educationUser](educationuser.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="aeece-129">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="aeece-130">Abrufen einer **educationUser**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="aeece-130">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="aeece-131">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="aeece-131">Properties</span></span>
<span data-ttu-id="aeece-132">Keine.</span><span class="sxs-lookup"><span data-stu-id="aeece-132">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="aeece-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="aeece-133">Relationships</span></span>
| <span data-ttu-id="aeece-134">Beziehung</span><span class="sxs-lookup"><span data-stu-id="aeece-134">Relationship</span></span> | <span data-ttu-id="aeece-135">Typ</span><span class="sxs-lookup"><span data-stu-id="aeece-135">Type</span></span>   |<span data-ttu-id="aeece-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aeece-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aeece-137">classes</span><span class="sxs-lookup"><span data-stu-id="aeece-137">classes</span></span>|<span data-ttu-id="aeece-138">[educationClass](educationclass.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="aeece-138">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="aeece-p103">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="aeece-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="aeece-141">me</span><span class="sxs-lookup"><span data-stu-id="aeece-141">me</span></span>|[<span data-ttu-id="aeece-142">educationUser</span><span class="sxs-lookup"><span data-stu-id="aeece-142">educationUser</span></span>](educationuser.md)| <span data-ttu-id="aeece-p104">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="aeece-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="aeece-145">schools</span><span class="sxs-lookup"><span data-stu-id="aeece-145">schools</span></span>|<span data-ttu-id="aeece-146">[educationSchool](educationschool.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="aeece-146">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="aeece-p105">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="aeece-p105">Read-only. Nullable.</span></span>|
|<span data-ttu-id="aeece-149">users</span><span class="sxs-lookup"><span data-stu-id="aeece-149">users</span></span>|<span data-ttu-id="aeece-150">[educationUser](educationuser.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="aeece-150">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="aeece-p106">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="aeece-p106">Read-only. Nullable.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->