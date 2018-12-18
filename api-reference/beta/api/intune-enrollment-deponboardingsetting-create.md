---
title: Erstellen von depOnboardingSetting
description: Erstellen eines neuen DepOnboardingSetting-Objekts.
author: tfitzmac
ms.openlocfilehash: 11f2e5217e4040a7d4345c9271b459e608075498
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330660"
---
# <a name="create-deponboardingsetting"></a><span data-ttu-id="d461d-103">Erstellen von depOnboardingSetting</span><span class="sxs-lookup"><span data-stu-id="d461d-103">Create depOnboardingSetting</span></span>

> <span data-ttu-id="d461d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d461d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d461d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d461d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d461d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d461d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d461d-107">Erstellen eines neuen [DepOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d461d-107">Create a new [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d461d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d461d-108">Prerequisites</span></span>
<span data-ttu-id="d461d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d461d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d461d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d461d-111">Permission type</span></span>|<span data-ttu-id="d461d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d461d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d461d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d461d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d461d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d461d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d461d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d461d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d461d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d461d-116">Not supported.</span></span>|
|<span data-ttu-id="d461d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d461d-117">Application</span></span>|<span data-ttu-id="d461d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d461d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d461d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d461d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings
```

## <a name="request-headers"></a><span data-ttu-id="d461d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d461d-120">Request headers</span></span>
|<span data-ttu-id="d461d-121">Header</span><span class="sxs-lookup"><span data-stu-id="d461d-121">Header</span></span>|<span data-ttu-id="d461d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d461d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d461d-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d461d-123">Authorization</span></span>|<span data-ttu-id="d461d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d461d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d461d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d461d-125">Accept</span></span>|<span data-ttu-id="d461d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d461d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d461d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d461d-127">Request body</span></span>
<span data-ttu-id="d461d-128">Geben Sie im Textkörper Anforderung für das Objekt DepOnboardingSetting eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="d461d-128">In the request body, supply a JSON representation for the depOnboardingSetting object.</span></span>

<span data-ttu-id="d461d-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die DepOnboardingSetting erstellen.</span><span class="sxs-lookup"><span data-stu-id="d461d-129">The following table shows the properties that are required when you create the depOnboardingSetting.</span></span>

|<span data-ttu-id="d461d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d461d-130">Property</span></span>|<span data-ttu-id="d461d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="d461d-131">Type</span></span>|<span data-ttu-id="d461d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d461d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d461d-133">id</span><span class="sxs-lookup"><span data-stu-id="d461d-133">id</span></span>|<span data-ttu-id="d461d-134">String</span><span class="sxs-lookup"><span data-stu-id="d461d-134">String</span></span>|<span data-ttu-id="d461d-135">UUID für das Objekt</span><span class="sxs-lookup"><span data-stu-id="d461d-135">UUID for the object</span></span>|
|<span data-ttu-id="d461d-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="d461d-136">appleIdentifier</span></span>|<span data-ttu-id="d461d-137">String</span><span class="sxs-lookup"><span data-stu-id="d461d-137">String</span></span>|<span data-ttu-id="d461d-138">Die Apple-ID verwendet, um das aktuelle Token abzurufen.</span><span class="sxs-lookup"><span data-stu-id="d461d-138">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="d461d-139">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d461d-139">tokenExpirationDateTime</span></span>|<span data-ttu-id="d461d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d461d-140">DateTimeOffset</span></span>|<span data-ttu-id="d461d-141">Wenn das Token abläuft.</span><span class="sxs-lookup"><span data-stu-id="d461d-141">When the token will expire.</span></span>|
|<span data-ttu-id="d461d-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d461d-142">lastModifiedDateTime</span></span>|<span data-ttu-id="d461d-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d461d-143">DateTimeOffset</span></span>|<span data-ttu-id="d461d-144">Wenn der Dienst Onboarded wurde.</span><span class="sxs-lookup"><span data-stu-id="d461d-144">When the service was onboarded.</span></span>|
|<span data-ttu-id="d461d-145">lastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d461d-145">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="d461d-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d461d-146">DateTimeOffset</span></span>|<span data-ttu-id="d461d-147">Wenn der Dienst letzten Syned mit Intune</span><span class="sxs-lookup"><span data-stu-id="d461d-147">When the service last syned with Intune</span></span>|
|<span data-ttu-id="d461d-148">lastSyncTriggeredDateTime</span><span class="sxs-lookup"><span data-stu-id="d461d-148">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="d461d-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d461d-149">DateTimeOffset</span></span>|<span data-ttu-id="d461d-150">Wenn Intune zuletzt eine Synchronisierung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="d461d-150">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="d461d-151">shareTokenWithSchoolDataSyncService</span><span class="sxs-lookup"><span data-stu-id="d461d-151">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="d461d-152">Boolesch</span><span class="sxs-lookup"><span data-stu-id="d461d-152">Boolean</span></span>|<span data-ttu-id="d461d-153">Unabhängig davon, ob die Datenausführungsverhinderung token Freigabe mit dem Schule Daten Sync-Dienst aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="d461d-153">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="d461d-154">lastSyncErrorCode</span><span class="sxs-lookup"><span data-stu-id="d461d-154">lastSyncErrorCode</span></span>|<span data-ttu-id="d461d-155">Int32</span><span class="sxs-lookup"><span data-stu-id="d461d-155">Int32</span></span>|<span data-ttu-id="d461d-156">Fehlercode von Apple während der letzten Synchronisierung der Datenausführungsverhinderung gemeldet.</span><span class="sxs-lookup"><span data-stu-id="d461d-156">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="d461d-157">"TokenType"</span><span class="sxs-lookup"><span data-stu-id="d461d-157">tokenType</span></span>|[<span data-ttu-id="d461d-158">depTokenType</span><span class="sxs-lookup"><span data-stu-id="d461d-158">depTokenType</span></span>](../resources/intune-enrollment-deptokentype.md)|<span data-ttu-id="d461d-159">Ruft ab oder legt ihn fest die Datenausführungsverhinderung Token.</span><span class="sxs-lookup"><span data-stu-id="d461d-159">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="d461d-160">Mögliche Werte sind: `none`, `dep` und `appleSchoolManager`.</span><span class="sxs-lookup"><span data-stu-id="d461d-160">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="d461d-161">tokenName</span><span class="sxs-lookup"><span data-stu-id="d461d-161">tokenName</span></span>|<span data-ttu-id="d461d-162">String</span><span class="sxs-lookup"><span data-stu-id="d461d-162">String</span></span>|<span data-ttu-id="d461d-163">Anzeigename für die Datenausführungsverhinderung Token</span><span class="sxs-lookup"><span data-stu-id="d461d-163">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="d461d-164">syncedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d461d-164">syncedDeviceCount</span></span>|<span data-ttu-id="d461d-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d461d-165">Int32</span></span>|<span data-ttu-id="d461d-166">Ruft synchronisierter Anzahl der Geräte</span><span class="sxs-lookup"><span data-stu-id="d461d-166">Gets synced device count</span></span>|
|<span data-ttu-id="d461d-167">defaultProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="d461d-167">defaultProfileDisplayName</span></span>|<span data-ttu-id="d461d-168">String</span><span class="sxs-lookup"><span data-stu-id="d461d-168">String</span></span>|<span data-ttu-id="d461d-169">Ruft synchronisierter Anzahl der Geräte</span><span class="sxs-lookup"><span data-stu-id="d461d-169">Gets synced device count</span></span>|
|<span data-ttu-id="d461d-170">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="d461d-170">dataSharingConsentGranted</span></span>|<span data-ttu-id="d461d-171">Boolesch</span><span class="sxs-lookup"><span data-stu-id="d461d-171">Boolean</span></span>|<span data-ttu-id="d461d-172">Stimmen Sie gewährte Zugriffsberechtigungen für die Datenfreigabe mit Apple Dep-Dienst</span><span class="sxs-lookup"><span data-stu-id="d461d-172">Consent granted for data sharing with Apple Dep Service</span></span>|



## <a name="response"></a><span data-ttu-id="d461d-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="d461d-173">Response</span></span>
<span data-ttu-id="d461d-174">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [DepOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d461d-174">If successful, this method returns a `201 Created` response code and a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d461d-175">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d461d-175">Example</span></span>
### <a name="request"></a><span data-ttu-id="d461d-176">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d461d-176">Request</span></span>
<span data-ttu-id="d461d-177">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d461d-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings
Content-type: application/json
Content-length: 648

{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "appleIdentifier": "Apple Identifier value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
  "lastSyncTriggeredDateTime": "2017-01-01T00:00:02.0916369-08:00",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1,
  "tokenType": "dep",
  "tokenName": "Token Name value",
  "syncedDeviceCount": 1,
  "defaultProfileDisplayName": "Default Profile Display Name value",
  "dataSharingConsentGranted": true
}
```

### <a name="response"></a><span data-ttu-id="d461d-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="d461d-178">Response</span></span>
<span data-ttu-id="d461d-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d461d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 697

{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "id": "40342229-2229-4034-2922-344029223440",
  "appleIdentifier": "Apple Identifier value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
  "lastSyncTriggeredDateTime": "2017-01-01T00:00:02.0916369-08:00",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1,
  "tokenType": "dep",
  "tokenName": "Token Name value",
  "syncedDeviceCount": 1,
  "defaultProfileDisplayName": "Default Profile Display Name value",
  "dataSharingConsentGranted": true
}
```





