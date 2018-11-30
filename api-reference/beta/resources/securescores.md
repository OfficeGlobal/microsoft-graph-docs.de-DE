---
title: Ressourcentyp secureScores
description: 'Top n =, wobei n = Anzahl der Tage, die Daten, die Sie abrufen möchten. '
ms.openlocfilehash: 96d5c487bb854559b0128d93ea8e0783fcc61f0c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058982"
---
# <a name="securescores-resource-type"></a><span data-ttu-id="0f5c1-103">Ressourcentyp secureScores</span><span class="sxs-lookup"><span data-stu-id="0f5c1-103">secureScores resource type</span></span>

> <span data-ttu-id="0f5c1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0f5c1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f5c1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0f5c1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0f5c1-106">Stellt einen Mandanten sichere Faktor pro Tag der Daten, auf der Ebene Mandanten und Steuerelement bewerten.</span><span class="sxs-lookup"><span data-stu-id="0f5c1-106">Represents a tenant's secure score per day of scoring data, at the tenant and control level.</span></span> <span data-ttu-id="0f5c1-107">In der Standardeinstellung ist 90 Tage von Daten enthalten.</span><span class="sxs-lookup"><span data-stu-id="0f5c1-107">By default, 90 days of data is held.</span></span> <span data-ttu-id="0f5c1-108">Diese Daten sortiert spätesten zum frühesten durch **CreatedDateTime**, aus.</span><span class="sxs-lookup"><span data-stu-id="0f5c1-108">This data is sorted by **createdDateTime**, from latest to earliest.</span></span> <span data-ttu-id="0f5c1-109">Dadurch können Sie auf der Seitenantworten mithilfe von $top = n, wobei n = Anzahl der Tage, die Daten, die Sie abrufen möchten.</span><span class="sxs-lookup"><span data-stu-id="0f5c1-109">This will allow you to page responses by using $top=n, where n = the number of days of data that you want to retrieve.</span></span> 


## <a name="methods"></a><span data-ttu-id="0f5c1-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="0f5c1-110">Methods</span></span>

| <span data-ttu-id="0f5c1-111">Methode</span><span class="sxs-lookup"><span data-stu-id="0f5c1-111">Method</span></span>   | <span data-ttu-id="0f5c1-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="0f5c1-112">Return Type</span></span>|<span data-ttu-id="0f5c1-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f5c1-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0f5c1-114">Liste secureScores</span><span class="sxs-lookup"><span data-stu-id="0f5c1-114">List secureScores</span></span>](../api/securescores-list.md) | [<span data-ttu-id="0f5c1-115">secureScores</span><span class="sxs-lookup"><span data-stu-id="0f5c1-115">secureScores</span></span>](securescores.md) |<span data-ttu-id="0f5c1-116">Lesen Sie Eigenschaften und Metadaten eines SecureScores-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0f5c1-116">Read properties and metadata of a secureScores object.</span></span>|


## <a name="properties"></a><span data-ttu-id="0f5c1-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0f5c1-117">Properties</span></span>
<span data-ttu-id="0f5c1-118">Typ mit Eigenschaften der Mandant Sicherheit Entität Punktzahl (tägliche Momentaufnahme Daten).</span><span class="sxs-lookup"><span data-stu-id="0f5c1-118">Entity type containing properties of the tenant security score (daily snapshot data).</span></span>

|<span data-ttu-id="0f5c1-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0f5c1-119">Property</span></span> |<span data-ttu-id="0f5c1-120">Typ</span><span class="sxs-lookup"><span data-stu-id="0f5c1-120">Type</span></span> |<span data-ttu-id="0f5c1-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f5c1-121">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="0f5c1-122">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="0f5c1-122">azureTenantId</span></span>   |   <span data-ttu-id="0f5c1-123">String</span><span class="sxs-lookup"><span data-stu-id="0f5c1-123">String</span></span>  |   <span data-ttu-id="0f5c1-124">GUID-Zeichenfolge für Mandanten-ID ein.</span><span class="sxs-lookup"><span data-stu-id="0f5c1-124">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="0f5c1-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f5c1-125">createdDateTime</span></span> |   <span data-ttu-id="0f5c1-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f5c1-126">DateTimeOffset</span></span>  |   <span data-ttu-id="0f5c1-127">Das Datum, wenn die Entität erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="0f5c1-127">The date when the entity is created.</span></span>  |
|   <span data-ttu-id="0f5c1-128">id</span><span class="sxs-lookup"><span data-stu-id="0f5c1-128">id</span></span>  |   <span data-ttu-id="0f5c1-129">String</span><span class="sxs-lookup"><span data-stu-id="0f5c1-129">String</span></span>  |   <span data-ttu-id="0f5c1-130">Kombination von AzureTenantId_createdDateTime.</span><span class="sxs-lookup"><span data-stu-id="0f5c1-130">Combination of azureTenantId_createdDateTime.</span></span>   |
|   <span data-ttu-id="0f5c1-131">licensedUserCount</span><span class="sxs-lookup"><span data-stu-id="0f5c1-131">licensedUserCount</span></span>   |   <span data-ttu-id="0f5c1-132">Int32</span><span class="sxs-lookup"><span data-stu-id="0f5c1-132">Int32</span></span>   |   <span data-ttu-id="0f5c1-133">Die Anzahl der Benutzer des angegebenen Mandanten lizenziert.</span><span class="sxs-lookup"><span data-stu-id="0f5c1-133">Licensed user count of the given tenant.</span></span>    |
|   <span data-ttu-id="0f5c1-134">activeUserCount</span><span class="sxs-lookup"><span data-stu-id="0f5c1-134">activeUserCount</span></span> |   <span data-ttu-id="0f5c1-135">Int32</span><span class="sxs-lookup"><span data-stu-id="0f5c1-135">Int32</span></span>   |   <span data-ttu-id="0f5c1-136">Aktive Benutzeranzahl des angegebenen Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0f5c1-136">Active user count of the given tenant.</span></span>  |
|   <span data-ttu-id="0f5c1-137">currentScore</span><span class="sxs-lookup"><span data-stu-id="0f5c1-137">currentScore</span></span>    |   <span data-ttu-id="0f5c1-138">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="0f5c1-138">Double</span></span>  |   <span data-ttu-id="0f5c1-139">Mandanten aktuellen erreicht Score am angegebenen Datum.</span><span class="sxs-lookup"><span data-stu-id="0f5c1-139">Tenant current attained score on specified date.</span></span>    |
|   <span data-ttu-id="0f5c1-140">MaxErgebnis</span><span class="sxs-lookup"><span data-stu-id="0f5c1-140">maxScore</span></span> |  <span data-ttu-id="0f5c1-141">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="0f5c1-141">Double</span></span>  |   <span data-ttu-id="0f5c1-142">Mandanten maximale Bewertung am angegebenen Datum.</span><span class="sxs-lookup"><span data-stu-id="0f5c1-142">Tenant maximum possible score on specified date.</span></span>    |
|   <span data-ttu-id="0f5c1-143">enabledServices</span><span class="sxs-lookup"><span data-stu-id="0f5c1-143">enabledServices</span></span> |   <span data-ttu-id="0f5c1-144">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="0f5c1-144">String collection</span></span>   |   <span data-ttu-id="0f5c1-145">Microsoft-Dienste für den Mandanten (beispielsweise Exchange online, Skype, Sharepoint).</span><span class="sxs-lookup"><span data-stu-id="0f5c1-145">Microsoft-provided services for the tenant (for example, Exchange online, Skype, Sharepoint).</span></span>   |
|   <span data-ttu-id="0f5c1-146">averageComparativeScores</span><span class="sxs-lookup"><span data-stu-id="0f5c1-146">averageComparativeScores</span></span> |  <span data-ttu-id="0f5c1-147">[AverageComparativeScore](averagecomparativescore.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="0f5c1-147">[averageComparativeScore](averagecomparativescore.md) collection</span></span>    |<span data-ttu-id="0f5c1-148">Durchschnittliche Bewertung von unterschiedlichen Bereichen (beispielsweise Durchschnitt nach Branche, durchschnittliche durch Sitzplätze) und Steuerelement Kategorie (Identität, Daten, Gerät, Apps, Infrastruktur) innerhalb des Bereichs.</span><span class="sxs-lookup"><span data-stu-id="0f5c1-148">Average score by different scopes (for example, average by industry, average by seating) and control category (Identity, Data, Device, Apps, Infrastructure) within the scope.</span></span> |
|   <span data-ttu-id="0f5c1-149">controlScores</span><span class="sxs-lookup"><span data-stu-id="0f5c1-149">controlScores</span></span> | <span data-ttu-id="0f5c1-150">[ControlScore](controlscore.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="0f5c1-150">[controlScore](controlscore.md) collection</span></span>  |   <span data-ttu-id="0f5c1-151">Mandanten Bewertungen für eine Gruppe von Steuerelementen enthält.</span><span class="sxs-lookup"><span data-stu-id="0f5c1-151">Contains tenant scores for a set of controls.</span></span>   |


## <a name="relationships"></a><span data-ttu-id="0f5c1-152">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0f5c1-152">Relationships</span></span>

<span data-ttu-id="0f5c1-153">Keine.</span><span class="sxs-lookup"><span data-stu-id="0f5c1-153">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f5c1-154">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0f5c1-154">JSON representation</span></span>

<span data-ttu-id="0f5c1-155">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0f5c1-155">The following is a JSON representation of the resource.</span></span>

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
