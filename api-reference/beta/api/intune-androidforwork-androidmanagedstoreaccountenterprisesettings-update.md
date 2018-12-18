---
title: AndroidManagedStoreAccountEnterpriseSettings aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidManagedStoreAccountEnterpriseSettings-Objekts.
author: tfitzmac
ms.openlocfilehash: ee5fda9e9c6ce92cdf44ec878c2c5835ceed2c49
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356028"
---
# <a name="update-androidmanagedstoreaccountenterprisesettings"></a><span data-ttu-id="d79d7-103">AndroidManagedStoreAccountEnterpriseSettings aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d79d7-103">Update androidManagedStoreAccountEnterpriseSettings</span></span>

> <span data-ttu-id="d79d7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d79d7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d79d7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d79d7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d79d7-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d79d7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d79d7-107">Aktualisieren Sie die Eigenschaften eines [AndroidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d79d7-107">Update the properties of a [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d79d7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d79d7-108">Prerequisites</span></span>
<span data-ttu-id="d79d7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d79d7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d79d7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d79d7-111">Permission type</span></span>|<span data-ttu-id="d79d7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d79d7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d79d7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d79d7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d79d7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d79d7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d79d7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d79d7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d79d7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d79d7-116">Not supported.</span></span>|
|<span data-ttu-id="d79d7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d79d7-117">Application</span></span>|<span data-ttu-id="d79d7-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d79d7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d79d7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d79d7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAccountEnterpriseSettings
```

## <a name="request-headers"></a><span data-ttu-id="d79d7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d79d7-120">Request headers</span></span>
|<span data-ttu-id="d79d7-121">Header</span><span class="sxs-lookup"><span data-stu-id="d79d7-121">Header</span></span>|<span data-ttu-id="d79d7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d79d7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d79d7-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d79d7-123">Authorization</span></span>|<span data-ttu-id="d79d7-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d79d7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d79d7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d79d7-125">Accept</span></span>|<span data-ttu-id="d79d7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d79d7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d79d7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d79d7-127">Request body</span></span>
<span data-ttu-id="d79d7-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="d79d7-128">In the request body, supply a JSON representation for the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

<span data-ttu-id="d79d7-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="d79d7-129">The following table shows the properties that are required when you create the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md).</span></span>

|<span data-ttu-id="d79d7-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d79d7-130">Property</span></span>|<span data-ttu-id="d79d7-131">Typ</span><span class="sxs-lookup"><span data-stu-id="d79d7-131">Type</span></span>|<span data-ttu-id="d79d7-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d79d7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d79d7-133">id</span><span class="sxs-lookup"><span data-stu-id="d79d7-133">id</span></span>|<span data-ttu-id="d79d7-134">String</span><span class="sxs-lookup"><span data-stu-id="d79d7-134">String</span></span>|<span data-ttu-id="d79d7-135">Die Android Enterprise-Konto-ID Einstellungen speichern</span><span class="sxs-lookup"><span data-stu-id="d79d7-135">The Android store account enterprise settings identifier</span></span>|
|<span data-ttu-id="d79d7-136">bindStatus</span><span class="sxs-lookup"><span data-stu-id="d79d7-136">bindStatus</span></span>|[<span data-ttu-id="d79d7-137">androidManagedStoreAccountBindStatus</span><span class="sxs-lookup"><span data-stu-id="d79d7-137">androidManagedStoreAccountBindStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|<span data-ttu-id="d79d7-138">Status des Mandanten mit der Google EMM-API zu binden.</span><span class="sxs-lookup"><span data-stu-id="d79d7-138">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="d79d7-139">Mögliche Werte: sind `notBound`, `bound`, `boundAndValidated` und `unbinding`.</span><span class="sxs-lookup"><span data-stu-id="d79d7-139">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="d79d7-140">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d79d7-140">lastAppSyncDateTime</span></span>|<span data-ttu-id="d79d7-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d79d7-141">DateTimeOffset</span></span>|<span data-ttu-id="d79d7-142">Zeitpunkt, zu dem zuletzt eine App-Synchronisierung abgeschlossen wurde.</span><span class="sxs-lookup"><span data-stu-id="d79d7-142">Last completion time for app sync</span></span>|
|<span data-ttu-id="d79d7-143">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="d79d7-143">lastAppSyncStatus</span></span>|[<span data-ttu-id="d79d7-144">androidManagedStoreAccountAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="d79d7-144">androidManagedStoreAccountAppSyncStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|<span data-ttu-id="d79d7-145">Letzte Anwendung Sync Ergebnis.</span><span class="sxs-lookup"><span data-stu-id="d79d7-145">Last application sync result.</span></span> <span data-ttu-id="d79d7-146">Mögliche Werte sind: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError` und `none`.</span><span class="sxs-lookup"><span data-stu-id="d79d7-146">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="d79d7-147">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d79d7-147">ownerUserPrincipalName</span></span>|<span data-ttu-id="d79d7-148">String</span><span class="sxs-lookup"><span data-stu-id="d79d7-148">String</span></span>|<span data-ttu-id="d79d7-149">Besitzer-UPN, der das Unternehmen erstellt hat</span><span class="sxs-lookup"><span data-stu-id="d79d7-149">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="d79d7-150">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="d79d7-150">ownerOrganizationName</span></span>|<span data-ttu-id="d79d7-151">String</span><span class="sxs-lookup"><span data-stu-id="d79d7-151">String</span></span>|<span data-ttu-id="d79d7-152">Name der Organisation verwendet, wenn Onboarding Android Enterprise</span><span class="sxs-lookup"><span data-stu-id="d79d7-152">Organization name used when onboarding Android Enterprise</span></span>|
|<span data-ttu-id="d79d7-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d79d7-153">lastModifiedDateTime</span></span>|<span data-ttu-id="d79d7-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d79d7-154">DateTimeOffset</span></span>|<span data-ttu-id="d79d7-155">Zeitpunkt der letzten Änderung für Android Enterprise-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="d79d7-155">Last modification time for Android enterprise settings</span></span>|
|<span data-ttu-id="d79d7-156">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="d79d7-156">enrollmentTarget</span></span>|[<span data-ttu-id="d79d7-157">androidManagedStoreAccountEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="d79d7-157">androidManagedStoreAccountEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|<span data-ttu-id="d79d7-158">Gibt an, welche Benutzer Geräte in Android Enterprise Gerätemanagement registrieren können.</span><span class="sxs-lookup"><span data-stu-id="d79d7-158">Indicates which users can enroll devices in Android Enterprise device management.</span></span> <span data-ttu-id="d79d7-159">Mögliche Werte: sind `none`, `all`, `targeted` und `targetedAsEnrollmentRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="d79d7-159">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="d79d7-160">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="d79d7-160">targetGroupIds</span></span>|<span data-ttu-id="d79d7-161">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="d79d7-161">String collection</span></span>|<span data-ttu-id="d79d7-162">Gibt an, welche AAD-Gruppen Geräte in der Android for Work-Geräteverwaltung registrieren dürfen, wenn die Eigenschaft „enrollmentTarget“ auf „Targeted“ gesetzt ist.</span><span class="sxs-lookup"><span data-stu-id="d79d7-162">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="d79d7-163">deviceOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="d79d7-163">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="d79d7-164">Boolesch</span><span class="sxs-lookup"><span data-stu-id="d79d7-164">Boolean</span></span>|<span data-ttu-id="d79d7-165">Gibt an, ob dieses Konto für Android Besitzer Gerätemanagement mit CloudDPC flighting ist.</span><span class="sxs-lookup"><span data-stu-id="d79d7-165">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|



## <a name="response"></a><span data-ttu-id="d79d7-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="d79d7-166">Response</span></span>
<span data-ttu-id="d79d7-167">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d79d7-167">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d79d7-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d79d7-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="d79d7-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d79d7-169">Request</span></span>
<span data-ttu-id="d79d7-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d79d7-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings
Content-type: application/json
Content-length: 458

{
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
  "deviceOwnerManagementEnabled": true
}
```

### <a name="response"></a><span data-ttu-id="d79d7-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="d79d7-171">Response</span></span>
<span data-ttu-id="d79d7-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d79d7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 590

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
  "deviceOwnerManagementEnabled": true
}
```





