---
title: VppToken aktualisieren
description: Aktualisieren der Eigenschaften eines vppToken-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 19541267f099afd03b5910b034234dbe34146e44
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978703"
---
# <a name="update-vpptoken"></a><span data-ttu-id="b9aeb-103">VppToken aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b9aeb-103">Update vppToken</span></span>

> <span data-ttu-id="b9aeb-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9aeb-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9aeb-106">Aktualisieren der Eigenschaften eines [vppToken](../resources/intune-onboarding-vpptoken.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-106">Update the properties of a [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9aeb-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b9aeb-107">Prerequisites</span></span>
<span data-ttu-id="b9aeb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9aeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9aeb-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b9aeb-110">Permission type</span></span>|<span data-ttu-id="b9aeb-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b9aeb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9aeb-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b9aeb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b9aeb-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9aeb-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b9aeb-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b9aeb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9aeb-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9aeb-115">Not supported.</span></span>|
|<span data-ttu-id="b9aeb-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b9aeb-116">Application</span></span>|<span data-ttu-id="b9aeb-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9aeb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9aeb-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9aeb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a><span data-ttu-id="b9aeb-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b9aeb-119">Request headers</span></span>
|<span data-ttu-id="b9aeb-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b9aeb-120">Header</span></span>|<span data-ttu-id="b9aeb-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b9aeb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9aeb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9aeb-122">Authorization</span></span>|<span data-ttu-id="b9aeb-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b9aeb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9aeb-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b9aeb-124">Accept</span></span>|<span data-ttu-id="b9aeb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b9aeb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9aeb-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b9aeb-126">Request body</span></span>
<span data-ttu-id="b9aeb-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [vppToken](../resources/intune-onboarding-vpptoken.md) an.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-127">In the request body, supply a JSON representation for the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

<span data-ttu-id="b9aeb-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [vppToken](../resources/intune-onboarding-vpptoken.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-128">The following table shows the properties that are required when you create the [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>

|<span data-ttu-id="b9aeb-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b9aeb-129">Property</span></span>|<span data-ttu-id="b9aeb-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b9aeb-130">Type</span></span>|<span data-ttu-id="b9aeb-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9aeb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9aeb-132">id</span><span class="sxs-lookup"><span data-stu-id="b9aeb-132">id</span></span>|<span data-ttu-id="b9aeb-133">String</span><span class="sxs-lookup"><span data-stu-id="b9aeb-133">String</span></span>|<span data-ttu-id="b9aeb-134">Dies wird automatisch generiert, wenn das appleVolumePurchaseProgramToken erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-134">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="b9aeb-135">Es ist der Schlüssel für die Entität.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-135">It is the Key of the entity.</span></span>|
|<span data-ttu-id="b9aeb-136">organizationName</span><span class="sxs-lookup"><span data-stu-id="b9aeb-136">organizationName</span></span>|<span data-ttu-id="b9aeb-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b9aeb-137">String</span></span>|<span data-ttu-id="b9aeb-138">Organisation, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="b9aeb-138">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="b9aeb-139">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="b9aeb-139">vppTokenAccountType</span></span>|[<span data-ttu-id="b9aeb-140">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="b9aeb-140">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="b9aeb-141">Volume Purchase Program-Typ, dem das angegebene Apple Volume Purchase Program-Token zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-141">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="b9aeb-142">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-142">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="b9aeb-143">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-143">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="b9aeb-144">appleId</span><span class="sxs-lookup"><span data-stu-id="b9aeb-144">appleId</span></span>|<span data-ttu-id="b9aeb-145">String</span><span class="sxs-lookup"><span data-stu-id="b9aeb-145">String</span></span>|<span data-ttu-id="b9aeb-146">Die Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-146">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="b9aeb-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b9aeb-147">expirationDateTime</span></span>|<span data-ttu-id="b9aeb-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9aeb-148">DateTimeOffset</span></span>|<span data-ttu-id="b9aeb-149">Ablaufdatum und -Uhrzeit des Apple Volume Purchase Program-Tokens</span><span class="sxs-lookup"><span data-stu-id="b9aeb-149">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="b9aeb-150">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b9aeb-150">lastSyncDateTime</span></span>|<span data-ttu-id="b9aeb-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9aeb-151">DateTimeOffset</span></span>|<span data-ttu-id="b9aeb-152">Der Zeitpunkt der letzten Anwendungssynchronisierung mit dem Apple Volume Purchase Program-Dienst mithilfe des Apple Volume Purchase Program-Tokens.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-152">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="b9aeb-153">token</span><span class="sxs-lookup"><span data-stu-id="b9aeb-153">token</span></span>|<span data-ttu-id="b9aeb-154">String</span><span class="sxs-lookup"><span data-stu-id="b9aeb-154">String</span></span>|<span data-ttu-id="b9aeb-155">Die Zeichenfolge des Apple Volume Purchase Program-Tokens, die vom Apple Volume Purchase Program heruntergeladen wurde.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-155">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="b9aeb-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9aeb-156">lastModifiedDateTime</span></span>|<span data-ttu-id="b9aeb-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9aeb-157">DateTimeOffset</span></span>|<span data-ttu-id="b9aeb-158">Datum und Uhrzeit der letzten Änderung, die dem Apple Volume Purchase Program-Token zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-158">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="b9aeb-159">state</span><span class="sxs-lookup"><span data-stu-id="b9aeb-159">state</span></span>|[<span data-ttu-id="b9aeb-160">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="b9aeb-160">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="b9aeb-161">Aktueller Status des Apple Volume Purchase Program-Tokens.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-161">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="b9aeb-162">Mögliche Werte: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-162">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="b9aeb-163">Mögliche Werte: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-163">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="b9aeb-164">tokenActionResults</span><span class="sxs-lookup"><span data-stu-id="b9aeb-164">tokenActionResults</span></span>|<span data-ttu-id="b9aeb-165">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="b9aeb-165">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) collection</span></span>|<span data-ttu-id="b9aeb-166">Die Sammlung von Status der Aktionen, die für das Apple Volume Purchase Program-Token ausgeführt wurden.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-166">The collection of statuses of the actions performed on the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="b9aeb-167">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="b9aeb-167">lastSyncStatus</span></span>|[<span data-ttu-id="b9aeb-168">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="b9aeb-168">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="b9aeb-169">Aktueller Synchronisierungsstatus der letzten Anwendungssynchronisierung, die mit dem Apple Volume Purchase Program-Token ausgelöst wurde.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-169">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="b9aeb-170">Mögliche Werte sind: `none`, `inProgress`, `completed` und `failed`.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-170">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="b9aeb-171">Mögliche Werte sind: `none`, `inProgress`, `completed` und `failed`.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-171">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="b9aeb-172">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="b9aeb-172">automaticallyUpdateApps</span></span>|<span data-ttu-id="b9aeb-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9aeb-173">Boolean</span></span>|<span data-ttu-id="b9aeb-174">Gibt an, ob Apps für das VPP-Token automatisch aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-174">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="b9aeb-175">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="b9aeb-175">countryOrRegion</span></span>|<span data-ttu-id="b9aeb-176">String</span><span class="sxs-lookup"><span data-stu-id="b9aeb-176">String</span></span>|<span data-ttu-id="b9aeb-177">Gibt an, ob Apps für das VPP-Token automatisch aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-177">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="b9aeb-178">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="b9aeb-178">dataSharingConsentGranted</span></span>|<span data-ttu-id="b9aeb-179">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9aeb-179">Boolean</span></span>|<span data-ttu-id="b9aeb-180">Einwilligung zur Datenfreigabe mit dem Apple Volume Purchase-Programm.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-180">Consent granted for data sharing with the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="b9aeb-181">displayName</span><span class="sxs-lookup"><span data-stu-id="b9aeb-181">displayName</span></span>|<span data-ttu-id="b9aeb-182">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b9aeb-182">String</span></span>|<span data-ttu-id="b9aeb-183">Ein vom Administrator angegebener, von Token angezeigter Name.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-183">An admin specified token friendly name.</span></span>|
|<span data-ttu-id="b9aeb-184">LocationName</span><span class="sxs-lookup"><span data-stu-id="b9aeb-184">locationName</span></span>|<span data-ttu-id="b9aeb-185">String</span><span class="sxs-lookup"><span data-stu-id="b9aeb-185">String</span></span>|<span data-ttu-id="b9aeb-186">Von Apple VSS zurückgegebener Tokensort.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-186">Token location returned from Apple VPP.</span></span>|
|<span data-ttu-id="b9aeb-187">claimTokenManagementFromExternalMdm</span><span class="sxs-lookup"><span data-stu-id="b9aeb-187">claimTokenManagementFromExternalMdm</span></span>|<span data-ttu-id="b9aeb-188">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b9aeb-188">Boolean</span></span>|<span data-ttu-id="b9aeb-189">Zustimmung des Administrators, um die Forderungs Tokenverwaltung über externes MDM zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-189">Admin consent to allow claiming token management from external MDM.</span></span>|
|<span data-ttu-id="b9aeb-190">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="b9aeb-190">roleScopeTagIds</span></span>|<span data-ttu-id="b9aeb-191">String collection</span><span class="sxs-lookup"><span data-stu-id="b9aeb-191">String collection</span></span>|<span data-ttu-id="b9aeb-192">Rollenbereichs Tags-IDs, die dieser Entität zugewiesen sind.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-192">Role Scope Tags IDs assigned to this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="b9aeb-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9aeb-193">Response</span></span>
<span data-ttu-id="b9aeb-194">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [vppToken](../resources/intune-onboarding-vpptoken.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-194">If successful, this method returns a `200 OK` response code and an updated [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9aeb-195">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b9aeb-195">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9aeb-196">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9aeb-196">Request</span></span>
<span data-ttu-id="b9aeb-197">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-197">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}
Content-type: application/json
Content-length: 1002

{
  "@odata.type": "#microsoft.graph.vppToken",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "state": "valid",
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value",
  "dataSharingConsentGranted": true,
  "displayName": "Display Name value",
  "locationName": "Location Name value",
  "claimTokenManagementFromExternalMdm": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="b9aeb-198">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9aeb-198">Response</span></span>
<span data-ttu-id="b9aeb-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b9aeb-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1115

{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "valid",
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value",
  "dataSharingConsentGranted": true,
  "displayName": "Display Name value",
  "locationName": "Location Name value",
  "claimTokenManagementFromExternalMdm": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




