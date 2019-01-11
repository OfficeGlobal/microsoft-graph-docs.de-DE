---
title: Vereinbarung Ressourcentyp
description: Stellt einen Mandanten anpassbare Vertragsbedingungen verwenden, die erstellt und mit Azure Active Directory (AD Azure) verwaltet wird. Sie können die folgenden Methoden zum Erstellen und Verwalten des Azure Active Directory Ausdrücken verwenden Features gemäß Ihrem Szenario.
localization_priority: Normal
ms.openlocfilehash: 8c082ed6229b44cc3a3d4cba6dd8645feee5d07c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845346"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="fdbd4-104">Vereinbarung Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fdbd4-104">agreement resource type</span></span>

> <span data-ttu-id="fdbd4-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fdbd4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fdbd4-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fdbd4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fdbd4-107">Stellt einen Mandanten anpassbare Vertragsbedingungen verwenden, die erstellt und mit Azure Active Directory (AD Azure) verwaltet wird.</span><span class="sxs-lookup"><span data-stu-id="fdbd4-107">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="fdbd4-108">Sie können die folgenden Methoden zum Erstellen und Verwalten des [Azure Active Directory Ausdrücken verwenden Feature](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) entsprechend Ihrem Szenario.</span><span class="sxs-lookup"><span data-stu-id="fdbd4-108">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="fdbd4-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="fdbd4-109">Methods</span></span>

| <span data-ttu-id="fdbd4-110">Methode</span><span class="sxs-lookup"><span data-stu-id="fdbd4-110">Method</span></span>       | <span data-ttu-id="fdbd4-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="fdbd4-111">Return Type</span></span> | <span data-ttu-id="fdbd4-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fdbd4-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="fdbd4-113">Vereinbarungen zur erstellen</span><span class="sxs-lookup"><span data-stu-id="fdbd4-113">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="fdbd4-114">Vereinbarung</span><span class="sxs-lookup"><span data-stu-id="fdbd4-114">agreement</span></span>](agreement.md) | <span data-ttu-id="fdbd4-115">Erstellen Sie eine neue Vereinbarung durch die Veröffentlichung auf der Vereinbarung-Auflistung.</span><span class="sxs-lookup"><span data-stu-id="fdbd4-115">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="fdbd4-116">Vereinbarungen zur Liste</span><span class="sxs-lookup"><span data-stu-id="fdbd4-116">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="fdbd4-117">[Vereinbarung](agreement.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="fdbd4-117">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="fdbd4-118">Rufen Sie eine Auflistung der Vereinbarung-Objekts.</span><span class="sxs-lookup"><span data-stu-id="fdbd4-118">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="fdbd4-119">Abrufen der Vereinbarung</span><span class="sxs-lookup"><span data-stu-id="fdbd4-119">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="fdbd4-120">Vereinbarung</span><span class="sxs-lookup"><span data-stu-id="fdbd4-120">agreement</span></span>](agreement.md) | <span data-ttu-id="fdbd4-121">Lesen Sie Eigenschaften und Beziehungen eines Vereinbarung-Objekts.</span><span class="sxs-lookup"><span data-stu-id="fdbd4-121">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="fdbd4-122">Vereinbarung aktualisieren</span><span class="sxs-lookup"><span data-stu-id="fdbd4-122">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="fdbd4-123">Vereinbarung</span><span class="sxs-lookup"><span data-stu-id="fdbd4-123">agreement</span></span>](agreement.md) | <span data-ttu-id="fdbd4-124">Ein Objekt zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="fdbd4-124">Update an agreement object.</span></span> |
| [<span data-ttu-id="fdbd4-125">Vereinbarung löschen</span><span class="sxs-lookup"><span data-stu-id="fdbd4-125">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="fdbd4-126">Keine</span><span class="sxs-lookup"><span data-stu-id="fdbd4-126">None</span></span> | <span data-ttu-id="fdbd4-127">Ein Objekt zu löschen.</span><span class="sxs-lookup"><span data-stu-id="fdbd4-127">Delete an agreement object.</span></span> |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a><span data-ttu-id="fdbd4-128">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fdbd4-128">Properties</span></span>
| <span data-ttu-id="fdbd4-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fdbd4-129">Property</span></span>     | <span data-ttu-id="fdbd4-130">Typ</span><span class="sxs-lookup"><span data-stu-id="fdbd4-130">Type</span></span>        | <span data-ttu-id="fdbd4-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fdbd4-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fdbd4-132">displayName</span><span class="sxs-lookup"><span data-stu-id="fdbd4-132">displayName</span></span>|<span data-ttu-id="fdbd4-133">String</span><span class="sxs-lookup"><span data-stu-id="fdbd4-133">String</span></span>|<span data-ttu-id="fdbd4-134">Der Anzeigename der Vereinbarung.</span><span class="sxs-lookup"><span data-stu-id="fdbd4-134">Display name of the agreement.</span></span>|
|<span data-ttu-id="fdbd4-135">id</span><span class="sxs-lookup"><span data-stu-id="fdbd4-135">id</span></span>|<span data-ttu-id="fdbd4-136">String</span><span class="sxs-lookup"><span data-stu-id="fdbd4-136">String</span></span>| <span data-ttu-id="fdbd4-137">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fdbd4-137">Read-only.</span></span>|
|<span data-ttu-id="fdbd4-138">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="fdbd4-138">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="fdbd4-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdbd4-139">Boolean</span></span>|<span data-ttu-id="fdbd4-140">Gibt an, ob der Benutzer zu erweitern und vor dem akzeptieren die Vereinbarung anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="fdbd4-140">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fdbd4-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fdbd4-141">Relationships</span></span>
| <span data-ttu-id="fdbd4-142">Beziehung</span><span class="sxs-lookup"><span data-stu-id="fdbd4-142">Relationship</span></span> | <span data-ttu-id="fdbd4-143">Typ</span><span class="sxs-lookup"><span data-stu-id="fdbd4-143">Type</span></span>        | <span data-ttu-id="fdbd4-144">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fdbd4-144">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fdbd4-145">files</span><span class="sxs-lookup"><span data-stu-id="fdbd4-145">files</span></span>|<span data-ttu-id="fdbd4-146">[AgreementFile](agreementfile.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="fdbd4-146">[agreementFile](agreementfile.md) collection</span></span>|<span data-ttu-id="fdbd4-147">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fdbd4-147">Read-only.</span></span> <span data-ttu-id="fdbd4-148">PDF-Dateien mit diesem Vertrag verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="fdbd4-148">PDFs linked to this agreement.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fdbd4-149">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fdbd4-149">JSON representation</span></span>

<span data-ttu-id="fdbd4-150">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fdbd4-150">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreement"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "isViewingBeforeAcceptanceRequired": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "agreement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
