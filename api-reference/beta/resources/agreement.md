---
title: Vereinbarung Ressourcentyp
description: Stellt einen Mandanten anpassbare Vertragsbedingungen verwenden, die erstellt und mit Azure Active Directory (AD Azure) verwaltet wird. Sie können die folgenden Methoden zum Erstellen und Verwalten des Azure Active Directory Ausdrücken verwenden Features gemäß Ihrem Szenario.
localization_priority: Normal
ms.openlocfilehash: b253877f1bf82e4fbc61cebaef3c1bce208d9cca
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513851"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="779a5-104">Vereinbarung Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="779a5-104">agreement resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="779a5-105">Stellt einen Mandanten anpassbare Vertragsbedingungen verwenden, die erstellt und mit Azure Active Directory (AD Azure) verwaltet wird.</span><span class="sxs-lookup"><span data-stu-id="779a5-105">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="779a5-106">Sie können die folgenden Methoden zum Erstellen und Verwalten des [Azure Active Directory Ausdrücken verwenden Feature](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) entsprechend Ihrem Szenario.</span><span class="sxs-lookup"><span data-stu-id="779a5-106">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="779a5-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="779a5-107">Methods</span></span>

| <span data-ttu-id="779a5-108">Methode</span><span class="sxs-lookup"><span data-stu-id="779a5-108">Method</span></span>       | <span data-ttu-id="779a5-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="779a5-109">Return Type</span></span> | <span data-ttu-id="779a5-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="779a5-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="779a5-111">Vereinbarungen zur erstellen</span><span class="sxs-lookup"><span data-stu-id="779a5-111">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="779a5-112">Vereinbarung</span><span class="sxs-lookup"><span data-stu-id="779a5-112">agreement</span></span>](agreement.md) | <span data-ttu-id="779a5-113">Erstellen Sie eine neue Vereinbarung durch die Veröffentlichung auf der Vereinbarung-Auflistung.</span><span class="sxs-lookup"><span data-stu-id="779a5-113">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="779a5-114">Vereinbarungen zur Liste</span><span class="sxs-lookup"><span data-stu-id="779a5-114">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="779a5-115">[Vereinbarung](agreement.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="779a5-115">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="779a5-116">Rufen Sie eine Auflistung der Vereinbarung-Objekts.</span><span class="sxs-lookup"><span data-stu-id="779a5-116">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="779a5-117">Abrufen der Vereinbarung</span><span class="sxs-lookup"><span data-stu-id="779a5-117">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="779a5-118">Vereinbarung</span><span class="sxs-lookup"><span data-stu-id="779a5-118">agreement</span></span>](agreement.md) | <span data-ttu-id="779a5-119">Lesen Sie Eigenschaften und Beziehungen eines Vereinbarung-Objekts.</span><span class="sxs-lookup"><span data-stu-id="779a5-119">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="779a5-120">Vereinbarung aktualisieren</span><span class="sxs-lookup"><span data-stu-id="779a5-120">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="779a5-121">Vereinbarung</span><span class="sxs-lookup"><span data-stu-id="779a5-121">agreement</span></span>](agreement.md) | <span data-ttu-id="779a5-122">Ein Objekt zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="779a5-122">Update an agreement object.</span></span> |
| [<span data-ttu-id="779a5-123">Vereinbarung löschen</span><span class="sxs-lookup"><span data-stu-id="779a5-123">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="779a5-124">Keine</span><span class="sxs-lookup"><span data-stu-id="779a5-124">None</span></span> | <span data-ttu-id="779a5-125">Ein Objekt zu löschen.</span><span class="sxs-lookup"><span data-stu-id="779a5-125">Delete an agreement object.</span></span> |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a><span data-ttu-id="779a5-126">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="779a5-126">Properties</span></span>
| <span data-ttu-id="779a5-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="779a5-127">Property</span></span>     | <span data-ttu-id="779a5-128">Typ</span><span class="sxs-lookup"><span data-stu-id="779a5-128">Type</span></span>        | <span data-ttu-id="779a5-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="779a5-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="779a5-130">displayName</span><span class="sxs-lookup"><span data-stu-id="779a5-130">displayName</span></span>|<span data-ttu-id="779a5-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="779a5-131">String</span></span>|<span data-ttu-id="779a5-132">Der Anzeigename der Vereinbarung.</span><span class="sxs-lookup"><span data-stu-id="779a5-132">Display name of the agreement.</span></span>|
|<span data-ttu-id="779a5-133">id</span><span class="sxs-lookup"><span data-stu-id="779a5-133">id</span></span>|<span data-ttu-id="779a5-134">String</span><span class="sxs-lookup"><span data-stu-id="779a5-134">String</span></span>| <span data-ttu-id="779a5-135">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="779a5-135">Read-only.</span></span>|
|<span data-ttu-id="779a5-136">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="779a5-136">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="779a5-137">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="779a5-137">Boolean</span></span>|<span data-ttu-id="779a5-138">Gibt an, ob der Benutzer zu erweitern und vor dem akzeptieren die Vereinbarung anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="779a5-138">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="779a5-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="779a5-139">Relationships</span></span>
| <span data-ttu-id="779a5-140">Beziehung</span><span class="sxs-lookup"><span data-stu-id="779a5-140">Relationship</span></span> | <span data-ttu-id="779a5-141">Typ</span><span class="sxs-lookup"><span data-stu-id="779a5-141">Type</span></span>        | <span data-ttu-id="779a5-142">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="779a5-142">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="779a5-143">files</span><span class="sxs-lookup"><span data-stu-id="779a5-143">files</span></span>|<span data-ttu-id="779a5-144">[AgreementFile](agreementfile.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="779a5-144">[agreementFile](agreementfile.md) collection</span></span>|<span data-ttu-id="779a5-145">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="779a5-145">Read-only.</span></span> <span data-ttu-id="779a5-146">PDF-Dateien mit diesem Vertrag verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="779a5-146">PDFs linked to this agreement.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="779a5-147">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="779a5-147">JSON representation</span></span>

<span data-ttu-id="779a5-148">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="779a5-148">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "agreement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/agreement.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
