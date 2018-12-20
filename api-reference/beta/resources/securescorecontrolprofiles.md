---
title: Ressourcentyp secureScoreControlProfiles
description: Stellt einen Mandanten sichere Faktor pro Steuerelementdaten. In der Standardeinstellung alle Steuerelemente für einen Mandanten zurückgegeben und einzelne Steuerelemente können explizit abrufen.
ms.openlocfilehash: 3e7dc463d7521e1980b41034ae4121ab610dd8f5
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380583"
---
# <a name="securescorecontrolprofiles-resource-type"></a><span data-ttu-id="6c672-104">Ressourcentyp secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="6c672-104">secureScoreControlProfiles resource type</span></span>

> <span data-ttu-id="6c672-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6c672-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c672-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6c672-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6c672-107">Stellt einen Mandanten sichere Faktor pro Steuerelementdaten.</span><span class="sxs-lookup"><span data-stu-id="6c672-107">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="6c672-108">In der Standardeinstellung alle Steuerelemente für einen Mandanten zurückgegeben und einzelne Steuerelemente können explizit abrufen.</span><span class="sxs-lookup"><span data-stu-id="6c672-108">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="6c672-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="6c672-109">Methods</span></span>

| <span data-ttu-id="6c672-110">Methode</span><span class="sxs-lookup"><span data-stu-id="6c672-110">Method</span></span>   | <span data-ttu-id="6c672-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="6c672-111">Return Type</span></span>|<span data-ttu-id="6c672-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6c672-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6c672-113">List secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="6c672-113">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | [<span data-ttu-id="6c672-114">secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="6c672-114">secureScoreControlProfiles</span></span>](securescorecontrolprofiles.md) |<span data-ttu-id="6c672-115">Lesen Sie Eigenschaften und Metadaten eines SecureScoreControlProfiles-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6c672-115">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|


## <a name="properties"></a><span data-ttu-id="6c672-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6c672-116">Properties</span></span>

|<span data-ttu-id="6c672-117">Name</span><span class="sxs-lookup"><span data-stu-id="6c672-117">Name</span></span> |<span data-ttu-id="6c672-118">Typ</span><span class="sxs-lookup"><span data-stu-id="6c672-118">Type</span></span> |<span data-ttu-id="6c672-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6c672-119">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="6c672-120">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="6c672-120">azureTenantId</span></span>   |   <span data-ttu-id="6c672-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6c672-121">String</span></span>  |   <span data-ttu-id="6c672-122">GUID-Zeichenfolge für Mandanten-ID ein.</span><span class="sxs-lookup"><span data-stu-id="6c672-122">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="6c672-123">Steuerelementname</span><span class="sxs-lookup"><span data-stu-id="6c672-123">controlName</span></span> |   <span data-ttu-id="6c672-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6c672-124">String</span></span>  |   <span data-ttu-id="6c672-125">Name des Steuerelements.</span><span class="sxs-lookup"><span data-stu-id="6c672-125">Name of the control.</span></span> |
|   <span data-ttu-id="6c672-126">title</span><span class="sxs-lookup"><span data-stu-id="6c672-126">title</span></span>   |   <span data-ttu-id="6c672-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6c672-127">String</span></span>  |   <span data-ttu-id="6c672-128">Titel des Steuerelements.</span><span class="sxs-lookup"><span data-stu-id="6c672-128">Title of the control.</span></span>   |
| <span data-ttu-id="6c672-129">complianceInformation</span><span class="sxs-lookup"><span data-stu-id="6c672-129">complianceInformation</span></span> | <span data-ttu-id="6c672-130">[ComplianceInformation](complianceinformation.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6c672-130">[complianceInformation](complianceinformation.md) collection</span></span> | <span data-ttu-id="6c672-131">Die Auflistung der Informationen im Zusammenhang mit Compliance secure Score-Steuerelement</span><span class="sxs-lookup"><span data-stu-id="6c672-131">The collection of compliance information associated with secure score control</span></span> |
|   <span data-ttu-id="6c672-132">controlCategory</span><span class="sxs-lookup"><span data-stu-id="6c672-132">controlCategory</span></span> |   <span data-ttu-id="6c672-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6c672-133">String</span></span>  |   <span data-ttu-id="6c672-134">Steuerelement-Aktionskategorie (Konto, Daten, Gerät, Apps, Infrastruktur).</span><span class="sxs-lookup"><span data-stu-id="6c672-134">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="6c672-135">actionType</span><span class="sxs-lookup"><span data-stu-id="6c672-135">actionType</span></span>  |   <span data-ttu-id="6c672-136">String</span><span class="sxs-lookup"><span data-stu-id="6c672-136">String</span></span>  |   <span data-ttu-id="6c672-137">Steuerelementtyp Aktion (Config überprüfen, Verhalten).</span><span class="sxs-lookup"><span data-stu-id="6c672-137">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="6c672-138">service</span><span class="sxs-lookup"><span data-stu-id="6c672-138">service</span></span> |   <span data-ttu-id="6c672-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6c672-139">String</span></span>  |   <span data-ttu-id="6c672-140">Dienst, der das Steuerelement (Exchange, Sharepoint, Azure AD) besitzt.</span><span class="sxs-lookup"><span data-stu-id="6c672-140">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="6c672-141">MaxErgebnis</span><span class="sxs-lookup"><span data-stu-id="6c672-141">maxScore</span></span> |  <span data-ttu-id="6c672-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6c672-142">String</span></span>  |   <span data-ttu-id="6c672-143">Aktuelle abgerufen max Score am angegebenen Datum.</span><span class="sxs-lookup"><span data-stu-id="6c672-143">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="6c672-144">Tier</span><span class="sxs-lookup"><span data-stu-id="6c672-144">tier</span></span> |  <span data-ttu-id="6c672-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6c672-145">String</span></span>  |   <span data-ttu-id="6c672-146">Steuerelement-Tier (Quad-Core, mehrstufige im Detail, erweiterte.)</span><span class="sxs-lookup"><span data-stu-id="6c672-146">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="6c672-147">userImpact</span><span class="sxs-lookup"><span data-stu-id="6c672-147">userImpact</span></span> |    <span data-ttu-id="6c672-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6c672-148">String</span></span>  | <span data-ttu-id="6c672-149">Beeinträchtigung für die Benutzer Implementieren von Steuerelement (niedrig, Mittel, hoch).</span><span class="sxs-lookup"><span data-stu-id="6c672-149">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="6c672-150">implementationCost</span><span class="sxs-lookup"><span data-stu-id="6c672-150">implementationCost</span></span> |    <span data-ttu-id="6c672-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6c672-151">String</span></span>  |   <span data-ttu-id="6c672-152">Ressourcenkosten Implemmentating-Steuerelements (niedrig, Mittel, hoch).</span><span class="sxs-lookup"><span data-stu-id="6c672-152">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="6c672-153">rank</span><span class="sxs-lookup"><span data-stu-id="6c672-153">rank</span></span> |  <span data-ttu-id="6c672-154">Int32</span><span class="sxs-lookup"><span data-stu-id="6c672-154">Int32</span></span>   |   <span data-ttu-id="6c672-155">Microsoft Stapel ranking des Steuerelements.</span><span class="sxs-lookup"><span data-stu-id="6c672-155">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="6c672-156">Bedrohungen</span><span class="sxs-lookup"><span data-stu-id="6c672-156">threats</span></span> |   <span data-ttu-id="6c672-157">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="6c672-157">String Collection</span></span>   |   <span data-ttu-id="6c672-158">Liste der Bedrohungen für das Steuerelement reduziert (AccountBreach, DataDeletion, DataExfiltration, DataSpillage, ElevationOfPrivilege, MaliciousInsider, PasswordCracking, PhishingOrWhaling, spoofing).</span><span class="sxs-lookup"><span data-stu-id="6c672-158">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="6c672-159">veraltet</span><span class="sxs-lookup"><span data-stu-id="6c672-159">deprecated</span></span> |    <span data-ttu-id="6c672-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6c672-160">Boolean</span></span> |   <span data-ttu-id="6c672-161">Flag, das angibt, ob ein Steuerelement abgeschrieben wird.</span><span class="sxs-lookup"><span data-stu-id="6c672-161">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="6c672-162">Wartung</span><span class="sxs-lookup"><span data-stu-id="6c672-162">remediation</span></span> |   <span data-ttu-id="6c672-163">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6c672-163">String</span></span>  |   <span data-ttu-id="6c672-164">Beschreibung, wie das Steuerelement helfen warten.</span><span class="sxs-lookup"><span data-stu-id="6c672-164">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="6c672-165">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="6c672-165">remediationImpact</span></span> | <span data-ttu-id="6c672-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6c672-166">String</span></span>  |   <span data-ttu-id="6c672-167">Beschreibung der Auswirkung auf den Benutzer von der Wartung.</span><span class="sxs-lookup"><span data-stu-id="6c672-167">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="6c672-168">actionUrl</span><span class="sxs-lookup"><span data-stu-id="6c672-168">actionUrl</span></span> | <span data-ttu-id="6c672-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6c672-169">String</span></span>  |   <span data-ttu-id="6c672-170">URL zu, in dem das Steuerelement verarbeitet werden kann.</span><span class="sxs-lookup"><span data-stu-id="6c672-170">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="6c672-171">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="6c672-171">controlStateUpdates</span></span> |   <span data-ttu-id="6c672-172">[SecureScoreControlStateUpdate](securescorecontrolstateupdate.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6c672-172">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)   collection</span></span> |    <span data-ttu-id="6c672-173">Kennzeichnung, die angibt, für der Mandanten ein Steuerelement markiert wurde (ignorieren, ThirdParty, überprüft) (unterstützt [Aktualisieren](../api/securescorecontrolprofiles-update.md)).</span><span class="sxs-lookup"><span data-stu-id="6c672-173">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |

## <a name="relationships"></a><span data-ttu-id="6c672-174">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6c672-174">Relationships</span></span>

<span data-ttu-id="6c672-175">Keine.</span><span class="sxs-lookup"><span data-stu-id="6c672-175">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c672-176">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6c672-176">JSON representation</span></span>

<span data-ttu-id="6c672-177">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6c672-177">The following is a JSON representation of the resource.</span></span>

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
