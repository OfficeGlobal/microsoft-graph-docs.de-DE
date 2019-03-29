---
title: Windows10EnrollmentCompletionPageConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines windows10EnrollmentCompletionPageConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 862ec01be1bd6b99351d9b01f16797ae4a376e75
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30981132"
---
# <a name="update-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="097d1-103">Windows10EnrollmentCompletionPageConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="097d1-103">Update windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="097d1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="097d1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="097d1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="097d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="097d1-106">Aktualisieren der Eigenschaften eines [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="097d1-106">Update the properties of a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="097d1-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="097d1-107">Prerequisites</span></span>
<span data-ttu-id="097d1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="097d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="097d1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="097d1-110">Permission type</span></span>|<span data-ttu-id="097d1-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="097d1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="097d1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="097d1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="097d1-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="097d1-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="097d1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="097d1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="097d1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="097d1-115">Not supported.</span></span>|
|<span data-ttu-id="097d1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="097d1-116">Application</span></span>|<span data-ttu-id="097d1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="097d1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="097d1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="097d1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="097d1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="097d1-119">Request headers</span></span>
|<span data-ttu-id="097d1-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="097d1-120">Header</span></span>|<span data-ttu-id="097d1-121">Wert</span><span class="sxs-lookup"><span data-stu-id="097d1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="097d1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="097d1-122">Authorization</span></span>|<span data-ttu-id="097d1-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="097d1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="097d1-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="097d1-124">Accept</span></span>|<span data-ttu-id="097d1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="097d1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="097d1-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="097d1-126">Request body</span></span>
<span data-ttu-id="097d1-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="097d1-127">In the request body, supply a JSON representation for the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

<span data-ttu-id="097d1-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="097d1-128">The following table shows the properties that are required when you create the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).</span></span>

|<span data-ttu-id="097d1-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="097d1-129">Property</span></span>|<span data-ttu-id="097d1-130">Typ</span><span class="sxs-lookup"><span data-stu-id="097d1-130">Type</span></span>|<span data-ttu-id="097d1-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="097d1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="097d1-132">id</span><span class="sxs-lookup"><span data-stu-id="097d1-132">id</span></span>|<span data-ttu-id="097d1-133">String</span><span class="sxs-lookup"><span data-stu-id="097d1-133">String</span></span>|<span data-ttu-id="097d1-134">ID der von [DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) geerbten Konfiguration der Registrierungs Status Seite</span><span class="sxs-lookup"><span data-stu-id="097d1-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="097d1-135">displayName</span><span class="sxs-lookup"><span data-stu-id="097d1-135">displayName</span></span>|<span data-ttu-id="097d1-136">String</span><span class="sxs-lookup"><span data-stu-id="097d1-136">String</span></span>|<span data-ttu-id="097d1-137">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="097d1-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="097d1-138">description</span><span class="sxs-lookup"><span data-stu-id="097d1-138">description</span></span>|<span data-ttu-id="097d1-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="097d1-139">String</span></span>|<span data-ttu-id="097d1-140">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="097d1-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="097d1-141">Priorität</span><span class="sxs-lookup"><span data-stu-id="097d1-141">priority</span></span>|<span data-ttu-id="097d1-142">Int32</span><span class="sxs-lookup"><span data-stu-id="097d1-142">Int32</span></span>|<span data-ttu-id="097d1-143">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="097d1-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="097d1-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="097d1-144">createdDateTime</span></span>|<span data-ttu-id="097d1-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="097d1-145">DateTimeOffset</span></span>|<span data-ttu-id="097d1-146">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="097d1-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="097d1-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="097d1-147">lastModifiedDateTime</span></span>|<span data-ttu-id="097d1-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="097d1-148">DateTimeOffset</span></span>|<span data-ttu-id="097d1-149">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="097d1-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="097d1-150">Version</span><span class="sxs-lookup"><span data-stu-id="097d1-150">version</span></span>|<span data-ttu-id="097d1-151">Int32</span><span class="sxs-lookup"><span data-stu-id="097d1-151">Int32</span></span>|<span data-ttu-id="097d1-152">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="097d1-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="097d1-153">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="097d1-153">showInstallationProgress</span></span>|<span data-ttu-id="097d1-154">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="097d1-154">Boolean</span></span>|<span data-ttu-id="097d1-155">Anzeigen oder Ausblenden des Installationsfortschritts für den Benutzer</span><span class="sxs-lookup"><span data-stu-id="097d1-155">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="097d1-156">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="097d1-156">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="097d1-157">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="097d1-157">Boolean</span></span>|<span data-ttu-id="097d1-158">Wiederholen des Setups bei Installationsfehlers für den Benutzer</span><span class="sxs-lookup"><span data-stu-id="097d1-158">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="097d1-159">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="097d1-159">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="097d1-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="097d1-160">Boolean</span></span>|<span data-ttu-id="097d1-161">Gerätezurücksetzung bei Installationsfehlers zulassen oder blockieren</span><span class="sxs-lookup"><span data-stu-id="097d1-161">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="097d1-162">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="097d1-162">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="097d1-163">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="097d1-163">Boolean</span></span>|<span data-ttu-id="097d1-164">Zulassen oder Blockieren der Protokollsammlung bei Installations Ausfällen</span><span class="sxs-lookup"><span data-stu-id="097d1-164">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="097d1-165">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="097d1-165">customErrorMessage</span></span>|<span data-ttu-id="097d1-166">String</span><span class="sxs-lookup"><span data-stu-id="097d1-166">String</span></span>|<span data-ttu-id="097d1-167">Festlegen der benutzerdefinierten Fehlermeldung beim Installationsfehler</span><span class="sxs-lookup"><span data-stu-id="097d1-167">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="097d1-168">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="097d1-168">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="097d1-169">Int32</span><span class="sxs-lookup"><span data-stu-id="097d1-169">Int32</span></span>|<span data-ttu-id="097d1-170">Festlegen des Installationsfortschritts-Timeouts in Minuten</span><span class="sxs-lookup"><span data-stu-id="097d1-170">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="097d1-171">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="097d1-171">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="097d1-172">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="097d1-172">Boolean</span></span>|<span data-ttu-id="097d1-173">Zulassen, dass der Benutzer das Gerät bei der Installation weiterhin verwendet</span><span class="sxs-lookup"><span data-stu-id="097d1-173">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="097d1-174">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="097d1-174">selectedMobileAppIds</span></span>|<span data-ttu-id="097d1-175">String collection</span><span class="sxs-lookup"><span data-stu-id="097d1-175">String collection</span></span>|<span data-ttu-id="097d1-176">Ausgewählte Anwendungen zum Nachverfolgen des Installationsstatus</span><span class="sxs-lookup"><span data-stu-id="097d1-176">Selected applications to track the installation status</span></span>|



## <a name="response"></a><span data-ttu-id="097d1-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="097d1-177">Response</span></span>
<span data-ttu-id="097d1-178">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="097d1-178">If successful, this method returns a `200 OK` response code and an updated [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="097d1-179">Beispiel</span><span class="sxs-lookup"><span data-stu-id="097d1-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="097d1-180">Anforderung</span><span class="sxs-lookup"><span data-stu-id="097d1-180">Request</span></span>
<span data-ttu-id="097d1-181">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="097d1-181">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 583

{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
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

### <a name="response"></a><span data-ttu-id="097d1-182">Antwort</span><span class="sxs-lookup"><span data-stu-id="097d1-182">Response</span></span>
<span data-ttu-id="097d1-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="097d1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




