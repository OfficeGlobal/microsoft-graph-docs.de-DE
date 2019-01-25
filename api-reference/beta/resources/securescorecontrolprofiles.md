---
title: Ressourcentyp secureScoreControlProfiles
description: Stellt einen Mandanten sichere Faktor pro Steuerelementdaten. In der Standardeinstellung alle Steuerelemente für einen Mandanten zurückgegeben und einzelne Steuerelemente können explizit abrufen.
localization_priority: Normal
ms.openlocfilehash: 3e800271f1ef5f8ac7847d14d97ae6f24f1e01cf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524429"
---
# <a name="securescorecontrolprofiles-resource-type"></a><span data-ttu-id="e5e59-104">Ressourcentyp secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="e5e59-104">secureScoreControlProfiles resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5e59-105">Stellt einen Mandanten sichere Faktor pro Steuerelementdaten.</span><span class="sxs-lookup"><span data-stu-id="e5e59-105">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="e5e59-106">In der Standardeinstellung alle Steuerelemente für einen Mandanten zurückgegeben und einzelne Steuerelemente können explizit abrufen.</span><span class="sxs-lookup"><span data-stu-id="e5e59-106">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="e5e59-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="e5e59-107">Methods</span></span>

| <span data-ttu-id="e5e59-108">Methode</span><span class="sxs-lookup"><span data-stu-id="e5e59-108">Method</span></span>   | <span data-ttu-id="e5e59-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e5e59-109">Return Type</span></span>|<span data-ttu-id="e5e59-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e5e59-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e5e59-111">List secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="e5e59-111">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | [<span data-ttu-id="e5e59-112">secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="e5e59-112">secureScoreControlProfiles</span></span>](securescorecontrolprofiles.md) |<span data-ttu-id="e5e59-113">Lesen Sie Eigenschaften und Metadaten eines SecureScoreControlProfiles-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e5e59-113">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|


## <a name="properties"></a><span data-ttu-id="e5e59-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e5e59-114">Properties</span></span>

|<span data-ttu-id="e5e59-115">Name</span><span class="sxs-lookup"><span data-stu-id="e5e59-115">Name</span></span> |<span data-ttu-id="e5e59-116">Typ</span><span class="sxs-lookup"><span data-stu-id="e5e59-116">Type</span></span> |<span data-ttu-id="e5e59-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e5e59-117">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="e5e59-118">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="e5e59-118">azureTenantId</span></span>   |   <span data-ttu-id="e5e59-119">String</span><span class="sxs-lookup"><span data-stu-id="e5e59-119">String</span></span>  |   <span data-ttu-id="e5e59-120">GUID-Zeichenfolge für Mandanten-ID ein.</span><span class="sxs-lookup"><span data-stu-id="e5e59-120">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="e5e59-121">Steuerelementname</span><span class="sxs-lookup"><span data-stu-id="e5e59-121">controlName</span></span> |   <span data-ttu-id="e5e59-122">String</span><span class="sxs-lookup"><span data-stu-id="e5e59-122">String</span></span>  |   <span data-ttu-id="e5e59-123">Name des Steuerelements.</span><span class="sxs-lookup"><span data-stu-id="e5e59-123">Name of the control.</span></span> |
|   <span data-ttu-id="e5e59-124">title</span><span class="sxs-lookup"><span data-stu-id="e5e59-124">title</span></span>   |   <span data-ttu-id="e5e59-125">String</span><span class="sxs-lookup"><span data-stu-id="e5e59-125">String</span></span>  |   <span data-ttu-id="e5e59-126">Titel des Steuerelements.</span><span class="sxs-lookup"><span data-stu-id="e5e59-126">Title of the control.</span></span>   |
| <span data-ttu-id="e5e59-127">complianceInformation</span><span class="sxs-lookup"><span data-stu-id="e5e59-127">complianceInformation</span></span> | <span data-ttu-id="e5e59-128">[ComplianceInformation](complianceinformation.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="e5e59-128">[complianceInformation](complianceinformation.md) collection</span></span> | <span data-ttu-id="e5e59-129">Die Auflistung der Informationen im Zusammenhang mit Compliance secure Score-Steuerelement</span><span class="sxs-lookup"><span data-stu-id="e5e59-129">The collection of compliance information associated with secure score control</span></span> |
|   <span data-ttu-id="e5e59-130">controlCategory</span><span class="sxs-lookup"><span data-stu-id="e5e59-130">controlCategory</span></span> |   <span data-ttu-id="e5e59-131">String</span><span class="sxs-lookup"><span data-stu-id="e5e59-131">String</span></span>  |   <span data-ttu-id="e5e59-132">Steuerelement-Aktionskategorie (Konto, Daten, Gerät, Apps, Infrastruktur).</span><span class="sxs-lookup"><span data-stu-id="e5e59-132">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="e5e59-133">actionType</span><span class="sxs-lookup"><span data-stu-id="e5e59-133">actionType</span></span>  |   <span data-ttu-id="e5e59-134">String</span><span class="sxs-lookup"><span data-stu-id="e5e59-134">String</span></span>  |   <span data-ttu-id="e5e59-135">Steuerelementtyp Aktion (Config überprüfen, Verhalten).</span><span class="sxs-lookup"><span data-stu-id="e5e59-135">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="e5e59-136">service</span><span class="sxs-lookup"><span data-stu-id="e5e59-136">service</span></span> |   <span data-ttu-id="e5e59-137">String</span><span class="sxs-lookup"><span data-stu-id="e5e59-137">String</span></span>  |   <span data-ttu-id="e5e59-138">Dienst, der das Steuerelement (Exchange, Sharepoint, Azure AD) besitzt.</span><span class="sxs-lookup"><span data-stu-id="e5e59-138">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="e5e59-139">MaxErgebnis</span><span class="sxs-lookup"><span data-stu-id="e5e59-139">maxScore</span></span> |  <span data-ttu-id="e5e59-140">String</span><span class="sxs-lookup"><span data-stu-id="e5e59-140">String</span></span>  |   <span data-ttu-id="e5e59-141">Aktuelle abgerufen max Score am angegebenen Datum.</span><span class="sxs-lookup"><span data-stu-id="e5e59-141">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="e5e59-142">Ebene</span><span class="sxs-lookup"><span data-stu-id="e5e59-142">tier</span></span> |  <span data-ttu-id="e5e59-143">String</span><span class="sxs-lookup"><span data-stu-id="e5e59-143">String</span></span>  |   <span data-ttu-id="e5e59-144">Steuerelement-Tier (Quad-Core, mehrstufige im Detail, erweiterte.)</span><span class="sxs-lookup"><span data-stu-id="e5e59-144">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="e5e59-145">userImpact</span><span class="sxs-lookup"><span data-stu-id="e5e59-145">userImpact</span></span> |    <span data-ttu-id="e5e59-146">String</span><span class="sxs-lookup"><span data-stu-id="e5e59-146">String</span></span>  | <span data-ttu-id="e5e59-147">Beeinträchtigung für die Benutzer Implementieren von Steuerelement (niedrig, Mittel, hoch).</span><span class="sxs-lookup"><span data-stu-id="e5e59-147">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="e5e59-148">implementationCost</span><span class="sxs-lookup"><span data-stu-id="e5e59-148">implementationCost</span></span> |    <span data-ttu-id="e5e59-149">String</span><span class="sxs-lookup"><span data-stu-id="e5e59-149">String</span></span>  |   <span data-ttu-id="e5e59-150">Ressourcenkosten Implemmentating-Steuerelements (niedrig, Mittel, hoch).</span><span class="sxs-lookup"><span data-stu-id="e5e59-150">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="e5e59-151">rank</span><span class="sxs-lookup"><span data-stu-id="e5e59-151">rank</span></span> |  <span data-ttu-id="e5e59-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e5e59-152">Int32</span></span>   |   <span data-ttu-id="e5e59-153">Microsoft Stapel ranking des Steuerelements.</span><span class="sxs-lookup"><span data-stu-id="e5e59-153">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="e5e59-154">Bedrohungen</span><span class="sxs-lookup"><span data-stu-id="e5e59-154">threats</span></span> |   <span data-ttu-id="e5e59-155">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="e5e59-155">String Collection</span></span>   |   <span data-ttu-id="e5e59-156">Liste der Bedrohungen für das Steuerelement reduziert (AccountBreach, DataDeletion, DataExfiltration, DataSpillage, ElevationOfPrivilege, MaliciousInsider, PasswordCracking, PhishingOrWhaling, spoofing).</span><span class="sxs-lookup"><span data-stu-id="e5e59-156">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="e5e59-157">Veraltet</span><span class="sxs-lookup"><span data-stu-id="e5e59-157">deprecated</span></span> |    <span data-ttu-id="e5e59-158">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e5e59-158">Boolean</span></span> |   <span data-ttu-id="e5e59-159">Flag, das angibt, ob ein Steuerelement abgeschrieben wird.</span><span class="sxs-lookup"><span data-stu-id="e5e59-159">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="e5e59-160">Wartung</span><span class="sxs-lookup"><span data-stu-id="e5e59-160">remediation</span></span> |   <span data-ttu-id="e5e59-161">String</span><span class="sxs-lookup"><span data-stu-id="e5e59-161">String</span></span>  |   <span data-ttu-id="e5e59-162">Beschreibung, wie das Steuerelement helfen warten.</span><span class="sxs-lookup"><span data-stu-id="e5e59-162">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="e5e59-163">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="e5e59-163">remediationImpact</span></span> | <span data-ttu-id="e5e59-164">String</span><span class="sxs-lookup"><span data-stu-id="e5e59-164">String</span></span>  |   <span data-ttu-id="e5e59-165">Beschreibung der Auswirkung auf den Benutzer von der Wartung.</span><span class="sxs-lookup"><span data-stu-id="e5e59-165">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="e5e59-166">ActionUrl</span><span class="sxs-lookup"><span data-stu-id="e5e59-166">actionUrl</span></span> | <span data-ttu-id="e5e59-167">String</span><span class="sxs-lookup"><span data-stu-id="e5e59-167">String</span></span>  |   <span data-ttu-id="e5e59-168">URL zu, in dem das Steuerelement verarbeitet werden kann.</span><span class="sxs-lookup"><span data-stu-id="e5e59-168">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="e5e59-169">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="e5e59-169">controlStateUpdates</span></span> |   <span data-ttu-id="e5e59-170">[SecureScoreControlStateUpdate](securescorecontrolstateupdate.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="e5e59-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)   collection</span></span> |    <span data-ttu-id="e5e59-171">Kennzeichnung, die angibt, für der Mandanten ein Steuerelement markiert wurde (ignorieren, ThirdParty, überprüft) (unterstützt [Aktualisieren](../api/securescorecontrolprofiles-update.md)).</span><span class="sxs-lookup"><span data-stu-id="e5e59-171">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |

## <a name="relationships"></a><span data-ttu-id="e5e59-172">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e5e59-172">Relationships</span></span>

<span data-ttu-id="e5e59-173">Keine.</span><span class="sxs-lookup"><span data-stu-id="e5e59-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5e59-174">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e5e59-174">JSON representation</span></span>

<span data-ttu-id="e5e59-175">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e5e59-175">The following is a JSON representation of the resource.</span></span>

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


<!--
{
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/securescorecontrolprofiles.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
