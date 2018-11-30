---
title: Ressourcentyp secureScoreControlProfiles
description: Stellt einen Mandanten sichere Faktor pro Steuerelementdaten. In der Standardeinstellung alle Steuerelemente für einen Mandanten zurückgegeben und einzelne Steuerelemente können explizit abrufen.
ms.openlocfilehash: e02c9ae3b1431b131576e2e0e115377dd3480bc2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063544"
---
# <a name="securescorecontrolprofiles-resource-type"></a><span data-ttu-id="54bbd-104">Ressourcentyp secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="54bbd-104">secureScoreControlProfiles resource type</span></span>

> <span data-ttu-id="54bbd-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="54bbd-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54bbd-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="54bbd-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="54bbd-107">Stellt einen Mandanten sichere Faktor pro Steuerelementdaten.</span><span class="sxs-lookup"><span data-stu-id="54bbd-107">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="54bbd-108">In der Standardeinstellung alle Steuerelemente für einen Mandanten zurückgegeben und einzelne Steuerelemente können explizit abrufen.</span><span class="sxs-lookup"><span data-stu-id="54bbd-108">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="54bbd-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="54bbd-109">Methods</span></span>

| <span data-ttu-id="54bbd-110">Methode</span><span class="sxs-lookup"><span data-stu-id="54bbd-110">Method</span></span>   | <span data-ttu-id="54bbd-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="54bbd-111">Return Type</span></span>|<span data-ttu-id="54bbd-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="54bbd-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="54bbd-113">Liste secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="54bbd-113">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | [<span data-ttu-id="54bbd-114">secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="54bbd-114">secureScoreControlProfiles</span></span>](securescorecontrolprofiles.md) |<span data-ttu-id="54bbd-115">Lesen Sie Eigenschaften und Metadaten eines SecureScoreControlProfiles-Objekts.</span><span class="sxs-lookup"><span data-stu-id="54bbd-115">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|


## <a name="properties"></a><span data-ttu-id="54bbd-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="54bbd-116">Properties</span></span>

|<span data-ttu-id="54bbd-117">Name</span><span class="sxs-lookup"><span data-stu-id="54bbd-117">Name</span></span> |<span data-ttu-id="54bbd-118">Typ</span><span class="sxs-lookup"><span data-stu-id="54bbd-118">Type</span></span> |<span data-ttu-id="54bbd-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="54bbd-119">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="54bbd-120">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="54bbd-120">azureTenantId</span></span>   |   <span data-ttu-id="54bbd-121">String</span><span class="sxs-lookup"><span data-stu-id="54bbd-121">String</span></span>  |   <span data-ttu-id="54bbd-122">GUID-Zeichenfolge für Mandanten-ID ein.</span><span class="sxs-lookup"><span data-stu-id="54bbd-122">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="54bbd-123">Steuerelementname</span><span class="sxs-lookup"><span data-stu-id="54bbd-123">controlName</span></span> |   <span data-ttu-id="54bbd-124">String</span><span class="sxs-lookup"><span data-stu-id="54bbd-124">String</span></span>  |   <span data-ttu-id="54bbd-125">Name des Steuerelements.</span><span class="sxs-lookup"><span data-stu-id="54bbd-125">Name of the control.</span></span> |
|   <span data-ttu-id="54bbd-126">title</span><span class="sxs-lookup"><span data-stu-id="54bbd-126">title</span></span>   |   <span data-ttu-id="54bbd-127">String</span><span class="sxs-lookup"><span data-stu-id="54bbd-127">String</span></span>  |   <span data-ttu-id="54bbd-128">Titel des Steuerelements.</span><span class="sxs-lookup"><span data-stu-id="54bbd-128">Title of the control.</span></span>   |
|   <span data-ttu-id="54bbd-129">controlCategory</span><span class="sxs-lookup"><span data-stu-id="54bbd-129">controlCategory</span></span> |   <span data-ttu-id="54bbd-130">String</span><span class="sxs-lookup"><span data-stu-id="54bbd-130">String</span></span>  |   <span data-ttu-id="54bbd-131">Steuerelement-Aktionskategorie (Konto, Daten, Gerät, Apps, Infrastruktur).</span><span class="sxs-lookup"><span data-stu-id="54bbd-131">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="54bbd-132">actionType</span><span class="sxs-lookup"><span data-stu-id="54bbd-132">actionType</span></span>  |   <span data-ttu-id="54bbd-133">String</span><span class="sxs-lookup"><span data-stu-id="54bbd-133">String</span></span>  |   <span data-ttu-id="54bbd-134">Steuerelementtyp Aktion (Config überprüfen, Verhalten).</span><span class="sxs-lookup"><span data-stu-id="54bbd-134">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="54bbd-135">service</span><span class="sxs-lookup"><span data-stu-id="54bbd-135">service</span></span> |   <span data-ttu-id="54bbd-136">String</span><span class="sxs-lookup"><span data-stu-id="54bbd-136">String</span></span>  |   <span data-ttu-id="54bbd-137">Dienst, der das Steuerelement (Exchange, Sharepoint, Azure AD) besitzt.</span><span class="sxs-lookup"><span data-stu-id="54bbd-137">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="54bbd-138">MaxErgebnis</span><span class="sxs-lookup"><span data-stu-id="54bbd-138">maxScore</span></span> |  <span data-ttu-id="54bbd-139">String</span><span class="sxs-lookup"><span data-stu-id="54bbd-139">String</span></span>  |   <span data-ttu-id="54bbd-140">Aktuelle abgerufen max Score am angegebenen Datum.</span><span class="sxs-lookup"><span data-stu-id="54bbd-140">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="54bbd-141">Tier</span><span class="sxs-lookup"><span data-stu-id="54bbd-141">tier</span></span> |  <span data-ttu-id="54bbd-142">String</span><span class="sxs-lookup"><span data-stu-id="54bbd-142">String</span></span>  |   <span data-ttu-id="54bbd-143">Steuerelement-Tier (Quad-Core, mehrstufige im Detail, erweiterte.)</span><span class="sxs-lookup"><span data-stu-id="54bbd-143">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="54bbd-144">userImpact</span><span class="sxs-lookup"><span data-stu-id="54bbd-144">userImpact</span></span> |    <span data-ttu-id="54bbd-145">String</span><span class="sxs-lookup"><span data-stu-id="54bbd-145">String</span></span>  | <span data-ttu-id="54bbd-146">Beeinträchtigung für die Benutzer Implementieren von Steuerelement (niedrig, Mittel, hoch).</span><span class="sxs-lookup"><span data-stu-id="54bbd-146">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="54bbd-147">implementationCost</span><span class="sxs-lookup"><span data-stu-id="54bbd-147">implementationCost</span></span> |    <span data-ttu-id="54bbd-148">String</span><span class="sxs-lookup"><span data-stu-id="54bbd-148">String</span></span>  |   <span data-ttu-id="54bbd-149">Ressourcenkosten Implemmentating-Steuerelements (niedrig, Mittel, hoch).</span><span class="sxs-lookup"><span data-stu-id="54bbd-149">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="54bbd-150">rank</span><span class="sxs-lookup"><span data-stu-id="54bbd-150">rank</span></span> |  <span data-ttu-id="54bbd-151">Int32</span><span class="sxs-lookup"><span data-stu-id="54bbd-151">Int32</span></span>   |   <span data-ttu-id="54bbd-152">Microsoft Stapel ranking des Steuerelements.</span><span class="sxs-lookup"><span data-stu-id="54bbd-152">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="54bbd-153">Bedrohungen</span><span class="sxs-lookup"><span data-stu-id="54bbd-153">threats</span></span> |   <span data-ttu-id="54bbd-154">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="54bbd-154">String Collection</span></span>   |   <span data-ttu-id="54bbd-155">Liste der Bedrohungen für das Steuerelement reduziert (AccountBreach, DataDeletion, DataExfiltration, DataSpillage, ElevationOfPrivilege, MaliciousInsider, PasswordCracking, PhishingOrWhaling, spoofing).</span><span class="sxs-lookup"><span data-stu-id="54bbd-155">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="54bbd-156">veraltet</span><span class="sxs-lookup"><span data-stu-id="54bbd-156">deprecated</span></span> |    <span data-ttu-id="54bbd-157">Boolesch</span><span class="sxs-lookup"><span data-stu-id="54bbd-157">Boolean</span></span> |   <span data-ttu-id="54bbd-158">Flag, das angibt, ob ein Steuerelement abgeschrieben wird.</span><span class="sxs-lookup"><span data-stu-id="54bbd-158">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="54bbd-159">Wartung</span><span class="sxs-lookup"><span data-stu-id="54bbd-159">remediation</span></span> |   <span data-ttu-id="54bbd-160">String</span><span class="sxs-lookup"><span data-stu-id="54bbd-160">String</span></span>  |   <span data-ttu-id="54bbd-161">Beschreibung, wie das Steuerelement helfen warten.</span><span class="sxs-lookup"><span data-stu-id="54bbd-161">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="54bbd-162">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="54bbd-162">remediationImpact</span></span> | <span data-ttu-id="54bbd-163">String</span><span class="sxs-lookup"><span data-stu-id="54bbd-163">String</span></span>  |   <span data-ttu-id="54bbd-164">Beschreibung der Auswirkung auf den Benutzer von der Wartung.</span><span class="sxs-lookup"><span data-stu-id="54bbd-164">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="54bbd-165">actionUrl</span><span class="sxs-lookup"><span data-stu-id="54bbd-165">actionUrl</span></span> | <span data-ttu-id="54bbd-166">String</span><span class="sxs-lookup"><span data-stu-id="54bbd-166">String</span></span>  |   <span data-ttu-id="54bbd-167">URL zu, in dem das Steuerelement verarbeitet werden kann.</span><span class="sxs-lookup"><span data-stu-id="54bbd-167">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="54bbd-168">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="54bbd-168">controlStateUpdates</span></span> |   <span data-ttu-id="54bbd-169">String</span><span class="sxs-lookup"><span data-stu-id="54bbd-169">String</span></span>  |   <span data-ttu-id="54bbd-170">Kennzeichnung, die angibt, für der Mandanten ein Steuerelement markiert wurde (ignorieren, ThirdParty, überprüft) (unterstützt [Aktualisieren](../api/securescorecontrolprofiles-update.md)).</span><span class="sxs-lookup"><span data-stu-id="54bbd-170">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |
|   <span data-ttu-id="54bbd-171">tenantNote</span><span class="sxs-lookup"><span data-stu-id="54bbd-171">tenantNote</span></span> |    <span data-ttu-id="54bbd-172">String</span><span class="sxs-lookup"><span data-stu-id="54bbd-172">String</span></span>  |   <span data-ttu-id="54bbd-173">Mandanten kann pro Steuerelement Kommentare (unterstützt [Aktualisieren](../api/securescorecontrolprofiles-update.md)) festlegen.</span><span class="sxs-lookup"><span data-stu-id="54bbd-173">Tenant can set per control comments (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |
|   <span data-ttu-id="54bbd-174">assignedTo</span><span class="sxs-lookup"><span data-stu-id="54bbd-174">assignedTo</span></span> |    <span data-ttu-id="54bbd-175">String</span><span class="sxs-lookup"><span data-stu-id="54bbd-175">String</span></span>  |   <span data-ttu-id="54bbd-176">Mandanten kann das Steuerelement an eine Person (unterstützt [Aktualisieren](../api/securescorecontrolprofiles-update.md)) zuweisen.</span><span class="sxs-lookup"><span data-stu-id="54bbd-176">Tenant can assign the control to a individual (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |
|   <span data-ttu-id="54bbd-177">updatedBy</span><span class="sxs-lookup"><span data-stu-id="54bbd-177">updatedBy</span></span> | <span data-ttu-id="54bbd-178">String</span><span class="sxs-lookup"><span data-stu-id="54bbd-178">String</span></span>  |   <span data-ttu-id="54bbd-179">User principal Name des, die der Zustand eines Steuerelements geändert.</span><span class="sxs-lookup"><span data-stu-id="54bbd-179">User principal name of who made changes to a control's state.</span></span> |

## <a name="relationships"></a><span data-ttu-id="54bbd-180">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="54bbd-180">Relationships</span></span>

<span data-ttu-id="54bbd-181">Keine.</span><span class="sxs-lookup"><span data-stu-id="54bbd-181">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="54bbd-182">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="54bbd-182">JSON representation</span></span>

<span data-ttu-id="54bbd-183">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="54bbd-183">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScores"
}-->

```json
{
"title": "String", 
"azureTenantId": "Guid", 
"referenceId": "String", 
"controlName": "String", 
"maxScore": "Int32",
"actionCategory": "Collection(microsoft.graph.SecureScore.actionCategory)",
"actionType": "Collection(microsoft.graph.SecureScore.actionType)",
"service": "String",
"tier": "Collection(microsoft.graph.SecureScore.tier)",
"userImpact": "Collection(microsoft.graph.SecureScore.ranking)",
"implementationCost ": "Collection(microsoft.graph.SecureScore.ranking)",
"rank ": "Int32",
"threats": "Collection(microsoft.graph.SecureScore.threat)",
"deprecated ": "Boolean",
"remediation": "String",
"remediationImpact ": "String",
"actionUrl": "String",
"controlStateUpdates": "Collection(microsoft.graph.SecureScore.controlStateUpdates)",
"tenantNotes": "String",
"upn": "String",
"comments": "String",
}


```


<!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
