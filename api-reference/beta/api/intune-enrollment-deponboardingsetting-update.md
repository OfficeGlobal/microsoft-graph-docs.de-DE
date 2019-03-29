---
title: DepOnboardingSetting aktualisieren
description: Aktualisieren der Eigenschaften eines depOnboardingSetting-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c882957b8fb44e1df539e98dec96e2c457fe854b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30968238"
---
# <a name="update-deponboardingsetting"></a><span data-ttu-id="07d12-103">DepOnboardingSetting aktualisieren</span><span class="sxs-lookup"><span data-stu-id="07d12-103">Update depOnboardingSetting</span></span>

> <span data-ttu-id="07d12-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="07d12-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07d12-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="07d12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07d12-106">Aktualisieren der Eigenschaften eines [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="07d12-106">Update the properties of a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07d12-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="07d12-107">Prerequisites</span></span>
<span data-ttu-id="07d12-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07d12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07d12-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="07d12-110">Permission type</span></span>|<span data-ttu-id="07d12-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="07d12-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07d12-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="07d12-112">Delegated (work or school account)</span></span>|<span data-ttu-id="07d12-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07d12-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="07d12-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="07d12-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07d12-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="07d12-115">Not supported.</span></span>|
|<span data-ttu-id="07d12-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="07d12-116">Application</span></span>|<span data-ttu-id="07d12-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="07d12-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="07d12-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="07d12-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

## <a name="request-headers"></a><span data-ttu-id="07d12-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="07d12-119">Request headers</span></span>
|<span data-ttu-id="07d12-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="07d12-120">Header</span></span>|<span data-ttu-id="07d12-121">Wert</span><span class="sxs-lookup"><span data-stu-id="07d12-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07d12-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="07d12-122">Authorization</span></span>|<span data-ttu-id="07d12-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="07d12-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07d12-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="07d12-124">Accept</span></span>|<span data-ttu-id="07d12-125">application/json</span><span class="sxs-lookup"><span data-stu-id="07d12-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07d12-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="07d12-126">Request body</span></span>
<span data-ttu-id="07d12-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="07d12-127">In the request body, supply a JSON representation for the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

<span data-ttu-id="07d12-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="07d12-128">The following table shows the properties that are required when you create the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md).</span></span>

|<span data-ttu-id="07d12-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="07d12-129">Property</span></span>|<span data-ttu-id="07d12-130">Typ</span><span class="sxs-lookup"><span data-stu-id="07d12-130">Type</span></span>|<span data-ttu-id="07d12-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07d12-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07d12-132">id</span><span class="sxs-lookup"><span data-stu-id="07d12-132">id</span></span>|<span data-ttu-id="07d12-133">String</span><span class="sxs-lookup"><span data-stu-id="07d12-133">String</span></span>|<span data-ttu-id="07d12-134">UUID für das Objekt</span><span class="sxs-lookup"><span data-stu-id="07d12-134">UUID for the object</span></span>|
|<span data-ttu-id="07d12-135">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="07d12-135">appleIdentifier</span></span>|<span data-ttu-id="07d12-136">String</span><span class="sxs-lookup"><span data-stu-id="07d12-136">String</span></span>|<span data-ttu-id="07d12-137">Die Apple-ID, die zum Abrufen des aktuellen Tokens verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="07d12-137">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="07d12-138">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="07d12-138">tokenExpirationDateTime</span></span>|<span data-ttu-id="07d12-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07d12-139">DateTimeOffset</span></span>|<span data-ttu-id="07d12-140">Wenn das Token abläuft.</span><span class="sxs-lookup"><span data-stu-id="07d12-140">When the token will expire.</span></span>|
|<span data-ttu-id="07d12-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="07d12-141">lastModifiedDateTime</span></span>|<span data-ttu-id="07d12-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07d12-142">DateTimeOffset</span></span>|<span data-ttu-id="07d12-143">Wenn der Dienst an Bord war.</span><span class="sxs-lookup"><span data-stu-id="07d12-143">When the service was onboarded.</span></span>|
|<span data-ttu-id="07d12-144">lastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="07d12-144">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="07d12-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07d12-145">DateTimeOffset</span></span>|<span data-ttu-id="07d12-146">Wenn der Dienst zuletzt mit InTune syned</span><span class="sxs-lookup"><span data-stu-id="07d12-146">When the service last syned with Intune</span></span>|
|<span data-ttu-id="07d12-147">lastSyncTriggeredDateTime</span><span class="sxs-lookup"><span data-stu-id="07d12-147">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="07d12-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07d12-148">DateTimeOffset</span></span>|<span data-ttu-id="07d12-149">Wenn InTune eine Synchronisierung zuletzt angefordert hat.</span><span class="sxs-lookup"><span data-stu-id="07d12-149">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="07d12-150">shareTokenWithSchoolDataSyncService</span><span class="sxs-lookup"><span data-stu-id="07d12-150">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="07d12-151">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="07d12-151">Boolean</span></span>|<span data-ttu-id="07d12-152">Gibt an, ob die DEP-Token-Freigabe mit dem School Data Sync-Dienst aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="07d12-152">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="07d12-153">Lastsyncerrorcode wurden</span><span class="sxs-lookup"><span data-stu-id="07d12-153">lastSyncErrorCode</span></span>|<span data-ttu-id="07d12-154">Int32</span><span class="sxs-lookup"><span data-stu-id="07d12-154">Int32</span></span>|<span data-ttu-id="07d12-155">Fehlercode, der von Apple während der letzten DEP-Synchronisierung gemeldet wurde.</span><span class="sxs-lookup"><span data-stu-id="07d12-155">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="07d12-156">tokenType</span><span class="sxs-lookup"><span data-stu-id="07d12-156">tokenType</span></span>|[<span data-ttu-id="07d12-157">depTokenType</span><span class="sxs-lookup"><span data-stu-id="07d12-157">depTokenType</span></span>](../resources/intune-enrollment-deptokentype.md)|<span data-ttu-id="07d12-158">Ruft den Typ der DEP-Token ab oder legt ihn fest.</span><span class="sxs-lookup"><span data-stu-id="07d12-158">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="07d12-159">Mögliche Werte sind: `none`, `dep` und `appleSchoolManager`.</span><span class="sxs-lookup"><span data-stu-id="07d12-159">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="07d12-160">Tokenname</span><span class="sxs-lookup"><span data-stu-id="07d12-160">tokenName</span></span>|<span data-ttu-id="07d12-161">String</span><span class="sxs-lookup"><span data-stu-id="07d12-161">String</span></span>|<span data-ttu-id="07d12-162">Anzeige Name für DEP-Token</span><span class="sxs-lookup"><span data-stu-id="07d12-162">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="07d12-163">syncedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="07d12-163">syncedDeviceCount</span></span>|<span data-ttu-id="07d12-164">Int32</span><span class="sxs-lookup"><span data-stu-id="07d12-164">Int32</span></span>|<span data-ttu-id="07d12-165">Ruft die Anzahl synchronisierter Geräte ab.</span><span class="sxs-lookup"><span data-stu-id="07d12-165">Gets synced device count</span></span>|
|<span data-ttu-id="07d12-166">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="07d12-166">dataSharingConsentGranted</span></span>|<span data-ttu-id="07d12-167">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="07d12-167">Boolean</span></span>|<span data-ttu-id="07d12-168">Einwilligung zur Datenfreigabe mit Apple DEP Service</span><span class="sxs-lookup"><span data-stu-id="07d12-168">Consent granted for data sharing with Apple Dep Service</span></span>|
|<span data-ttu-id="07d12-169">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="07d12-169">roleScopeTagIds</span></span>|<span data-ttu-id="07d12-170">String collection</span><span class="sxs-lookup"><span data-stu-id="07d12-170">String collection</span></span>|<span data-ttu-id="07d12-171">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="07d12-171">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="07d12-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="07d12-172">Response</span></span>
<span data-ttu-id="07d12-173">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="07d12-173">If successful, this method returns a `200 OK` response code and an updated [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07d12-174">Beispiel</span><span class="sxs-lookup"><span data-stu-id="07d12-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="07d12-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="07d12-175">Request</span></span>
<span data-ttu-id="07d12-176">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="07d12-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
Content-type: application/json
Content-length: 576

{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "appleIdentifier": "Apple Identifier value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
  "lastSyncTriggeredDateTime": "2017-01-01T00:00:02.0916369-08:00",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1,
  "tokenType": "dep",
  "tokenName": "Token Name value",
  "syncedDeviceCount": 1,
  "dataSharingConsentGranted": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="07d12-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="07d12-177">Response</span></span>
<span data-ttu-id="07d12-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="07d12-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 689

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
  "dataSharingConsentGranted": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




