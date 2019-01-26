---
title: Ressourcentyp secureScoreControlProfiles
description: Stellt einen Mandanten sichere Faktor pro Steuerelementdaten. In der Standardeinstellung alle Steuerelemente für einen Mandanten zurückgegeben und einzelne Steuerelemente können explizit abrufen.
localization_priority: Normal
ms.openlocfilehash: 4e599bbffd291de51ba478f8661999d01c8c8998
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576059"
---
# <a name="securescorecontrolprofiles-resource-type"></a><span data-ttu-id="17c18-104">Ressourcentyp secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="17c18-104">secureScoreControlProfiles resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17c18-105">Stellt einen Mandanten sichere Faktor pro Steuerelementdaten.</span><span class="sxs-lookup"><span data-stu-id="17c18-105">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="17c18-106">In der Standardeinstellung alle Steuerelemente für einen Mandanten zurückgegeben und einzelne Steuerelemente können explizit abrufen.</span><span class="sxs-lookup"><span data-stu-id="17c18-106">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="17c18-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="17c18-107">Methods</span></span>

| <span data-ttu-id="17c18-108">Methode</span><span class="sxs-lookup"><span data-stu-id="17c18-108">Method</span></span>   | <span data-ttu-id="17c18-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="17c18-109">Return Type</span></span>|<span data-ttu-id="17c18-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="17c18-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="17c18-111">List secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="17c18-111">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | [<span data-ttu-id="17c18-112">secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="17c18-112">secureScoreControlProfile</span></span>](securescorecontrolprofiles.md) |<span data-ttu-id="17c18-113">Lesen Sie Eigenschaften und Metadaten eines SecureScoreControlProfiles-Objekts.</span><span class="sxs-lookup"><span data-stu-id="17c18-113">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|


## <a name="properties"></a><span data-ttu-id="17c18-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="17c18-114">Properties</span></span>

|<span data-ttu-id="17c18-115">Name</span><span class="sxs-lookup"><span data-stu-id="17c18-115">Name</span></span> |<span data-ttu-id="17c18-116">Typ</span><span class="sxs-lookup"><span data-stu-id="17c18-116">Type</span></span> |<span data-ttu-id="17c18-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="17c18-117">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="17c18-118">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="17c18-118">azureTenantId</span></span>   |   <span data-ttu-id="17c18-119">String</span><span class="sxs-lookup"><span data-stu-id="17c18-119">String</span></span>  |   <span data-ttu-id="17c18-120">GUID-Zeichenfolge für Mandanten-ID ein.</span><span class="sxs-lookup"><span data-stu-id="17c18-120">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="17c18-121">Steuerelementname</span><span class="sxs-lookup"><span data-stu-id="17c18-121">controlName</span></span> |   <span data-ttu-id="17c18-122">String</span><span class="sxs-lookup"><span data-stu-id="17c18-122">String</span></span>  |   <span data-ttu-id="17c18-123">Name des Steuerelements.</span><span class="sxs-lookup"><span data-stu-id="17c18-123">Name of the control.</span></span> |
|   <span data-ttu-id="17c18-124">title</span><span class="sxs-lookup"><span data-stu-id="17c18-124">title</span></span>   |   <span data-ttu-id="17c18-125">String</span><span class="sxs-lookup"><span data-stu-id="17c18-125">String</span></span>  |   <span data-ttu-id="17c18-126">Titel des Steuerelements.</span><span class="sxs-lookup"><span data-stu-id="17c18-126">Title of the control.</span></span>   |
|   <span data-ttu-id="17c18-127">controlCategory</span><span class="sxs-lookup"><span data-stu-id="17c18-127">controlCategory</span></span> |   <span data-ttu-id="17c18-128">String</span><span class="sxs-lookup"><span data-stu-id="17c18-128">String</span></span>  |   <span data-ttu-id="17c18-129">Steuerelement-Aktionskategorie (Konto, Daten, Gerät, Apps, Infrastruktur).</span><span class="sxs-lookup"><span data-stu-id="17c18-129">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="17c18-130">actionType</span><span class="sxs-lookup"><span data-stu-id="17c18-130">actionType</span></span>  |   <span data-ttu-id="17c18-131">String</span><span class="sxs-lookup"><span data-stu-id="17c18-131">String</span></span>  |   <span data-ttu-id="17c18-132">Steuerelementtyp Aktion (Config überprüfen, Verhalten).</span><span class="sxs-lookup"><span data-stu-id="17c18-132">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="17c18-133">service</span><span class="sxs-lookup"><span data-stu-id="17c18-133">service</span></span> |   <span data-ttu-id="17c18-134">String</span><span class="sxs-lookup"><span data-stu-id="17c18-134">String</span></span>  |   <span data-ttu-id="17c18-135">Dienst, der das Steuerelement (Exchange, Sharepoint, Azure AD) besitzt.</span><span class="sxs-lookup"><span data-stu-id="17c18-135">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="17c18-136">MaxErgebnis</span><span class="sxs-lookup"><span data-stu-id="17c18-136">maxScore</span></span> |  <span data-ttu-id="17c18-137">Gleitkommawert mit doppelter Genauigkeit</span><span class="sxs-lookup"><span data-stu-id="17c18-137">Double</span></span>  |   <span data-ttu-id="17c18-138">Aktuelle abgerufen max Score am angegebenen Datum.</span><span class="sxs-lookup"><span data-stu-id="17c18-138">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="17c18-139">Tier</span><span class="sxs-lookup"><span data-stu-id="17c18-139">tier</span></span> |  <span data-ttu-id="17c18-140">String</span><span class="sxs-lookup"><span data-stu-id="17c18-140">String</span></span>  |   <span data-ttu-id="17c18-141">Steuerelement-Tier (Quad-Core, mehrstufige im Detail, erweiterte.)</span><span class="sxs-lookup"><span data-stu-id="17c18-141">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="17c18-142">userImpact</span><span class="sxs-lookup"><span data-stu-id="17c18-142">userImpact</span></span> |    <span data-ttu-id="17c18-143">String</span><span class="sxs-lookup"><span data-stu-id="17c18-143">String</span></span>  | <span data-ttu-id="17c18-144">Beeinträchtigung für die Benutzer Implementieren von Steuerelement (niedrig, Mittel, hoch).</span><span class="sxs-lookup"><span data-stu-id="17c18-144">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="17c18-145">implementationCost</span><span class="sxs-lookup"><span data-stu-id="17c18-145">implementationCost</span></span> |    <span data-ttu-id="17c18-146">String</span><span class="sxs-lookup"><span data-stu-id="17c18-146">String</span></span>  |   <span data-ttu-id="17c18-147">Ressourcenkosten Implemmentating-Steuerelements (niedrig, Mittel, hoch).</span><span class="sxs-lookup"><span data-stu-id="17c18-147">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="17c18-148">rank</span><span class="sxs-lookup"><span data-stu-id="17c18-148">rank</span></span> |  <span data-ttu-id="17c18-149">Int32</span><span class="sxs-lookup"><span data-stu-id="17c18-149">Int32</span></span>   |   <span data-ttu-id="17c18-150">Microsoft Stapel ranking des Steuerelements.</span><span class="sxs-lookup"><span data-stu-id="17c18-150">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="17c18-151">Bedrohungen</span><span class="sxs-lookup"><span data-stu-id="17c18-151">threats</span></span> |   <span data-ttu-id="17c18-152">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="17c18-152">String Collection</span></span>   |   <span data-ttu-id="17c18-153">Liste der Bedrohungen für das Steuerelement reduziert (AccountBreach, DataDeletion, DataExfiltration, DataSpillage, ElevationOfPrivilege, MaliciousInsider, PasswordCracking, PhishingOrWhaling, spoofing).</span><span class="sxs-lookup"><span data-stu-id="17c18-153">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="17c18-154">veraltet</span><span class="sxs-lookup"><span data-stu-id="17c18-154">deprecated</span></span> |    <span data-ttu-id="17c18-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="17c18-155">Boolean</span></span> |   <span data-ttu-id="17c18-156">Flag, das angibt, ob ein Steuerelement abgeschrieben wird.</span><span class="sxs-lookup"><span data-stu-id="17c18-156">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="17c18-157">Wartung</span><span class="sxs-lookup"><span data-stu-id="17c18-157">remediation</span></span> |   <span data-ttu-id="17c18-158">String</span><span class="sxs-lookup"><span data-stu-id="17c18-158">String</span></span>  |   <span data-ttu-id="17c18-159">Beschreibung, wie das Steuerelement helfen warten.</span><span class="sxs-lookup"><span data-stu-id="17c18-159">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="17c18-160">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="17c18-160">remediationImpact</span></span> | <span data-ttu-id="17c18-161">String</span><span class="sxs-lookup"><span data-stu-id="17c18-161">String</span></span>  |   <span data-ttu-id="17c18-162">Beschreibung der Auswirkung auf den Benutzer von der Wartung.</span><span class="sxs-lookup"><span data-stu-id="17c18-162">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="17c18-163">actionUrl</span><span class="sxs-lookup"><span data-stu-id="17c18-163">actionUrl</span></span> | <span data-ttu-id="17c18-164">String</span><span class="sxs-lookup"><span data-stu-id="17c18-164">String</span></span>  |   <span data-ttu-id="17c18-165">URL zu, in dem das Steuerelement verarbeitet werden kann.</span><span class="sxs-lookup"><span data-stu-id="17c18-165">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="17c18-166">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="17c18-166">lastModifiedDateTime</span></span> |  <span data-ttu-id="17c18-167">Zeichenfolge (DateTimeOffset)</span><span class="sxs-lookup"><span data-stu-id="17c18-167">String (DateTimeOffset)</span></span> |   <span data-ttu-id="17c18-168">Datum der letzten Änderung</span><span class="sxs-lookup"><span data-stu-id="17c18-168">Date last modified</span></span> |
|   <span data-ttu-id="17c18-169">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="17c18-169">controlStateUpdates</span></span> |   <span data-ttu-id="17c18-170">[SecureScoreControlStateUpdate](securescorecontrolstateupdate.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="17c18-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) collection</span></span> |  <span data-ttu-id="17c18-171">Kennzeichnung, die angibt, für der Mandanten ein Steuerelement markiert wurde (ignorieren, ThirdParty, überprüft) (unterstützt [Aktualisieren](../api/securescorecontrolprofiles-update.md)).</span><span class="sxs-lookup"><span data-stu-id="17c18-171">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |
|   <span data-ttu-id="17c18-172">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="17c18-172">vendorInformation</span></span> | [<span data-ttu-id="17c18-173">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="17c18-173">securityVendorInformation</span></span>](securityvendorinformation.md) | <span data-ttu-id="17c18-174">Enthält Details über die Produkt-Dienst Sicherheitsanbieter, Anbieter und Subprovider (beispielsweise Hersteller = Microsoft; Provider = Windows Defender ATP; SubProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="17c18-174">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>|

## <a name="relationships"></a><span data-ttu-id="17c18-175">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="17c18-175">Relationships</span></span>

<span data-ttu-id="17c18-176">Keine.</span><span class="sxs-lookup"><span data-stu-id="17c18-176">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="17c18-177">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="17c18-177">JSON representation</span></span>

<span data-ttu-id="17c18-178">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="17c18-178">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
}-->

```json
{
    "title": "String", 
    "azureTenantId": "String (identifier)", 
    "referenceId": "String", 
    "controlName": "String", 
    "maxScore": "Double",
    "controlCategory": "string",
    "actionType": "string",
    "service": "String",
    "tier": "string",
    "userImpact": "string",
    "implementationCost ": "string",
    "rank ": "Int32",
    "deprecated ": "Boolean",
    "remediation": "String",
    "remediationImpact ": "String",
    "actionUrl": "String",
    "lastModifiedDateTime": "   String (DateTimeOffset)",
    "controlStateUpdates": [{"odata.type":"microsoft.graph.secureScorecontrolStateUpdates"}],
    "tenantNotes": "String",
    "upn": "String",    
    "vendorInformation" : "microsoft.graph.securityVendorInformation"
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
