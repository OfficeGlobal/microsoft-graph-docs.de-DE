---
title: DepOnboardingSetting aktualisieren
description: Aktualisieren Sie die Eigenschaften eines DepOnboardingSetting-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 78d3138950776dd74a055fbb00339e9e69b5f0f1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412289"
---
# <a name="update-deponboardingsetting"></a><span data-ttu-id="71fee-103">DepOnboardingSetting aktualisieren</span><span class="sxs-lookup"><span data-stu-id="71fee-103">Update depOnboardingSetting</span></span>

> <span data-ttu-id="71fee-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="71fee-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="71fee-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="71fee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="71fee-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="71fee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71fee-107">Aktualisieren Sie die Eigenschaften eines [DepOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="71fee-107">Update the properties of a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71fee-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="71fee-108">Prerequisites</span></span>
<span data-ttu-id="71fee-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="71fee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="71fee-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="71fee-111">Permission type</span></span>|<span data-ttu-id="71fee-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="71fee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71fee-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="71fee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="71fee-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71fee-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="71fee-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="71fee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71fee-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71fee-116">Not supported.</span></span>|
|<span data-ttu-id="71fee-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="71fee-117">Application</span></span>|<span data-ttu-id="71fee-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71fee-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71fee-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="71fee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

## <a name="request-headers"></a><span data-ttu-id="71fee-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="71fee-120">Request headers</span></span>
|<span data-ttu-id="71fee-121">Header</span><span class="sxs-lookup"><span data-stu-id="71fee-121">Header</span></span>|<span data-ttu-id="71fee-122">Wert</span><span class="sxs-lookup"><span data-stu-id="71fee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71fee-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="71fee-123">Authorization</span></span>|<span data-ttu-id="71fee-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="71fee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71fee-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="71fee-125">Accept</span></span>|<span data-ttu-id="71fee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="71fee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71fee-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="71fee-127">Request body</span></span>
<span data-ttu-id="71fee-128">Geben Sie im Textkörper Anforderung für das Objekt [DepOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="71fee-128">In the request body, supply a JSON representation for the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

<span data-ttu-id="71fee-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [DepOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="71fee-129">The following table shows the properties that are required when you create the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md).</span></span>

|<span data-ttu-id="71fee-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="71fee-130">Property</span></span>|<span data-ttu-id="71fee-131">Typ</span><span class="sxs-lookup"><span data-stu-id="71fee-131">Type</span></span>|<span data-ttu-id="71fee-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71fee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71fee-133">id</span><span class="sxs-lookup"><span data-stu-id="71fee-133">id</span></span>|<span data-ttu-id="71fee-134">String</span><span class="sxs-lookup"><span data-stu-id="71fee-134">String</span></span>|<span data-ttu-id="71fee-135">UUID für das Objekt</span><span class="sxs-lookup"><span data-stu-id="71fee-135">UUID for the object</span></span>|
|<span data-ttu-id="71fee-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="71fee-136">appleIdentifier</span></span>|<span data-ttu-id="71fee-137">String</span><span class="sxs-lookup"><span data-stu-id="71fee-137">String</span></span>|<span data-ttu-id="71fee-138">Die Apple-ID verwendet, um das aktuelle Token abzurufen.</span><span class="sxs-lookup"><span data-stu-id="71fee-138">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="71fee-139">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="71fee-139">tokenExpirationDateTime</span></span>|<span data-ttu-id="71fee-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71fee-140">DateTimeOffset</span></span>|<span data-ttu-id="71fee-141">Wenn das Token abläuft.</span><span class="sxs-lookup"><span data-stu-id="71fee-141">When the token will expire.</span></span>|
|<span data-ttu-id="71fee-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71fee-142">lastModifiedDateTime</span></span>|<span data-ttu-id="71fee-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71fee-143">DateTimeOffset</span></span>|<span data-ttu-id="71fee-144">Wenn der Dienst Onboarded wurde.</span><span class="sxs-lookup"><span data-stu-id="71fee-144">When the service was onboarded.</span></span>|
|<span data-ttu-id="71fee-145">lastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="71fee-145">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="71fee-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71fee-146">DateTimeOffset</span></span>|<span data-ttu-id="71fee-147">Wenn der Dienst letzten Syned mit Intune</span><span class="sxs-lookup"><span data-stu-id="71fee-147">When the service last syned with Intune</span></span>|
|<span data-ttu-id="71fee-148">lastSyncTriggeredDateTime</span><span class="sxs-lookup"><span data-stu-id="71fee-148">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="71fee-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71fee-149">DateTimeOffset</span></span>|<span data-ttu-id="71fee-150">Wenn Intune zuletzt eine Synchronisierung angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="71fee-150">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="71fee-151">shareTokenWithSchoolDataSyncService</span><span class="sxs-lookup"><span data-stu-id="71fee-151">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="71fee-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="71fee-152">Boolean</span></span>|<span data-ttu-id="71fee-153">Unabhängig davon, ob die Datenausführungsverhinderung token Freigabe mit dem Schule Daten Sync-Dienst aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="71fee-153">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="71fee-154">lastSyncErrorCode</span><span class="sxs-lookup"><span data-stu-id="71fee-154">lastSyncErrorCode</span></span>|<span data-ttu-id="71fee-155">Int32</span><span class="sxs-lookup"><span data-stu-id="71fee-155">Int32</span></span>|<span data-ttu-id="71fee-156">Fehlercode von Apple während der letzten Synchronisierung der Datenausführungsverhinderung gemeldet.</span><span class="sxs-lookup"><span data-stu-id="71fee-156">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="71fee-157">"TokenType"</span><span class="sxs-lookup"><span data-stu-id="71fee-157">tokenType</span></span>|[<span data-ttu-id="71fee-158">depTokenType</span><span class="sxs-lookup"><span data-stu-id="71fee-158">depTokenType</span></span>](../resources/intune-enrollment-deptokentype.md)|<span data-ttu-id="71fee-159">Ruft ab oder legt ihn fest die Datenausführungsverhinderung Token.</span><span class="sxs-lookup"><span data-stu-id="71fee-159">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="71fee-160">Mögliche Werte sind: `none`, `dep` und `appleSchoolManager`.</span><span class="sxs-lookup"><span data-stu-id="71fee-160">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="71fee-161">tokenName</span><span class="sxs-lookup"><span data-stu-id="71fee-161">tokenName</span></span>|<span data-ttu-id="71fee-162">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="71fee-162">String</span></span>|<span data-ttu-id="71fee-163">Anzeigename für die Datenausführungsverhinderung Token</span><span class="sxs-lookup"><span data-stu-id="71fee-163">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="71fee-164">syncedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="71fee-164">syncedDeviceCount</span></span>|<span data-ttu-id="71fee-165">Int32</span><span class="sxs-lookup"><span data-stu-id="71fee-165">Int32</span></span>|<span data-ttu-id="71fee-166">Ruft synchronisierter Anzahl der Geräte</span><span class="sxs-lookup"><span data-stu-id="71fee-166">Gets synced device count</span></span>|
|<span data-ttu-id="71fee-167">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="71fee-167">dataSharingConsentGranted</span></span>|<span data-ttu-id="71fee-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="71fee-168">Boolean</span></span>|<span data-ttu-id="71fee-169">Stimmen Sie gewährte Zugriffsberechtigungen für die Datenfreigabe mit Apple Dep-Dienst</span><span class="sxs-lookup"><span data-stu-id="71fee-169">Consent granted for data sharing with Apple Dep Service</span></span>|



## <a name="response"></a><span data-ttu-id="71fee-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="71fee-170">Response</span></span>
<span data-ttu-id="71fee-171">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [DepOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="71fee-171">If successful, this method returns a `200 OK` response code and an updated [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71fee-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="71fee-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="71fee-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="71fee-173">Request</span></span>
<span data-ttu-id="71fee-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="71fee-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
Content-type: application/json
Content-length: 514

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
  "dataSharingConsentGranted": true
}
```

### <a name="response"></a><span data-ttu-id="71fee-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="71fee-175">Response</span></span>
<span data-ttu-id="71fee-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="71fee-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 627

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
  "dataSharingConsentGranted": true
}
```




