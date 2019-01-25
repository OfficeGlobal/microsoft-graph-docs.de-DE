---
title: Ressourcentyp secureScores
description: 'Top n =, wobei n = Anzahl der Tage, die Daten, die Sie abrufen möchten. '
localization_priority: Normal
ms.openlocfilehash: 8b4be9822b782303efe38dbdf5bd43e1ee543421
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528662"
---
# <a name="securescores-resource-type"></a><span data-ttu-id="40d8d-103">Ressourcentyp secureScores</span><span class="sxs-lookup"><span data-stu-id="40d8d-103">secureScores resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40d8d-104">Stellt einen Mandanten sichere Faktor pro Tag der Daten, auf der Ebene Mandanten und Steuerelement bewerten.</span><span class="sxs-lookup"><span data-stu-id="40d8d-104">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="40d8d-105">In der Standardeinstellung ist 90 Tage von Daten enthalten.</span><span class="sxs-lookup"><span data-stu-id="40d8d-105">By default, 90 days of data is held.</span></span> <span data-ttu-id="40d8d-106">Diese Daten sortiert spätesten zum frühesten durch **CreatedDateTime**, aus.</span><span class="sxs-lookup"><span data-stu-id="40d8d-106">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="40d8d-107">Dadurch können Sie auf der Seitenantworten mithilfe von $top = n, wobei n = Anzahl der Tage, die Daten, die Sie abrufen möchten.</span><span class="sxs-lookup"><span data-stu-id="40d8d-107">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="40d8d-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="40d8d-108">Methods</span></span>

| <span data-ttu-id="40d8d-109">Methode</span><span class="sxs-lookup"><span data-stu-id="40d8d-109">Method</span></span>   | <span data-ttu-id="40d8d-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="40d8d-110">Return Type</span></span>|<span data-ttu-id="40d8d-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="40d8d-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="40d8d-112">List secureScores</span><span class="sxs-lookup"><span data-stu-id="40d8d-112">List secureScores</span></span>](../api/securescores-list.md) | [<span data-ttu-id="40d8d-113">secureScores</span><span class="sxs-lookup"><span data-stu-id="40d8d-113">secureScores</span></span>](securescores.md) |<span data-ttu-id="40d8d-114">Lesen Sie Eigenschaften und Metadaten eines SecureScores-Objekts.</span><span class="sxs-lookup"><span data-stu-id="40d8d-114">Read properties and metadata of a secureScores object.</span></span>|


## <a name="properties"></a><span data-ttu-id="40d8d-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="40d8d-115">Properties</span></span>
<span data-ttu-id="40d8d-116">Typ mit Eigenschaften der Mandant Sicherheit Entität Punktzahl (tägliche Momentaufnahme Daten).</span><span class="sxs-lookup"><span data-stu-id="40d8d-116">Entity type containing properties of the tenant security score (daily snapshot data).</span></span>

|<span data-ttu-id="40d8d-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="40d8d-117">Property</span></span> |<span data-ttu-id="40d8d-118">Typ</span><span class="sxs-lookup"><span data-stu-id="40d8d-118">Type</span></span> |<span data-ttu-id="40d8d-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="40d8d-119">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="40d8d-120">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="40d8d-120">azureTenantId</span></span>   |   <span data-ttu-id="40d8d-121">String</span><span class="sxs-lookup"><span data-stu-id="40d8d-121">String</span></span>  |   <span data-ttu-id="40d8d-122">GUID-Zeichenfolge für Mandanten-ID ein.</span><span class="sxs-lookup"><span data-stu-id="40d8d-122">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="40d8d-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="40d8d-123">createdDateTime</span></span> |   <span data-ttu-id="40d8d-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40d8d-124">DateTimeOffset</span></span>  |   <span data-ttu-id="40d8d-125">Das Datum, wenn die Entität erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="40d8d-125">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="40d8d-126">id</span><span class="sxs-lookup"><span data-stu-id="40d8d-126">id</span></span>  |   <span data-ttu-id="40d8d-127">String</span><span class="sxs-lookup"><span data-stu-id="40d8d-127">String</span></span>  |   <span data-ttu-id="40d8d-128">Kombination von AzureTenantId_createdDateTime.</span><span class="sxs-lookup"><span data-stu-id="40d8d-128">Combination of azureTenantId_createdDateTime.</span></span>   |
|   <span data-ttu-id="40d8d-129">licensedUserCount</span><span class="sxs-lookup"><span data-stu-id="40d8d-129">licensedUserCount</span></span>   |   <span data-ttu-id="40d8d-130">Int32</span><span class="sxs-lookup"><span data-stu-id="40d8d-130">Int32</span></span>   |   <span data-ttu-id="40d8d-131">Die Anzahl der Benutzer des angegebenen Mandanten lizenziert.</span><span class="sxs-lookup"><span data-stu-id="40d8d-131">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="40d8d-132">activeUserCount</span><span class="sxs-lookup"><span data-stu-id="40d8d-132">activeUserCount</span></span> |   <span data-ttu-id="40d8d-133">Int32</span><span class="sxs-lookup"><span data-stu-id="40d8d-133">Int32</span></span>   |   <span data-ttu-id="40d8d-134">Aktive Benutzeranzahl des angegebenen Mandanten.</span><span class="sxs-lookup"><span data-stu-id="40d8d-134">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="40d8d-135">currentScore</span><span class="sxs-lookup"><span data-stu-id="40d8d-135">currentScore</span></span>    |   <span data-ttu-id="40d8d-136">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="40d8d-136">Double</span></span>  |   <span data-ttu-id="40d8d-137">Mandanten aktuellen erreicht Score am angegebenen Datum.</span><span class="sxs-lookup"><span data-stu-id="40d8d-137">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="40d8d-138">MaxErgebnis</span><span class="sxs-lookup"><span data-stu-id="40d8d-138">maxScore</span></span> |  <span data-ttu-id="40d8d-139">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="40d8d-139">Double</span></span>  |   <span data-ttu-id="40d8d-140">Mandanten maximale Bewertung am angegebenen Datum.</span><span class="sxs-lookup"><span data-stu-id="40d8d-140">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="40d8d-141">enabledServices</span><span class="sxs-lookup"><span data-stu-id="40d8d-141">enabledServices</span></span> |   <span data-ttu-id="40d8d-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="40d8d-142">String collection</span></span>   |   <span data-ttu-id="40d8d-143">Microsoft-Dienste für den Mandanten (beispielsweise Exchange online, Skype, Sharepoint).</span><span class="sxs-lookup"><span data-stu-id="40d8d-143">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="40d8d-144">averageComparativeScores</span><span class="sxs-lookup"><span data-stu-id="40d8d-144">averageComparativeScores</span></span> |  <span data-ttu-id="40d8d-145">[AverageComparativeScore](averagecomparativescore.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="40d8d-145">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="40d8d-146">Durchschnittliche Bewertung von unterschiedlichen Bereichen (beispielsweise Durchschnitt nach Branche, durchschnittliche durch Sitzplätze) und Steuerelement Kategorie (Identität, Daten, Gerät, Apps, Infrastruktur) innerhalb des Bereichs.</span><span class="sxs-lookup"><span data-stu-id="40d8d-146">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="40d8d-147">controlScores</span><span class="sxs-lookup"><span data-stu-id="40d8d-147">controlScores</span></span> | <span data-ttu-id="40d8d-148">[ControlScore](controlscore.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="40d8d-148">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="40d8d-149">Mandanten Bewertungen für eine Gruppe von Steuerelementen enthält.</span><span class="sxs-lookup"><span data-stu-id="40d8d-149">Contains tenant scores for a set of controls.</span></span>   |


## <a name="relationships"></a><span data-ttu-id="40d8d-150">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="40d8d-150">Relationships</span></span>

<span data-ttu-id="40d8d-151">Keine.</span><span class="sxs-lookup"><span data-stu-id="40d8d-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="40d8d-152">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="40d8d-152">JSON representation</span></span>

<span data-ttu-id="40d8d-153">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="40d8d-153">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScores"
}-->

```json
{
"id": "String",
"azureTenantId": "Guid",
"createdDate": "DateTimeOffset",
"licensedUserCount": "Int32",
"activeUserCount": "Int32",
"currentScore": "Int32",
"maxScore": "Int32",
"averageScore": "Double",
"enabledServices": "Collection(string)",
"averageComparativeScores": "Collection(microsoft.graph.SecureScore.averageComparativeScores)",
"controlScores": "Collection(microsoft.graph.SecureScore.controlScores)",
}

```


<!--
{
  "type": "#page.annotation",
  "description": "secureScores resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/securescores.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
