---
title: AndroidManagedStoreAccountEnterpriseSettings aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidManagedStoreAccountEnterpriseSettings-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e57b7965e5393faf9bdb953dc915652772deb14c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398485"
---
# <a name="update-androidmanagedstoreaccountenterprisesettings"></a><span data-ttu-id="7ba26-103">AndroidManagedStoreAccountEnterpriseSettings aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7ba26-103">Update androidManagedStoreAccountEnterpriseSettings</span></span>

> <span data-ttu-id="7ba26-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="7ba26-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7ba26-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7ba26-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7ba26-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7ba26-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ba26-107">Aktualisieren Sie die Eigenschaften eines [AndroidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="7ba26-107">Update the properties of a [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ba26-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7ba26-108">Prerequisites</span></span>
<span data-ttu-id="7ba26-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7ba26-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7ba26-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7ba26-111">Permission type</span></span>|<span data-ttu-id="7ba26-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7ba26-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ba26-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7ba26-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7ba26-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ba26-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7ba26-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7ba26-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ba26-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7ba26-116">Not supported.</span></span>|
|<span data-ttu-id="7ba26-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7ba26-117">Application</span></span>|<span data-ttu-id="7ba26-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7ba26-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ba26-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7ba26-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAccountEnterpriseSettings
```

## <a name="request-headers"></a><span data-ttu-id="7ba26-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7ba26-120">Request headers</span></span>
|<span data-ttu-id="7ba26-121">Header</span><span class="sxs-lookup"><span data-stu-id="7ba26-121">Header</span></span>|<span data-ttu-id="7ba26-122">Wert</span><span class="sxs-lookup"><span data-stu-id="7ba26-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ba26-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="7ba26-123">Authorization</span></span>|<span data-ttu-id="7ba26-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7ba26-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ba26-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7ba26-125">Accept</span></span>|<span data-ttu-id="7ba26-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7ba26-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ba26-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7ba26-127">Request body</span></span>
<span data-ttu-id="7ba26-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="7ba26-128">In the request body, supply a JSON representation for the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

<span data-ttu-id="7ba26-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="7ba26-129">The following table shows the properties that are required when you create the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md).</span></span>

|<span data-ttu-id="7ba26-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7ba26-130">Property</span></span>|<span data-ttu-id="7ba26-131">Typ</span><span class="sxs-lookup"><span data-stu-id="7ba26-131">Type</span></span>|<span data-ttu-id="7ba26-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7ba26-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ba26-133">id</span><span class="sxs-lookup"><span data-stu-id="7ba26-133">id</span></span>|<span data-ttu-id="7ba26-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7ba26-134">String</span></span>|<span data-ttu-id="7ba26-135">Die Android Enterprise-Konto-ID Einstellungen speichern</span><span class="sxs-lookup"><span data-stu-id="7ba26-135">The Android store account enterprise settings identifier</span></span>|
|<span data-ttu-id="7ba26-136">bindStatus</span><span class="sxs-lookup"><span data-stu-id="7ba26-136">bindStatus</span></span>|[<span data-ttu-id="7ba26-137">androidManagedStoreAccountBindStatus</span><span class="sxs-lookup"><span data-stu-id="7ba26-137">androidManagedStoreAccountBindStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|<span data-ttu-id="7ba26-138">Status des Mandanten mit der Google EMM-API zu binden.</span><span class="sxs-lookup"><span data-stu-id="7ba26-138">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="7ba26-139">Mögliche Werte: sind `notBound`, `bound`, `boundAndValidated` und `unbinding`.</span><span class="sxs-lookup"><span data-stu-id="7ba26-139">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="7ba26-140">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="7ba26-140">lastAppSyncDateTime</span></span>|<span data-ttu-id="7ba26-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ba26-141">DateTimeOffset</span></span>|<span data-ttu-id="7ba26-142">Zeitpunkt, zu dem zuletzt eine App-Synchronisierung abgeschlossen wurde.</span><span class="sxs-lookup"><span data-stu-id="7ba26-142">Last completion time for app sync</span></span>|
|<span data-ttu-id="7ba26-143">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="7ba26-143">lastAppSyncStatus</span></span>|[<span data-ttu-id="7ba26-144">androidManagedStoreAccountAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="7ba26-144">androidManagedStoreAccountAppSyncStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|<span data-ttu-id="7ba26-145">Letzte Anwendung Sync Ergebnis.</span><span class="sxs-lookup"><span data-stu-id="7ba26-145">Last application sync result.</span></span> <span data-ttu-id="7ba26-146">Mögliche Werte sind: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError` und `none`.</span><span class="sxs-lookup"><span data-stu-id="7ba26-146">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="7ba26-147">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7ba26-147">ownerUserPrincipalName</span></span>|<span data-ttu-id="7ba26-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7ba26-148">String</span></span>|<span data-ttu-id="7ba26-149">Besitzer-UPN, der das Unternehmen erstellt hat</span><span class="sxs-lookup"><span data-stu-id="7ba26-149">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="7ba26-150">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="7ba26-150">ownerOrganizationName</span></span>|<span data-ttu-id="7ba26-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7ba26-151">String</span></span>|<span data-ttu-id="7ba26-152">Name der Organisation verwendet, wenn Onboarding Android Enterprise</span><span class="sxs-lookup"><span data-stu-id="7ba26-152">Organization name used when onboarding Android Enterprise</span></span>|
|<span data-ttu-id="7ba26-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ba26-153">lastModifiedDateTime</span></span>|<span data-ttu-id="7ba26-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ba26-154">DateTimeOffset</span></span>|<span data-ttu-id="7ba26-155">Zeitpunkt der letzten Änderung für Android Enterprise-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="7ba26-155">Last modification time for Android enterprise settings</span></span>|
|<span data-ttu-id="7ba26-156">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="7ba26-156">enrollmentTarget</span></span>|[<span data-ttu-id="7ba26-157">androidManagedStoreAccountEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="7ba26-157">androidManagedStoreAccountEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|<span data-ttu-id="7ba26-158">Gibt an, welche Benutzer Geräte in Android Enterprise Gerätemanagement registrieren können.</span><span class="sxs-lookup"><span data-stu-id="7ba26-158">Indicates which users can enroll devices in Android Enterprise device management.</span></span> <span data-ttu-id="7ba26-159">Mögliche Werte: sind `none`, `all`, `targeted` und `targetedAsEnrollmentRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="7ba26-159">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="7ba26-160">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="7ba26-160">targetGroupIds</span></span>|<span data-ttu-id="7ba26-161">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="7ba26-161">String collection</span></span>|<span data-ttu-id="7ba26-162">Gibt an, welche AAD-Gruppen Geräte in der Android for Work-Geräteverwaltung registrieren dürfen, wenn die Eigenschaft „enrollmentTarget“ auf „Targeted“ gesetzt ist.</span><span class="sxs-lookup"><span data-stu-id="7ba26-162">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="7ba26-163">deviceOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="7ba26-163">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="7ba26-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ba26-164">Boolean</span></span>|<span data-ttu-id="7ba26-165">Gibt an, ob dieses Konto für Android Besitzer Gerätemanagement mit CloudDPC flighting ist.</span><span class="sxs-lookup"><span data-stu-id="7ba26-165">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|
|<span data-ttu-id="7ba26-166">companyCodes</span><span class="sxs-lookup"><span data-stu-id="7ba26-166">companyCodes</span></span>|<span data-ttu-id="7ba26-167">[AndroidEnrollmentCompanyCode](../resources/intune-androidforwork-androidenrollmentcompanycode.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="7ba26-167">[androidEnrollmentCompanyCode](../resources/intune-androidforwork-androidenrollmentcompanycode.md) collection</span></span>|<span data-ttu-id="7ba26-168">Unternehmens-Codes für AndroidManagedStoreAccountEnterpriseSettings</span><span class="sxs-lookup"><span data-stu-id="7ba26-168">Company codes for AndroidManagedStoreAccountEnterpriseSettings</span></span>|
|<span data-ttu-id="7ba26-169">androidDeviceOwnerFullyManagedEnrollmentEnabled</span><span class="sxs-lookup"><span data-stu-id="7ba26-169">androidDeviceOwnerFullyManagedEnrollmentEnabled</span></span>|<span data-ttu-id="7ba26-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ba26-170">Boolean</span></span>|<span data-ttu-id="7ba26-171">Unternehmens-Codes für AndroidManagedStoreAccountEnterpriseSettings</span><span class="sxs-lookup"><span data-stu-id="7ba26-171">Company codes for AndroidManagedStoreAccountEnterpriseSettings</span></span>|



## <a name="response"></a><span data-ttu-id="7ba26-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="7ba26-172">Response</span></span>
<span data-ttu-id="7ba26-173">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="7ba26-173">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ba26-174">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7ba26-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ba26-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7ba26-175">Request</span></span>
<span data-ttu-id="7ba26-176">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7ba26-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7ba26-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="7ba26-177">Response</span></span>
<span data-ttu-id="7ba26-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7ba26-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




