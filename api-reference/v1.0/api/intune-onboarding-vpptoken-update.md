---
title: VppToken aktualisieren
description: Aktualisieren der Eigenschaften eines vppToken-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5574a791de1d357d0e1b211530ac3121d96383cc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983100"
---
# <a name="update-vpptoken"></a><span data-ttu-id="ea34c-103">VppToken aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ea34c-103">Update vppToken</span></span>

> <span data-ttu-id="ea34c-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ea34c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea34c-105">Aktualisieren der Eigenschaften eines [vppToken](../resources/intune-onboarding-vpptoken.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ea34c-105">Update the properties of a [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ea34c-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ea34c-106">Prerequisites</span></span>
<span data-ttu-id="ea34c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea34c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea34c-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ea34c-109">Permission type</span></span>|<span data-ttu-id="ea34c-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ea34c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea34c-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ea34c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ea34c-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea34c-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ea34c-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ea34c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea34c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ea34c-114">Not supported.</span></span>|
|<span data-ttu-id="ea34c-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ea34c-115">Application</span></span>|<span data-ttu-id="ea34c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ea34c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea34c-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ea34c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a><span data-ttu-id="ea34c-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ea34c-118">Request headers</span></span>
|<span data-ttu-id="ea34c-119">Header</span><span class="sxs-lookup"><span data-stu-id="ea34c-119">Header</span></span>|<span data-ttu-id="ea34c-120">Wert</span><span class="sxs-lookup"><span data-stu-id="ea34c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea34c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea34c-121">Authorization</span></span>|<span data-ttu-id="ea34c-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ea34c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea34c-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ea34c-123">Accept</span></span>|<span data-ttu-id="ea34c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ea34c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea34c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ea34c-125">Request body</span></span>
<span data-ttu-id="ea34c-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [vppToken](../resources/intune-onboarding-vpptoken.md) an.</span><span class="sxs-lookup"><span data-stu-id="ea34c-126">In the request body, supply a JSON representation for the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

<span data-ttu-id="ea34c-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [vppToken](../resources/intune-onboarding-vpptoken.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="ea34c-127">The following table shows the properties that are required when you create the [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>

|<span data-ttu-id="ea34c-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ea34c-128">Property</span></span>|<span data-ttu-id="ea34c-129">Typ</span><span class="sxs-lookup"><span data-stu-id="ea34c-129">Type</span></span>|<span data-ttu-id="ea34c-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ea34c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea34c-131">id</span><span class="sxs-lookup"><span data-stu-id="ea34c-131">id</span></span>|<span data-ttu-id="ea34c-132">String</span><span class="sxs-lookup"><span data-stu-id="ea34c-132">String</span></span>|<span data-ttu-id="ea34c-133">Wird automatisch generiert, wenn AppleVolumePurchaseProgramToken erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="ea34c-133">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="ea34c-134">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="ea34c-134">It is the Key of the entity.</span></span>|
|<span data-ttu-id="ea34c-135">organizationName</span><span class="sxs-lookup"><span data-stu-id="ea34c-135">organizationName</span></span>|<span data-ttu-id="ea34c-136">String</span><span class="sxs-lookup"><span data-stu-id="ea34c-136">String</span></span>|<span data-ttu-id="ea34c-137">Organisation, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="ea34c-137">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="ea34c-138">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="ea34c-138">vppTokenAccountType</span></span>|[<span data-ttu-id="ea34c-139">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="ea34c-139">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="ea34c-140">Volume Purchase Program-Typ, dem das angegebene Apple Volume Purchase Program-Token zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="ea34c-140">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="ea34c-141">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="ea34c-141">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="ea34c-142">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="ea34c-142">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="ea34c-143">appleId</span><span class="sxs-lookup"><span data-stu-id="ea34c-143">appleId</span></span>|<span data-ttu-id="ea34c-144">String</span><span class="sxs-lookup"><span data-stu-id="ea34c-144">String</span></span>|<span data-ttu-id="ea34c-145">Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="ea34c-145">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="ea34c-146">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ea34c-146">expirationDateTime</span></span>|<span data-ttu-id="ea34c-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea34c-147">DateTimeOffset</span></span>|<span data-ttu-id="ea34c-148">Ablaufdatum und -uhrzeit des Apple Volume Purchase Program-Token.</span><span class="sxs-lookup"><span data-stu-id="ea34c-148">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="ea34c-149">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ea34c-149">lastSyncDateTime</span></span>|<span data-ttu-id="ea34c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea34c-150">DateTimeOffset</span></span>|<span data-ttu-id="ea34c-151">Zeitpunkt der letzten Synchronisierung der Anwendung mit dem Apple Volume Purchase Program Service mithilfe des Apple Volume Purchase Program-Token.</span><span class="sxs-lookup"><span data-stu-id="ea34c-151">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="ea34c-152">token</span><span class="sxs-lookup"><span data-stu-id="ea34c-152">token</span></span>|<span data-ttu-id="ea34c-153">String</span><span class="sxs-lookup"><span data-stu-id="ea34c-153">String</span></span>|<span data-ttu-id="ea34c-154">Aus dem Apple Volume Purchase Program heruntergeladene Zeichenfolge des Apple Volume Purchase Program-Token.</span><span class="sxs-lookup"><span data-stu-id="ea34c-154">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="ea34c-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ea34c-155">lastModifiedDateTime</span></span>|<span data-ttu-id="ea34c-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea34c-156">DateTimeOffset</span></span>|<span data-ttu-id="ea34c-157">Letztes Änderungsdatum und letzter Änderungszeitpunkt des Apple Volume Purchase Program-Token.</span><span class="sxs-lookup"><span data-stu-id="ea34c-157">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="ea34c-158">state</span><span class="sxs-lookup"><span data-stu-id="ea34c-158">state</span></span>|[<span data-ttu-id="ea34c-159">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="ea34c-159">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="ea34c-160">Aktueller Stand des Apple Volume Purchase Program-Token.</span><span class="sxs-lookup"><span data-stu-id="ea34c-160">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="ea34c-161">Mögliche Werte sind: `unknown`, `valid`, `expired`, `invalid` und `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="ea34c-161">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="ea34c-162">Mögliche Werte sind: `unknown`, `valid`, `expired`, `invalid` und `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="ea34c-162">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="ea34c-163">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="ea34c-163">lastSyncStatus</span></span>|[<span data-ttu-id="ea34c-164">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="ea34c-164">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="ea34c-165">Aktueller Synchronisierungsstatus seit der letzten Synchronisierung der Anwendung, die mit dem Apple Volume Purchase Program-Token durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="ea34c-165">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="ea34c-166">Mögliche Werte sind: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="ea34c-166">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="ea34c-167">Mögliche Werte sind: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="ea34c-167">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="ea34c-168">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="ea34c-168">automaticallyUpdateApps</span></span>|<span data-ttu-id="ea34c-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea34c-169">Boolean</span></span>|<span data-ttu-id="ea34c-170">Angabe, ob Anwendungen für das VPP-Token automatisch aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="ea34c-170">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="ea34c-171">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="ea34c-171">countryOrRegion</span></span>|<span data-ttu-id="ea34c-172">String</span><span class="sxs-lookup"><span data-stu-id="ea34c-172">String</span></span>|<span data-ttu-id="ea34c-173">Angabe, ob Anwendungen für das VPP-Token automatisch aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="ea34c-173">Whether or not apps for the VPP token will be automatically updated.</span></span>|



## <a name="response"></a><span data-ttu-id="ea34c-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="ea34c-174">Response</span></span>
<span data-ttu-id="ea34c-175">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [vppToken](../resources/intune-onboarding-vpptoken.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ea34c-175">If successful, this method returns a `200 OK` response code and an updated [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea34c-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ea34c-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="ea34c-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ea34c-177">Request</span></span>
<span data-ttu-id="ea34c-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ea34c-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}
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

### <a name="response"></a><span data-ttu-id="ea34c-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="ea34c-179">Response</span></span>
<span data-ttu-id="ea34c-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ea34c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



