---
title: Ressourcentyp educationSynchronizationError
description: Stellt einen Fehler bei der Validierung der Schule Profil und/oder Sync dar. Für jeden Eintrag, der nicht überprüfen und/oder Synchronisieren mit Azure Active Directory (AD Azure), ist ein eindeutiger Fehler generiert.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2808ba0fd633fcdcbbaa32ce63162ac1cd4531ff
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944726"
---
# <a name="educationsynchronizationerror-resource-type"></a><span data-ttu-id="28562-103">Ressourcentyp educationSynchronizationError</span><span class="sxs-lookup"><span data-stu-id="28562-103">educationSynchronizationError resource type</span></span>

> <span data-ttu-id="28562-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="28562-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="28562-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="28562-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="28562-106">Stellt einen Fehler bei der Validierung der Schule Profil und/oder Sync dar. Für jeden Eintrag, der nicht überprüfen und/oder Synchronisieren mit Azure Active Directory (AD Azure), ist ein eindeutiger Fehler generiert.</span><span class="sxs-lookup"><span data-stu-id="28562-106">Represents an error during school data profile validation and/or sync. A unique error is generated for every entry that fails to validate and/or synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="28562-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="28562-107">Methods</span></span>

| <span data-ttu-id="28562-108">Methode</span><span class="sxs-lookup"><span data-stu-id="28562-108">Method</span></span> | <span data-ttu-id="28562-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="28562-109">Return Type</span></span> | <span data-ttu-id="28562-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28562-110">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="28562-111">Abrufen von Synchronisierungsfehler</span><span class="sxs-lookup"><span data-stu-id="28562-111">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="28562-112">**EducationSynchronizationError** -Auflistung</span><span class="sxs-lookup"><span data-stu-id="28562-112">**educationSynchronizationError** collection</span></span>| <span data-ttu-id="28562-113">Gibt die Liste der Synchronisierungsfehler im Zusammenhang mit einem Profil.</span><span class="sxs-lookup"><span data-stu-id="28562-113">Returns the list of synchronization errors associated with a profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="28562-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="28562-114">Properties</span></span>

| <span data-ttu-id="28562-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="28562-115">Property</span></span> | <span data-ttu-id="28562-116">Typ</span><span class="sxs-lookup"><span data-stu-id="28562-116">Type</span></span> | <span data-ttu-id="28562-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28562-117">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="28562-118">**entryType**</span><span class="sxs-lookup"><span data-stu-id="28562-118">**entryType**</span></span> | <span data-ttu-id="28562-119">string</span><span class="sxs-lookup"><span data-stu-id="28562-119">string</span></span> |  <span data-ttu-id="28562-120">Stellt die Sync-Entität (Schule, Abschnitt, Student, Lehrer).</span><span class="sxs-lookup"><span data-stu-id="28562-120">Represents the sync entity (school, section, student, teacher).</span></span>       |
| <span data-ttu-id="28562-121">**<ui>errorCode</ui>**</span><span class="sxs-lookup"><span data-stu-id="28562-121">**errorCode**</span></span> | <span data-ttu-id="28562-122">string</span><span class="sxs-lookup"><span data-stu-id="28562-122">string</span></span> |  <span data-ttu-id="28562-123">Stellt den Fehlercode für diesen Fehler.</span><span class="sxs-lookup"><span data-stu-id="28562-123">Represents the error code for this error.</span></span>         |
| <span data-ttu-id="28562-124">**errorMessage**</span><span class="sxs-lookup"><span data-stu-id="28562-124">**errorMessage**</span></span> | <span data-ttu-id="28562-125">string</span><span class="sxs-lookup"><span data-stu-id="28562-125">string</span></span> |  <span data-ttu-id="28562-126">Enthält eine Beschreibung des Fehlers.</span><span class="sxs-lookup"><span data-stu-id="28562-126">Contains a description of the error.</span></span>        |
| <span data-ttu-id="28562-127">**joiningValue**</span><span class="sxs-lookup"><span data-stu-id="28562-127">**joiningValue**</span></span> | <span data-ttu-id="28562-128">string</span><span class="sxs-lookup"><span data-stu-id="28562-128">string</span></span> |  <span data-ttu-id="28562-129">Der eindeutige Bezeichner für den Eintrag.</span><span class="sxs-lookup"><span data-stu-id="28562-129">The unique identifier for the entry.</span></span>         |
| <span data-ttu-id="28562-130">**recordedDateTime**</span><span class="sxs-lookup"><span data-stu-id="28562-130">**recordedDateTime**</span></span> | <span data-ttu-id="28562-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28562-131">DateTimeOffset</span></span> | <span data-ttu-id="28562-132">Der Zeitpunkt des Auftretens dieses Fehlers.</span><span class="sxs-lookup"><span data-stu-id="28562-132">The time of occurrence of this error.</span></span>         |
| <span data-ttu-id="28562-133">**reportableIdentifier**</span><span class="sxs-lookup"><span data-stu-id="28562-133">**reportableIdentifier**</span></span> | <span data-ttu-id="28562-134">string</span><span class="sxs-lookup"><span data-stu-id="28562-134">string</span></span> | <span data-ttu-id="28562-135">Der Bezeichner für diesen Fehlereintrag.</span><span class="sxs-lookup"><span data-stu-id="28562-135">The identifier of this error entry.</span></span>       |

## <a name="json-representation"></a><span data-ttu-id="28562-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="28562-136">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationError"
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
