---
title: VppToken aktualisieren
description: Aktualisieren der Eigenschaften eines vppToken-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d1e38660c1fa83ced205b0bbcc506303a3968c41
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954148"
---
# <a name="update-vpptoken"></a><span data-ttu-id="a6c0e-103">VppToken aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a6c0e-103">Update vppToken</span></span>

> <span data-ttu-id="a6c0e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6c0e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a6c0e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6c0e-107">Aktualisieren der Eigenschaften eines [vppToken](../resources/intune-onboarding-vpptoken.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-107">Update the properties of a [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a6c0e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a6c0e-108">Prerequisites</span></span>
<span data-ttu-id="a6c0e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6c0e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6c0e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a6c0e-111">Permission type</span></span>|<span data-ttu-id="a6c0e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a6c0e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6c0e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a6c0e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6c0e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6c0e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a6c0e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a6c0e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6c0e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a6c0e-116">Not supported.</span></span>|
|<span data-ttu-id="a6c0e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a6c0e-117">Application</span></span>|<span data-ttu-id="a6c0e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a6c0e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6c0e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a6c0e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a><span data-ttu-id="a6c0e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a6c0e-120">Request headers</span></span>
|<span data-ttu-id="a6c0e-121">Header</span><span class="sxs-lookup"><span data-stu-id="a6c0e-121">Header</span></span>|<span data-ttu-id="a6c0e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a6c0e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6c0e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6c0e-123">Authorization</span></span>|<span data-ttu-id="a6c0e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a6c0e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6c0e-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a6c0e-125">Accept</span></span>|<span data-ttu-id="a6c0e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6c0e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6c0e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a6c0e-127">Request body</span></span>
<span data-ttu-id="a6c0e-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [vppToken](../resources/intune-onboarding-vpptoken.md) an.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-128">In the request body, supply a JSON representation for the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

<span data-ttu-id="a6c0e-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [vppToken](../resources/intune-onboarding-vpptoken.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-129">The following table shows the properties that are required when you create the [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>

|<span data-ttu-id="a6c0e-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a6c0e-130">Property</span></span>|<span data-ttu-id="a6c0e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="a6c0e-131">Type</span></span>|<span data-ttu-id="a6c0e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a6c0e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6c0e-133">id</span><span class="sxs-lookup"><span data-stu-id="a6c0e-133">id</span></span>|<span data-ttu-id="a6c0e-134">String</span><span class="sxs-lookup"><span data-stu-id="a6c0e-134">String</span></span>|<span data-ttu-id="a6c0e-135">Wird automatisch generiert, wenn AppleVolumePurchaseProgramToken erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-135">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="a6c0e-136">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-136">It is the Key of the entity.</span></span>|
|<span data-ttu-id="a6c0e-137">organizationName</span><span class="sxs-lookup"><span data-stu-id="a6c0e-137">organizationName</span></span>|<span data-ttu-id="a6c0e-138">String</span><span class="sxs-lookup"><span data-stu-id="a6c0e-138">String</span></span>|<span data-ttu-id="a6c0e-139">Organisation, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="a6c0e-139">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="a6c0e-140">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="a6c0e-140">vppTokenAccountType</span></span>|[<span data-ttu-id="a6c0e-141">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="a6c0e-141">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="a6c0e-142">Volume Purchase Program-Typ, dem das angegebene Apple Volume Purchase Program-Token zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-142">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="a6c0e-143">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-143">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="a6c0e-144">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-144">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="a6c0e-145">appleId</span><span class="sxs-lookup"><span data-stu-id="a6c0e-145">appleId</span></span>|<span data-ttu-id="a6c0e-146">String</span><span class="sxs-lookup"><span data-stu-id="a6c0e-146">String</span></span>|<span data-ttu-id="a6c0e-147">Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-147">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="a6c0e-148">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a6c0e-148">expirationDateTime</span></span>|<span data-ttu-id="a6c0e-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6c0e-149">DateTimeOffset</span></span>|<span data-ttu-id="a6c0e-150">Ablaufdatum und -uhrzeit des Apple Volume Purchase Program-Token.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-150">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="a6c0e-151">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a6c0e-151">lastSyncDateTime</span></span>|<span data-ttu-id="a6c0e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6c0e-152">DateTimeOffset</span></span>|<span data-ttu-id="a6c0e-153">Zeitpunkt der letzten Synchronisierung der Anwendung mit dem Apple Volume Purchase Program Service mithilfe des Apple Volume Purchase Program-Token.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-153">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="a6c0e-154">token</span><span class="sxs-lookup"><span data-stu-id="a6c0e-154">token</span></span>|<span data-ttu-id="a6c0e-155">String</span><span class="sxs-lookup"><span data-stu-id="a6c0e-155">String</span></span>|<span data-ttu-id="a6c0e-156">Aus dem Apple Volume Purchase Program heruntergeladene Zeichenfolge des Apple Volume Purchase Program-Token.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-156">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="a6c0e-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a6c0e-157">lastModifiedDateTime</span></span>|<span data-ttu-id="a6c0e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6c0e-158">DateTimeOffset</span></span>|<span data-ttu-id="a6c0e-159">Letztes Änderungsdatum und letzter Änderungszeitpunkt des Apple Volume Purchase Program-Token.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-159">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="a6c0e-160">state</span><span class="sxs-lookup"><span data-stu-id="a6c0e-160">state</span></span>|[<span data-ttu-id="a6c0e-161">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="a6c0e-161">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="a6c0e-162">Aktueller Stand des Apple Volume Purchase Program-Token.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-162">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="a6c0e-163">Mögliche Werte sind: `unknown`, `valid`, `expired`, `invalid` und `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-163">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="a6c0e-164">Mögliche Werte sind: `unknown`, `valid`, `expired`, `invalid` und `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-164">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="a6c0e-165">tokenActionResults</span><span class="sxs-lookup"><span data-stu-id="a6c0e-165">tokenActionResults</span></span>|<span data-ttu-id="a6c0e-166">[VppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="a6c0e-166">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) collection</span></span>|<span data-ttu-id="a6c0e-167">Die Auflistung der Status der Aktionen, die auf Apple Volume Purchase Programm Token ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-167">The collection of statuses of the actions performed on the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="a6c0e-168">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="a6c0e-168">lastSyncStatus</span></span>|[<span data-ttu-id="a6c0e-169">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="a6c0e-169">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="a6c0e-170">Aktueller Synchronisierungsstatus seit der letzten Synchronisierung der Anwendung, die mit dem Apple Volume Purchase Program-Token durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-170">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="a6c0e-171">Mögliche Werte sind: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-171">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="a6c0e-172">Mögliche Werte sind: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-172">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="a6c0e-173">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="a6c0e-173">automaticallyUpdateApps</span></span>|<span data-ttu-id="a6c0e-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6c0e-174">Boolean</span></span>|<span data-ttu-id="a6c0e-175">Angabe, ob Anwendungen für das VPP-Token automatisch aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-175">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="a6c0e-176">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="a6c0e-176">countryOrRegion</span></span>|<span data-ttu-id="a6c0e-177">String</span><span class="sxs-lookup"><span data-stu-id="a6c0e-177">String</span></span>|<span data-ttu-id="a6c0e-178">Angabe, ob Anwendungen für das VPP-Token automatisch aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-178">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="a6c0e-179">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="a6c0e-179">dataSharingConsentGranted</span></span>|<span data-ttu-id="a6c0e-180">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a6c0e-180">Boolean</span></span>|<span data-ttu-id="a6c0e-181">Stimmen Sie für Datenfreigaben über die Apple Volume Purchase Program gewährt.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-181">Consent granted for data sharing with the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="a6c0e-182">displayName</span><span class="sxs-lookup"><span data-stu-id="a6c0e-182">displayName</span></span>|<span data-ttu-id="a6c0e-183">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a6c0e-183">String</span></span>|<span data-ttu-id="a6c0e-184">Ein Administrator angegebene token Anzeigenamen.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-184">An admin specified token friendly name.</span></span>|
|<span data-ttu-id="a6c0e-185">locationName</span><span class="sxs-lookup"><span data-stu-id="a6c0e-185">locationName</span></span>|<span data-ttu-id="a6c0e-186">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a6c0e-186">String</span></span>|<span data-ttu-id="a6c0e-187">Token Speicherort von Apple VPP zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-187">Token location returned from Apple VPP.</span></span>|
|<span data-ttu-id="a6c0e-188">claimTokenManagementFromExternalMdm</span><span class="sxs-lookup"><span data-stu-id="a6c0e-188">claimTokenManagementFromExternalMdm</span></span>|<span data-ttu-id="a6c0e-189">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a6c0e-189">Boolean</span></span>|<span data-ttu-id="a6c0e-190">Admin stimmen ausgibt token Management von externen MDM zulassen</span><span class="sxs-lookup"><span data-stu-id="a6c0e-190">Admin consent to allow claiming token management from external MDM.</span></span>|



## <a name="response"></a><span data-ttu-id="a6c0e-191">Antwort</span><span class="sxs-lookup"><span data-stu-id="a6c0e-191">Response</span></span>
<span data-ttu-id="a6c0e-192">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [vppToken](../resources/intune-onboarding-vpptoken.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-192">If successful, this method returns a `200 OK` response code and an updated [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6c0e-193">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a6c0e-193">Example</span></span>
### <a name="request"></a><span data-ttu-id="a6c0e-194">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a6c0e-194">Request</span></span>
<span data-ttu-id="a6c0e-195">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-195">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}
Content-type: application/json
Content-length: 957

{
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
  "claimTokenManagementFromExternalMdm": true
}
```

### <a name="response"></a><span data-ttu-id="a6c0e-196">Antwort</span><span class="sxs-lookup"><span data-stu-id="a6c0e-196">Response</span></span>
<span data-ttu-id="a6c0e-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a6c0e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1053

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
  "claimTokenManagementFromExternalMdm": true
}
```





