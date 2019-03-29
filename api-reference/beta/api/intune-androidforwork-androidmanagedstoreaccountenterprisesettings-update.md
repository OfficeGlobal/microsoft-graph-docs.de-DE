---
title: Androidmanagedstoreaccountenterprisesettings hinzugefügt aktualisieren
description: Aktualisieren der Eigenschaften eines Androidmanagedstoreaccountenterprisesettings hinzugefügt-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2fa5d3d4187ce462c0d3e4875d2a77b60d7e66bb
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960587"
---
# <a name="update-androidmanagedstoreaccountenterprisesettings"></a><span data-ttu-id="d9f95-103">Androidmanagedstoreaccountenterprisesettings hinzugefügt aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d9f95-103">Update androidManagedStoreAccountEnterpriseSettings</span></span>

> <span data-ttu-id="d9f95-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d9f95-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9f95-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d9f95-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9f95-106">Aktualisieren der Eigenschaften eines [androidmanagedstoreaccountenterprisesettings hinzugefügt](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d9f95-106">Update the properties of a [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9f95-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d9f95-107">Prerequisites</span></span>
<span data-ttu-id="d9f95-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9f95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9f95-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d9f95-110">Permission type</span></span>|<span data-ttu-id="d9f95-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d9f95-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9f95-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d9f95-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d9f95-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9f95-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d9f95-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d9f95-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9f95-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d9f95-115">Not supported.</span></span>|
|<span data-ttu-id="d9f95-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d9f95-116">Application</span></span>|<span data-ttu-id="d9f95-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d9f95-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9f95-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9f95-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAccountEnterpriseSettings
```

## <a name="request-headers"></a><span data-ttu-id="d9f95-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d9f95-119">Request headers</span></span>
|<span data-ttu-id="d9f95-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d9f95-120">Header</span></span>|<span data-ttu-id="d9f95-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d9f95-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9f95-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9f95-122">Authorization</span></span>|<span data-ttu-id="d9f95-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d9f95-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9f95-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d9f95-124">Accept</span></span>|<span data-ttu-id="d9f95-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d9f95-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9f95-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d9f95-126">Request body</span></span>
<span data-ttu-id="d9f95-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [androidmanagedstoreaccountenterprisesettings hinzugefügt](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="d9f95-127">In the request body, supply a JSON representation for the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

<span data-ttu-id="d9f95-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androidmanagedstoreaccountenterprisesettings hinzugefügt](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="d9f95-128">The following table shows the properties that are required when you create the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md).</span></span>

|<span data-ttu-id="d9f95-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d9f95-129">Property</span></span>|<span data-ttu-id="d9f95-130">Typ</span><span class="sxs-lookup"><span data-stu-id="d9f95-130">Type</span></span>|<span data-ttu-id="d9f95-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d9f95-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9f95-132">id</span><span class="sxs-lookup"><span data-stu-id="d9f95-132">id</span></span>|<span data-ttu-id="d9f95-133">String</span><span class="sxs-lookup"><span data-stu-id="d9f95-133">String</span></span>|<span data-ttu-id="d9f95-134">Das Android Store-Konto Enterprise-Einstellungs-ID</span><span class="sxs-lookup"><span data-stu-id="d9f95-134">The Android store account enterprise settings identifier</span></span>|
|<span data-ttu-id="d9f95-135">bindStatus</span><span class="sxs-lookup"><span data-stu-id="d9f95-135">bindStatus</span></span>|[<span data-ttu-id="d9f95-136">androidManagedStoreAccountBindStatus</span><span class="sxs-lookup"><span data-stu-id="d9f95-136">androidManagedStoreAccountBindStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|<span data-ttu-id="d9f95-137">Binden des Status des Mandanten mit der Google EMM-API.</span><span class="sxs-lookup"><span data-stu-id="d9f95-137">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="d9f95-138">Mögliche Werte sind: `notBound`, `bound`, `boundAndValidated` und `unbinding`.</span><span class="sxs-lookup"><span data-stu-id="d9f95-138">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="d9f95-139">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d9f95-139">lastAppSyncDateTime</span></span>|<span data-ttu-id="d9f95-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9f95-140">DateTimeOffset</span></span>|<span data-ttu-id="d9f95-141">Zeitpunkt, zu dem zuletzt eine App-Synchronisierung abgeschlossen wurde.</span><span class="sxs-lookup"><span data-stu-id="d9f95-141">Last completion time for app sync</span></span>|
|<span data-ttu-id="d9f95-142">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="d9f95-142">lastAppSyncStatus</span></span>|[<span data-ttu-id="d9f95-143">androidManagedStoreAccountAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="d9f95-143">androidManagedStoreAccountAppSyncStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|<span data-ttu-id="d9f95-144">Ergebnis der letzten Anwendungssynchronisierung.</span><span class="sxs-lookup"><span data-stu-id="d9f95-144">Last application sync result.</span></span> <span data-ttu-id="d9f95-145">Mögliche Werte sind: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError` und `none`.</span><span class="sxs-lookup"><span data-stu-id="d9f95-145">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="d9f95-146">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d9f95-146">ownerUserPrincipalName</span></span>|<span data-ttu-id="d9f95-147">String</span><span class="sxs-lookup"><span data-stu-id="d9f95-147">String</span></span>|<span data-ttu-id="d9f95-148">Besitzer-UPN, der das Unternehmen erstellt hat</span><span class="sxs-lookup"><span data-stu-id="d9f95-148">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="d9f95-149">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="d9f95-149">ownerOrganizationName</span></span>|<span data-ttu-id="d9f95-150">String</span><span class="sxs-lookup"><span data-stu-id="d9f95-150">String</span></span>|<span data-ttu-id="d9f95-151">Name der Organisation, die beim Onboarding von Android Enterprise verwendet wird</span><span class="sxs-lookup"><span data-stu-id="d9f95-151">Organization name used when onboarding Android Enterprise</span></span>|
|<span data-ttu-id="d9f95-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9f95-152">lastModifiedDateTime</span></span>|<span data-ttu-id="d9f95-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9f95-153">DateTimeOffset</span></span>|<span data-ttu-id="d9f95-154">Zeitpunkt der letzten Änderung für Android Enterprise-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="d9f95-154">Last modification time for Android enterprise settings</span></span>|
|<span data-ttu-id="d9f95-155">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="d9f95-155">enrollmentTarget</span></span>|[<span data-ttu-id="d9f95-156">androidManagedStoreAccountEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="d9f95-156">androidManagedStoreAccountEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|<span data-ttu-id="d9f95-157">Gibt an, welche Benutzer Geräte in der Android Enterprise-Geräteverwaltung registrieren können.</span><span class="sxs-lookup"><span data-stu-id="d9f95-157">Indicates which users can enroll devices in Android Enterprise device management.</span></span> <span data-ttu-id="d9f95-158">Mögliche Werte sind: `none`, `all`, `targeted` und `targetedAsEnrollmentRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="d9f95-158">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="d9f95-159">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="d9f95-159">targetGroupIds</span></span>|<span data-ttu-id="d9f95-160">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d9f95-160">String collection</span></span>|<span data-ttu-id="d9f95-161">Gibt an, welche AAD-Gruppen Geräte in der Android for Work-Geräteverwaltung registrieren dürfen, wenn die Eigenschaft „enrollmentTarget“ auf „Targeted“ gesetzt ist.</span><span class="sxs-lookup"><span data-stu-id="d9f95-161">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="d9f95-162">deviceOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="d9f95-162">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="d9f95-163">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d9f95-163">Boolean</span></span>|<span data-ttu-id="d9f95-164">Gibt an, ob dieses Konto für die Verwaltung von Android-Geräte Besitzern mit CloudDPC läuft.</span><span class="sxs-lookup"><span data-stu-id="d9f95-164">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|
|<span data-ttu-id="d9f95-165">companyCodes</span><span class="sxs-lookup"><span data-stu-id="d9f95-165">companyCodes</span></span>|<span data-ttu-id="d9f95-166">[androidEnrollmentCompanyCode](../resources/intune-androidforwork-androidenrollmentcompanycode.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="d9f95-166">[androidEnrollmentCompanyCode](../resources/intune-androidforwork-androidenrollmentcompanycode.md) collection</span></span>|<span data-ttu-id="d9f95-167">Buchungskreise für Androidmanagedstoreaccountenterprisesettings hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d9f95-167">Company codes for AndroidManagedStoreAccountEnterpriseSettings</span></span>|
|<span data-ttu-id="d9f95-168">androidDeviceOwnerFullyManagedEnrollmentEnabled</span><span class="sxs-lookup"><span data-stu-id="d9f95-168">androidDeviceOwnerFullyManagedEnrollmentEnabled</span></span>|<span data-ttu-id="d9f95-169">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d9f95-169">Boolean</span></span>|<span data-ttu-id="d9f95-170">Buchungskreise für Androidmanagedstoreaccountenterprisesettings hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="d9f95-170">Company codes for AndroidManagedStoreAccountEnterpriseSettings</span></span>|



## <a name="response"></a><span data-ttu-id="d9f95-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9f95-171">Response</span></span>
<span data-ttu-id="d9f95-172">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [androidmanagedstoreaccountenterprisesettings hinzugefügt](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d9f95-172">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9f95-173">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d9f95-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9f95-174">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9f95-174">Request</span></span>
<span data-ttu-id="d9f95-175">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d9f95-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings
Content-type: application/json
Content-length: 897

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAccountEnterpriseSettings",
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ],
  "deviceOwnerManagementEnabled": true,
  "companyCodes": [
    {
      "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode",
      "enrollmentToken": "Enrollment Token value",
      "qrCodeContent": "Qr Code Content value",
      "qrCodeImage": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      }
    }
  ],
  "androidDeviceOwnerFullyManagedEnrollmentEnabled": true
}
```

### <a name="response"></a><span data-ttu-id="d9f95-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9f95-176">Response</span></span>
<span data-ttu-id="d9f95-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d9f95-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1010

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAccountEnterpriseSettings",
  "id": "b71357c9-57c9-b713-c957-13b7c95713b7",
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ],
  "deviceOwnerManagementEnabled": true,
  "companyCodes": [
    {
      "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode",
      "enrollmentToken": "Enrollment Token value",
      "qrCodeContent": "Qr Code Content value",
      "qrCodeImage": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      }
    }
  ],
  "androidDeviceOwnerFullyManagedEnrollmentEnabled": true
}
```




