---
title: Ressourcentyp educationSynchronizationError
description: Stellt einen Fehler bei der Validierung der Schule Profil und/oder Sync dar. Für jeden Eintrag, der nicht überprüfen und/oder Synchronisieren mit Azure Active Directory (AD Azure), ist ein eindeutiger Fehler generiert.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5c937e95441132e4633b0f5e48a75b0597b8f08d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525143"
---
# <a name="educationsynchronizationerror-resource-type"></a><span data-ttu-id="e0cd8-103">Ressourcentyp educationSynchronizationError</span><span class="sxs-lookup"><span data-stu-id="e0cd8-103">educationSynchronizationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0cd8-104">Stellt einen Fehler bei der Validierung der Schule Profil und/oder Sync dar. Für jeden Eintrag, der nicht überprüfen und/oder Synchronisieren mit Azure Active Directory (AD Azure), ist ein eindeutiger Fehler generiert.</span><span class="sxs-lookup"><span data-stu-id="e0cd8-104">Represents an error during school data profile validation and/or sync. A unique error is generated for every entry that fails to validate and/or synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="e0cd8-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="e0cd8-105">Methods</span></span>

| <span data-ttu-id="e0cd8-106">Methode</span><span class="sxs-lookup"><span data-stu-id="e0cd8-106">Method</span></span> | <span data-ttu-id="e0cd8-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e0cd8-107">Return Type</span></span> | <span data-ttu-id="e0cd8-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e0cd8-108">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="e0cd8-109">Abrufen von Synchronisierungsfehler</span><span class="sxs-lookup"><span data-stu-id="e0cd8-109">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="e0cd8-110">**EducationSynchronizationError** -Auflistung</span><span class="sxs-lookup"><span data-stu-id="e0cd8-110">**educationSynchronizationError** collection</span></span>| <span data-ttu-id="e0cd8-111">Gibt die Liste der Synchronisierungsfehler im Zusammenhang mit einem Profil.</span><span class="sxs-lookup"><span data-stu-id="e0cd8-111">Returns the list of synchronization errors associated with a profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="e0cd8-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e0cd8-112">Properties</span></span>

| <span data-ttu-id="e0cd8-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e0cd8-113">Property</span></span> | <span data-ttu-id="e0cd8-114">Typ</span><span class="sxs-lookup"><span data-stu-id="e0cd8-114">Type</span></span> | <span data-ttu-id="e0cd8-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e0cd8-115">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="e0cd8-116">**entryType**</span><span class="sxs-lookup"><span data-stu-id="e0cd8-116">**entryType**</span></span> | <span data-ttu-id="e0cd8-117">string</span><span class="sxs-lookup"><span data-stu-id="e0cd8-117">string</span></span> |  <span data-ttu-id="e0cd8-118">Stellt die Sync-Entität (Schule, Abschnitt, Student, Lehrer).</span><span class="sxs-lookup"><span data-stu-id="e0cd8-118">Represents the sync entity (school, section, student, teacher).</span></span>       |
| <span data-ttu-id="e0cd8-119">errorCode</span><span class="sxs-lookup"><span data-stu-id="e0cd8-119">**errorCode**</span></span> | <span data-ttu-id="e0cd8-120">string</span><span class="sxs-lookup"><span data-stu-id="e0cd8-120">string</span></span> |  <span data-ttu-id="e0cd8-121">Stellt den Fehlercode für diesen Fehler.</span><span class="sxs-lookup"><span data-stu-id="e0cd8-121">Represents the error code for this error.</span></span>         |
| <span data-ttu-id="e0cd8-122">error.message</span><span class="sxs-lookup"><span data-stu-id="e0cd8-122">**errorMessage**</span></span> | <span data-ttu-id="e0cd8-123">string</span><span class="sxs-lookup"><span data-stu-id="e0cd8-123">string</span></span> |  <span data-ttu-id="e0cd8-124">Enthält eine Beschreibung des Fehlers.</span><span class="sxs-lookup"><span data-stu-id="e0cd8-124">Contains a description of the error.</span></span>        |
| <span data-ttu-id="e0cd8-125">**joiningValue**</span><span class="sxs-lookup"><span data-stu-id="e0cd8-125">**joiningValue**</span></span> | <span data-ttu-id="e0cd8-126">string</span><span class="sxs-lookup"><span data-stu-id="e0cd8-126">string</span></span> |  <span data-ttu-id="e0cd8-127">Der eindeutige Bezeichner für den Eintrag.</span><span class="sxs-lookup"><span data-stu-id="e0cd8-127">The unique identifier for the entry.</span></span>         |
| <span data-ttu-id="e0cd8-128">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0cd8-128">**recordedDateTime**</span></span> | <span data-ttu-id="e0cd8-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0cd8-129">DateTimeOffset</span></span> | <span data-ttu-id="e0cd8-130">Der Zeitpunkt des Auftretens dieses Fehlers.</span><span class="sxs-lookup"><span data-stu-id="e0cd8-130">The time of occurrence of this error.</span></span>         |
| <span data-ttu-id="e0cd8-131">**reportableIdentifier**</span><span class="sxs-lookup"><span data-stu-id="e0cd8-131">**reportableIdentifier**</span></span> | <span data-ttu-id="e0cd8-132">string</span><span class="sxs-lookup"><span data-stu-id="e0cd8-132">string</span></span> | <span data-ttu-id="e0cd8-133">Der Bezeichner für diesen Fehlereintrag.</span><span class="sxs-lookup"><span data-stu-id="e0cd8-133">The identifier of this error entry.</span></span>       |

## <a name="json-representation"></a><span data-ttu-id="e0cd8-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e0cd8-134">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationError"
}-->

```json
{
    "entryType": "String",
    "errorCode": "String",
    "errorMessage": "String",
    "joiningValue": "String",
    "recordedDateTime": "DateTimeOffset",
    "reportableIdentifier": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
