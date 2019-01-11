---
title: Erstellen von depOnboardingSetting
description: Erstellen eines neuen DepOnboardingSetting-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 89e46c715b5f888ae3c9f1fb02a0566da8485944
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854901"
---
# <a name="create-deponboardingsetting"></a><span data-ttu-id="ff40f-103">Erstellen von depOnboardingSetting</span><span class="sxs-lookup"><span data-stu-id="ff40f-103">Create depOnboardingSetting</span></span>

> <span data-ttu-id="ff40f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ff40f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff40f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ff40f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff40f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ff40f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff40f-107">Erstellen eines neuen [DepOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ff40f-107">Create a new [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ff40f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ff40f-108">Prerequisites</span></span>
<span data-ttu-id="ff40f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff40f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff40f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ff40f-111">Permission type</span></span>|<span data-ttu-id="ff40f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ff40f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff40f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ff40f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff40f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff40f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ff40f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ff40f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff40f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ff40f-116">Not supported.</span></span>|
|<span data-ttu-id="ff40f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ff40f-117">Application</span></span>|<span data-ttu-id="ff40f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ff40f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff40f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff40f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings
```

## <a name="request-headers"></a><span data-ttu-id="ff40f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ff40f-120">Request headers</span></span>
|<span data-ttu-id="ff40f-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ff40f-121">Header</span></span>|<span data-ttu-id="ff40f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ff40f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff40f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff40f-123">Authorization</span></span>|<span data-ttu-id="ff40f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ff40f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff40f-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ff40f-125">Accept</span></span>|<span data-ttu-id="ff40f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff40f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff40f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ff40f-127">Request body</span></span>
<span data-ttu-id="ff40f-128">Geben Sie im Textkörper Anforderung für das Objekt DepOnboardingSetting eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="ff40f-128">In the request body, supply a JSON representation for the depOnboardingSetting object.</span></span>

<span data-ttu-id="ff40f-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die DepOnboardingSetting erstellen.</span><span class="sxs-lookup"><span data-stu-id="ff40f-129">The following table shows the properties that are required when you create the depOnboardingSetting.</span></span>

|<span data-ttu-id="ff40f-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ff40f-130">Property</span></span>|<span data-ttu-id="ff40f-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ff40f-131">Type</span></span>|<span data-ttu-id="ff40f-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ff40f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff40f-133">id</span><span class="sxs-lookup"><span data-stu-id="ff40f-133">id</span></span>|<span data-ttu-id="ff40f-134">String</span><span class="sxs-lookup"><span data-stu-id="ff40f-134">String</span></span>|<span data-ttu-id="ff40f-135">UUID für das Objekt</span><span class="sxs-lookup"><span data-stu-id="ff40f-135">UUID for the object</span></span>|
|<span data-ttu-id="ff40f-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="ff40f-136">appleIdentifier</span></span>|<span data-ttu-id="ff40f-137">String</span><span class="sxs-lookup"><span data-stu-id="ff40f-137">String</span></span>|<span data-ttu-id="ff40f-138">Die Apple-ID verwendet, um das aktuelle Token abzurufen.</span><span class="sxs-lookup"><span data-stu-id="ff40f-138">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="ff40f-139">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ff40f-139">tokenExpirationDateTime</span></span>|<span data-ttu-id="ff40f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff40f-140">DateTimeOffset</span></span>|<span data-ttu-id="ff40f-141">Wenn das Token abläuft.</span><span class="sxs-lookup"><span data-stu-id="ff40f-141">When the token will expire.</span></span>|
|<span data-ttu-id="ff40f-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff40f-142">lastModifiedDateTime</span></span>|<span data-ttu-id="ff40f-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff40f-143">DateTimeOffset</span></span>|<span data-ttu-id="ff40f-144">Wenn der Dienst Onboarded wurde.</span><span class="sxs-lookup"><span data-stu-id="ff40f-144">When the service was onboarded.</span></span>|
|<span data-ttu-id="ff40f-145">lastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ff40f-145">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="ff40f-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff40f-146">DateTimeOffset</span></span>|<span data-ttu-id="ff40f-147">Wenn der Dienst letzten Syned mit Intune</span><span class="sxs-lookup"><span data-stu-id="ff40f-147">When the service last syned with Intune</span></span>|
|<span data-ttu-id="ff40f-148">lastSyncTriggeredDateTime</span><span class="sxs-lookup"><span data-stu-id="ff40f-148">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="ff40f-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff40f-149">DateTimeOffset</span></span>|<span data-ttu-id="ff40f-150">Wenn Intune zuletzt eine Synchronisierung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="ff40f-150">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="ff40f-151">shareTokenWithSchoolDataSyncService</span><span class="sxs-lookup"><span data-stu-id="ff40f-151">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="ff40f-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff40f-152">Boolean</span></span>|<span data-ttu-id="ff40f-153">Unabhängig davon, ob die Datenausführungsverhinderung token Freigabe mit dem Schule Daten Sync-Dienst aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="ff40f-153">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="ff40f-154">lastSyncErrorCode</span><span class="sxs-lookup"><span data-stu-id="ff40f-154">lastSyncErrorCode</span></span>|<span data-ttu-id="ff40f-155">Int32</span><span class="sxs-lookup"><span data-stu-id="ff40f-155">Int32</span></span>|<span data-ttu-id="ff40f-156">Fehlercode von Apple während der letzten Synchronisierung der Datenausführungsverhinderung gemeldet.</span><span class="sxs-lookup"><span data-stu-id="ff40f-156">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="ff40f-157">"TokenType"</span><span class="sxs-lookup"><span data-stu-id="ff40f-157">tokenType</span></span>|[<span data-ttu-id="ff40f-158">depTokenType</span><span class="sxs-lookup"><span data-stu-id="ff40f-158">depTokenType</span></span>](../resources/intune-enrollment-deptokentype.md)|<span data-ttu-id="ff40f-159">Ruft ab oder legt ihn fest die Datenausführungsverhinderung Token.</span><span class="sxs-lookup"><span data-stu-id="ff40f-159">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="ff40f-160">Mögliche Werte sind: `none`, `dep` und `appleSchoolManager`.</span><span class="sxs-lookup"><span data-stu-id="ff40f-160">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="ff40f-161">tokenName</span><span class="sxs-lookup"><span data-stu-id="ff40f-161">tokenName</span></span>|<span data-ttu-id="ff40f-162">String</span><span class="sxs-lookup"><span data-stu-id="ff40f-162">String</span></span>|<span data-ttu-id="ff40f-163">Anzeigename für die Datenausführungsverhinderung Token</span><span class="sxs-lookup"><span data-stu-id="ff40f-163">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="ff40f-164">syncedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ff40f-164">syncedDeviceCount</span></span>|<span data-ttu-id="ff40f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ff40f-165">Int32</span></span>|<span data-ttu-id="ff40f-166">Ruft synchronisierter Anzahl der Geräte</span><span class="sxs-lookup"><span data-stu-id="ff40f-166">Gets synced device count</span></span>|
|<span data-ttu-id="ff40f-167">defaultProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="ff40f-167">defaultProfileDisplayName</span></span>|<span data-ttu-id="ff40f-168">String</span><span class="sxs-lookup"><span data-stu-id="ff40f-168">String</span></span>|<span data-ttu-id="ff40f-169">Ruft synchronisierter Anzahl der Geräte</span><span class="sxs-lookup"><span data-stu-id="ff40f-169">Gets synced device count</span></span>|
|<span data-ttu-id="ff40f-170">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="ff40f-170">dataSharingConsentGranted</span></span>|<span data-ttu-id="ff40f-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff40f-171">Boolean</span></span>|<span data-ttu-id="ff40f-172">Stimmen Sie gewährte Zugriffsberechtigungen für die Datenfreigabe mit Apple Dep-Dienst</span><span class="sxs-lookup"><span data-stu-id="ff40f-172">Consent granted for data sharing with Apple Dep Service</span></span>|



## <a name="response"></a><span data-ttu-id="ff40f-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff40f-173">Response</span></span>
<span data-ttu-id="ff40f-174">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [DepOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ff40f-174">If successful, this method returns a `201 Created` response code and a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff40f-175">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ff40f-175">Example</span></span>
### <a name="request"></a><span data-ttu-id="ff40f-176">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff40f-176">Request</span></span>
<span data-ttu-id="ff40f-177">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ff40f-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ff40f-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff40f-178">Response</span></span>
<span data-ttu-id="ff40f-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ff40f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





