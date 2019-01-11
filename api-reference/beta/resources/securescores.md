---
title: Ressourcentyp secureScores
description: 'Top n =, wobei n = Anzahl der Tage, die Daten, die Sie abrufen möchten. '
localization_priority: Normal
ms.openlocfilehash: 332a9656d8237bb07d5c7739b666e09539cf984f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828735"
---
# <a name="securescores-resource-type"></a><span data-ttu-id="196b9-103">Ressourcentyp secureScores</span><span class="sxs-lookup"><span data-stu-id="196b9-103">secureScores resource type</span></span>

> <span data-ttu-id="196b9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="196b9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="196b9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="196b9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="196b9-106">Stellt einen Mandanten sichere Faktor pro Tag der Daten, auf der Ebene Mandanten und Steuerelement bewerten.</span><span class="sxs-lookup"><span data-stu-id="196b9-106">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="196b9-107">In der Standardeinstellung ist 90 Tage von Daten enthalten.</span><span class="sxs-lookup"><span data-stu-id="196b9-107">By default, 90 days of data is held.</span></span> <span data-ttu-id="196b9-108">Diese Daten sortiert spätesten zum frühesten durch **CreatedDateTime**, aus.</span><span class="sxs-lookup"><span data-stu-id="196b9-108">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="196b9-109">Dadurch können Sie auf der Seitenantworten mithilfe von $top = n, wobei n = Anzahl der Tage, die Daten, die Sie abrufen möchten.</span><span class="sxs-lookup"><span data-stu-id="196b9-109">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="196b9-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="196b9-110">Methods</span></span>

| <span data-ttu-id="196b9-111">Methode</span><span class="sxs-lookup"><span data-stu-id="196b9-111">Method</span></span>   | <span data-ttu-id="196b9-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="196b9-112">Return Type</span></span>|<span data-ttu-id="196b9-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="196b9-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="196b9-114">List secureScores</span><span class="sxs-lookup"><span data-stu-id="196b9-114">List secureScores</span></span>](../api/securescores-list.md) | [<span data-ttu-id="196b9-115">secureScores</span><span class="sxs-lookup"><span data-stu-id="196b9-115">secureScores</span></span>](securescores.md) |<span data-ttu-id="196b9-116">Lesen Sie Eigenschaften und Metadaten eines SecureScores-Objekts.</span><span class="sxs-lookup"><span data-stu-id="196b9-116">Read properties and metadata of a secureScores object.</span></span>|


## <a name="properties"></a><span data-ttu-id="196b9-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="196b9-117">Properties</span></span>
<span data-ttu-id="196b9-118">Typ mit Eigenschaften der Mandant Sicherheit Entität Punktzahl (tägliche Momentaufnahme Daten).</span><span class="sxs-lookup"><span data-stu-id="196b9-118">Entity type containing properties of the tenant security score (daily snapshot data).</span></span>

|<span data-ttu-id="196b9-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="196b9-119">Property</span></span> |<span data-ttu-id="196b9-120">Typ</span><span class="sxs-lookup"><span data-stu-id="196b9-120">Type</span></span> |<span data-ttu-id="196b9-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="196b9-121">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="196b9-122">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="196b9-122">azureTenantId</span></span>   |   <span data-ttu-id="196b9-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="196b9-123">String</span></span>  |   <span data-ttu-id="196b9-124">GUID-Zeichenfolge für Mandanten-ID ein.</span><span class="sxs-lookup"><span data-stu-id="196b9-124">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="196b9-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="196b9-125">createdDateTime</span></span> |   <span data-ttu-id="196b9-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="196b9-126">DateTimeOffset</span></span>  |   <span data-ttu-id="196b9-127">Das Datum, wenn die Entität erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="196b9-127">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="196b9-128">id</span><span class="sxs-lookup"><span data-stu-id="196b9-128">id</span></span>  |   <span data-ttu-id="196b9-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="196b9-129">String</span></span>  |   <span data-ttu-id="196b9-130">Kombination von AzureTenantId_createdDateTime.</span><span class="sxs-lookup"><span data-stu-id="196b9-130">Combination of azureTenantId_createdDateTime.</span></span>   |
|   <span data-ttu-id="196b9-131">licensedUserCount</span><span class="sxs-lookup"><span data-stu-id="196b9-131">licensedUserCount</span></span>   |   <span data-ttu-id="196b9-132">Int32</span><span class="sxs-lookup"><span data-stu-id="196b9-132">Int32</span></span>   |   <span data-ttu-id="196b9-133">Die Anzahl der Benutzer des angegebenen Mandanten lizenziert.</span><span class="sxs-lookup"><span data-stu-id="196b9-133">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="196b9-134">activeUserCount</span><span class="sxs-lookup"><span data-stu-id="196b9-134">activeUserCount</span></span> |   <span data-ttu-id="196b9-135">Int32</span><span class="sxs-lookup"><span data-stu-id="196b9-135">Int32</span></span>   |   <span data-ttu-id="196b9-136">Aktive Benutzeranzahl des angegebenen Mandanten.</span><span class="sxs-lookup"><span data-stu-id="196b9-136">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="196b9-137">currentScore</span><span class="sxs-lookup"><span data-stu-id="196b9-137">currentScore</span></span>    |   <span data-ttu-id="196b9-138">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="196b9-138">Double</span></span>  |   <span data-ttu-id="196b9-139">Mandanten aktuellen erreicht Score am angegebenen Datum.</span><span class="sxs-lookup"><span data-stu-id="196b9-139">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="196b9-140">MaxErgebnis</span><span class="sxs-lookup"><span data-stu-id="196b9-140">maxScore</span></span> |  <span data-ttu-id="196b9-141">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="196b9-141">Double</span></span>  |   <span data-ttu-id="196b9-142">Mandanten maximale Bewertung am angegebenen Datum.</span><span class="sxs-lookup"><span data-stu-id="196b9-142">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="196b9-143">enabledServices</span><span class="sxs-lookup"><span data-stu-id="196b9-143">enabledServices</span></span> |   <span data-ttu-id="196b9-144">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="196b9-144">String collection</span></span>   |   <span data-ttu-id="196b9-145">Microsoft-Dienste für den Mandanten (beispielsweise Exchange online, Skype, Sharepoint).</span><span class="sxs-lookup"><span data-stu-id="196b9-145">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="196b9-146">averageComparativeScores</span><span class="sxs-lookup"><span data-stu-id="196b9-146">averageComparativeScores</span></span> |  <span data-ttu-id="196b9-147">[AverageComparativeScore](averagecomparativescore.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="196b9-147">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="196b9-148">Durchschnittliche Bewertung von unterschiedlichen Bereichen (beispielsweise Durchschnitt nach Branche, durchschnittliche durch Sitzplätze) und Steuerelement Kategorie (Identität, Daten, Gerät, Apps, Infrastruktur) innerhalb des Bereichs.</span><span class="sxs-lookup"><span data-stu-id="196b9-148">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="196b9-149">controlScores</span><span class="sxs-lookup"><span data-stu-id="196b9-149">controlScores</span></span> | <span data-ttu-id="196b9-150">[ControlScore](controlscore.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="196b9-150">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="196b9-151">Mandanten Bewertungen für eine Gruppe von Steuerelementen enthält.</span><span class="sxs-lookup"><span data-stu-id="196b9-151">Contains tenant scores for a set of controls.</span></span>   |


## <a name="relationships"></a><span data-ttu-id="196b9-152">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="196b9-152">Relationships</span></span>

<span data-ttu-id="196b9-153">Keine.</span><span class="sxs-lookup"><span data-stu-id="196b9-153">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="196b9-154">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="196b9-154">JSON representation</span></span>

<span data-ttu-id="196b9-155">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="196b9-155">The following is a JSON representation of the resource.</span></span>

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


<!-- {
  "type": "#page.annotation",
  "description": "secureScores resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
