---
title: VppToken erstellen
description: Erstellen Sie ein neues VppToken-Objekt.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 48b232098ea108f9dc02a47628a8ad9c8f413a00
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810003"
---
# <a name="create-vpptoken"></a><span data-ttu-id="8c62c-103">VppToken erstellen</span><span class="sxs-lookup"><span data-stu-id="8c62c-103">Create vppToken</span></span>

> <span data-ttu-id="8c62c-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8c62c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c62c-105">Erstellen Sie ein neues [VppToken](../resources/intune-onboarding-vpptoken.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="8c62c-105">Create a new [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8c62c-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8c62c-106">Prerequisites</span></span>
<span data-ttu-id="8c62c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c62c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c62c-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8c62c-109">Permission type</span></span>|<span data-ttu-id="8c62c-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8c62c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c62c-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8c62c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8c62c-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c62c-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8c62c-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8c62c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c62c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8c62c-114">Not supported.</span></span>|
|<span data-ttu-id="8c62c-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8c62c-115">Application</span></span>|<span data-ttu-id="8c62c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8c62c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c62c-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c62c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="8c62c-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8c62c-118">Request headers</span></span>
|<span data-ttu-id="8c62c-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8c62c-119">Header</span></span>|<span data-ttu-id="8c62c-120">Wert</span><span class="sxs-lookup"><span data-stu-id="8c62c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c62c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c62c-121">Authorization</span></span>|<span data-ttu-id="8c62c-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8c62c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c62c-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8c62c-123">Accept</span></span>|<span data-ttu-id="8c62c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8c62c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c62c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8c62c-125">Request body</span></span>
<span data-ttu-id="8c62c-126">Geben Sie im Anforderungstext eine JSON-Darstellung des vppToken-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="8c62c-126">In the request body, supply a JSON representation for the vppToken object.</span></span>

<span data-ttu-id="8c62c-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des vppToken erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8c62c-127">The following table shows the properties that are required when you create the vppToken.</span></span>

|<span data-ttu-id="8c62c-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8c62c-128">Property</span></span>|<span data-ttu-id="8c62c-129">Typ</span><span class="sxs-lookup"><span data-stu-id="8c62c-129">Type</span></span>|<span data-ttu-id="8c62c-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8c62c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c62c-131">id</span><span class="sxs-lookup"><span data-stu-id="8c62c-131">id</span></span>|<span data-ttu-id="8c62c-132">String</span><span class="sxs-lookup"><span data-stu-id="8c62c-132">String</span></span>|<span data-ttu-id="8c62c-133">Wird automatisch generiert, wenn AppleVolumePurchaseProgramToken erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="8c62c-133">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="8c62c-134">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="8c62c-134">It is the Key of the entity.</span></span>|
|<span data-ttu-id="8c62c-135">organizationName</span><span class="sxs-lookup"><span data-stu-id="8c62c-135">organizationName</span></span>|<span data-ttu-id="8c62c-136">String</span><span class="sxs-lookup"><span data-stu-id="8c62c-136">String</span></span>|<span data-ttu-id="8c62c-137">Organisation, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="8c62c-137">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="8c62c-138">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="8c62c-138">vppTokenAccountType</span></span>|[<span data-ttu-id="8c62c-139">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="8c62c-139">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="8c62c-140">Volume Purchase Program-Typ, dem das angegebene Apple Volume Purchase Program-Token zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="8c62c-140">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="8c62c-141">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="8c62c-141">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="8c62c-142">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="8c62c-142">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="8c62c-143">appleId</span><span class="sxs-lookup"><span data-stu-id="8c62c-143">appleId</span></span>|<span data-ttu-id="8c62c-144">String</span><span class="sxs-lookup"><span data-stu-id="8c62c-144">String</span></span>|<span data-ttu-id="8c62c-145">Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="8c62c-145">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="8c62c-146">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8c62c-146">expirationDateTime</span></span>|<span data-ttu-id="8c62c-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c62c-147">DateTimeOffset</span></span>|<span data-ttu-id="8c62c-148">Ablaufdatum und -uhrzeit des Apple Volume Purchase Program-Token.</span><span class="sxs-lookup"><span data-stu-id="8c62c-148">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="8c62c-149">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8c62c-149">lastSyncDateTime</span></span>|<span data-ttu-id="8c62c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c62c-150">DateTimeOffset</span></span>|<span data-ttu-id="8c62c-151">Zeitpunkt der letzten Synchronisierung der Anwendung mit dem Apple Volume Purchase Program Service mithilfe des Apple Volume Purchase Program-Token.</span><span class="sxs-lookup"><span data-stu-id="8c62c-151">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="8c62c-152">token</span><span class="sxs-lookup"><span data-stu-id="8c62c-152">token</span></span>|<span data-ttu-id="8c62c-153">String</span><span class="sxs-lookup"><span data-stu-id="8c62c-153">String</span></span>|<span data-ttu-id="8c62c-154">Aus dem Apple Volume Purchase Program heruntergeladene Zeichenfolge des Apple Volume Purchase Program-Token.</span><span class="sxs-lookup"><span data-stu-id="8c62c-154">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="8c62c-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8c62c-155">lastModifiedDateTime</span></span>|<span data-ttu-id="8c62c-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c62c-156">DateTimeOffset</span></span>|<span data-ttu-id="8c62c-157">Letztes Änderungsdatum und letzter Änderungszeitpunkt des Apple Volume Purchase Program-Token.</span><span class="sxs-lookup"><span data-stu-id="8c62c-157">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="8c62c-158">state</span><span class="sxs-lookup"><span data-stu-id="8c62c-158">state</span></span>|[<span data-ttu-id="8c62c-159">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="8c62c-159">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="8c62c-160">Aktueller Stand des Apple Volume Purchase Program-Token.</span><span class="sxs-lookup"><span data-stu-id="8c62c-160">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="8c62c-161">Mögliche Werte sind: `unknown`, `valid`, `expired`, `invalid` und `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="8c62c-161">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="8c62c-162">Mögliche Werte sind: `unknown`, `valid`, `expired`, `invalid` und `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="8c62c-162">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="8c62c-163">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="8c62c-163">lastSyncStatus</span></span>|[<span data-ttu-id="8c62c-164">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="8c62c-164">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="8c62c-165">Aktueller Synchronisierungsstatus seit der letzten Synchronisierung der Anwendung, die mit dem Apple Volume Purchase Program-Token durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="8c62c-165">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="8c62c-166">Mögliche Werte sind: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="8c62c-166">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="8c62c-167">Mögliche Werte sind: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="8c62c-167">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="8c62c-168">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="8c62c-168">automaticallyUpdateApps</span></span>|<span data-ttu-id="8c62c-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c62c-169">Boolean</span></span>|<span data-ttu-id="8c62c-170">Angabe, ob Anwendungen für das VPP-Token automatisch aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="8c62c-170">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="8c62c-171">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="8c62c-171">countryOrRegion</span></span>|<span data-ttu-id="8c62c-172">String</span><span class="sxs-lookup"><span data-stu-id="8c62c-172">String</span></span>|<span data-ttu-id="8c62c-173">Angabe, ob Anwendungen für das VPP-Token automatisch aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="8c62c-173">Whether or not apps for the VPP token will be automatically updated.</span></span>|



## <a name="response"></a><span data-ttu-id="8c62c-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c62c-174">Response</span></span>
<span data-ttu-id="8c62c-175">Bei Erfolg gibt diese Methode den Antwortcode `201 Created` und ein [vppToken](../resources/intune-onboarding-vpptoken.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8c62c-175">If successful, this method returns a `201 Created` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c62c-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8c62c-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="8c62c-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8c62c-177">Request</span></span>
<span data-ttu-id="8c62c-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8c62c-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens
Content-type: application/json
Content-length: 461

{
  "@odata.type": "#microsoft.graph.vppToken",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "state": "valid",
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```

### <a name="response"></a><span data-ttu-id="8c62c-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="8c62c-179">Response</span></span>
<span data-ttu-id="8c62c-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8c62c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 574

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
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```



