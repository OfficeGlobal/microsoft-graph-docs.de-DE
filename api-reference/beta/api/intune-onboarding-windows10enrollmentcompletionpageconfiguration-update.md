---
title: Windows10EnrollmentCompletionPageConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines windows10EnrollmentCompletionPageConfiguration-Objekts.
author: tfitzmac
ms.openlocfilehash: bcc62cc4bea069a6a29ce2d321578a86145a0446
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360046"
---
# <a name="update-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="ed894-103">Windows10EnrollmentCompletionPageConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ed894-103">Update windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="ed894-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ed894-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed894-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ed894-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed894-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ed894-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed894-107">Aktualisieren Sie die Eigenschaften eines [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ed894-107">Update the properties of a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ed894-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ed894-108">Prerequisites</span></span>
<span data-ttu-id="ed894-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed894-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed894-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ed894-111">Permission type</span></span>|<span data-ttu-id="ed894-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ed894-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed894-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ed894-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ed894-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed894-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ed894-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ed894-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed894-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed894-116">Not supported.</span></span>|
|<span data-ttu-id="ed894-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ed894-117">Application</span></span>|<span data-ttu-id="ed894-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed894-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed894-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed894-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ed894-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ed894-120">Request headers</span></span>
|<span data-ttu-id="ed894-121">Header</span><span class="sxs-lookup"><span data-stu-id="ed894-121">Header</span></span>|<span data-ttu-id="ed894-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ed894-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed894-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="ed894-123">Authorization</span></span>|<span data-ttu-id="ed894-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ed894-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed894-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ed894-125">Accept</span></span>|<span data-ttu-id="ed894-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ed894-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed894-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ed894-127">Request body</span></span>
<span data-ttu-id="ed894-128">Geben Sie im Textkörper Anforderung für das Objekt [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="ed894-128">In the request body, supply a JSON representation for the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

<span data-ttu-id="ed894-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="ed894-129">The following table shows the properties that are required when you create the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span></span>

|<span data-ttu-id="ed894-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ed894-130">Property</span></span>|<span data-ttu-id="ed894-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ed894-131">Type</span></span>|<span data-ttu-id="ed894-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ed894-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed894-133">id</span><span class="sxs-lookup"><span data-stu-id="ed894-133">id</span></span>|<span data-ttu-id="ed894-134">String</span><span class="sxs-lookup"><span data-stu-id="ed894-134">String</span></span>|<span data-ttu-id="ed894-135">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed894-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ed894-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ed894-136">displayName</span></span>|<span data-ttu-id="ed894-137">String</span><span class="sxs-lookup"><span data-stu-id="ed894-137">String</span></span>|<span data-ttu-id="ed894-138">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed894-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ed894-139">description</span><span class="sxs-lookup"><span data-stu-id="ed894-139">description</span></span>|<span data-ttu-id="ed894-140">String</span><span class="sxs-lookup"><span data-stu-id="ed894-140">String</span></span>|<span data-ttu-id="ed894-141">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed894-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ed894-142">Priorität</span><span class="sxs-lookup"><span data-stu-id="ed894-142">priority</span></span>|<span data-ttu-id="ed894-143">Int32</span><span class="sxs-lookup"><span data-stu-id="ed894-143">Int32</span></span>|<span data-ttu-id="ed894-144">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed894-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ed894-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ed894-145">createdDateTime</span></span>|<span data-ttu-id="ed894-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed894-146">DateTimeOffset</span></span>|<span data-ttu-id="ed894-147">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed894-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ed894-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed894-148">lastModifiedDateTime</span></span>|<span data-ttu-id="ed894-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed894-149">DateTimeOffset</span></span>|<span data-ttu-id="ed894-150">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed894-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ed894-151">Version</span><span class="sxs-lookup"><span data-stu-id="ed894-151">version</span></span>|<span data-ttu-id="ed894-152">Int32</span><span class="sxs-lookup"><span data-stu-id="ed894-152">Int32</span></span>|<span data-ttu-id="ed894-153">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed894-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ed894-154">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="ed894-154">showInstallationProgress</span></span>|<span data-ttu-id="ed894-155">Boolesch</span><span class="sxs-lookup"><span data-stu-id="ed894-155">Boolean</span></span>|<span data-ttu-id="ed894-156">Zeigen Sie an oder blenden Sie des installationsfortschritts für Benutzer aus</span><span class="sxs-lookup"><span data-stu-id="ed894-156">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="ed894-157">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="ed894-157">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="ed894-158">Boolesch</span><span class="sxs-lookup"><span data-stu-id="ed894-158">Boolean</span></span>|<span data-ttu-id="ed894-159">Ermöglicht es dem Benutzer, das von Setup auf Installationsfehler wiederholen</span><span class="sxs-lookup"><span data-stu-id="ed894-159">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="ed894-160">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="ed894-160">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="ed894-161">Boolesch</span><span class="sxs-lookup"><span data-stu-id="ed894-161">Boolean</span></span>|<span data-ttu-id="ed894-162">Zulassen Sie oder blockieren Sie Gerät zurücksetzen auf Installationsfehler</span><span class="sxs-lookup"><span data-stu-id="ed894-162">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="ed894-163">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="ed894-163">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="ed894-164">Boolesch</span><span class="sxs-lookup"><span data-stu-id="ed894-164">Boolean</span></span>|<span data-ttu-id="ed894-165">Zulassen Sie oder blockieren Sie Log-Auflistung auf Installationsfehler</span><span class="sxs-lookup"><span data-stu-id="ed894-165">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="ed894-166">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="ed894-166">customErrorMessage</span></span>|<span data-ttu-id="ed894-167">String</span><span class="sxs-lookup"><span data-stu-id="ed894-167">String</span></span>|<span data-ttu-id="ed894-168">Legen Sie benutzerdefinierte Fehlermeldung nach einem Installationsfehler anzeigen</span><span class="sxs-lookup"><span data-stu-id="ed894-168">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="ed894-169">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="ed894-169">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="ed894-170">Int32</span><span class="sxs-lookup"><span data-stu-id="ed894-170">Int32</span></span>|<span data-ttu-id="ed894-171">Legen Sie die Installation des Fortschritts Timeout in Minuten</span><span class="sxs-lookup"><span data-stu-id="ed894-171">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="ed894-172">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="ed894-172">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="ed894-173">Boolesch</span><span class="sxs-lookup"><span data-stu-id="ed894-173">Boolean</span></span>|<span data-ttu-id="ed894-174">Ermöglicht es dem Benutzer weiterhin verwenden das Gerät auf Installationsfehler</span><span class="sxs-lookup"><span data-stu-id="ed894-174">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="ed894-175">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="ed894-175">selectedMobileAppIds</span></span>|<span data-ttu-id="ed894-176">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="ed894-176">String collection</span></span>|<span data-ttu-id="ed894-177">Ausgewählte Anwendungen zum Nachverfolgen des Installationsstatus</span><span class="sxs-lookup"><span data-stu-id="ed894-177">Selected applications to track the installation status</span></span>|



## <a name="response"></a><span data-ttu-id="ed894-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed894-178">Response</span></span>
<span data-ttu-id="ed894-179">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ed894-179">If successful, this method returns a `200 OK` response code and an updated [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed894-180">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ed894-180">Example</span></span>
### <a name="request"></a><span data-ttu-id="ed894-181">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed894-181">Request</span></span>
<span data-ttu-id="ed894-182">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ed894-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 562

{
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "showInstallationProgress": true,
  "blockDeviceSetupRetryByUser": true,
  "allowDeviceResetOnInstallFailure": true,
  "allowLogCollectionOnInstallFailure": true,
  "customErrorMessage": "Custom Error Message value",
  "installProgressTimeoutInMinutes": 15,
  "allowDeviceUseOnInstallFailure": true,
  "selectedMobileAppIds": [
    "Selected Mobile App Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="ed894-183">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed894-183">Response</span></span>
<span data-ttu-id="ed894-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ed894-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 755

{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
  "id": "77bf8248-8248-77bf-4882-bf774882bf77",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "showInstallationProgress": true,
  "blockDeviceSetupRetryByUser": true,
  "allowDeviceResetOnInstallFailure": true,
  "allowLogCollectionOnInstallFailure": true,
  "customErrorMessage": "Custom Error Message value",
  "installProgressTimeoutInMinutes": 15,
  "allowDeviceUseOnInstallFailure": true,
  "selectedMobileAppIds": [
    "Selected Mobile App Ids value"
  ]
}
```





