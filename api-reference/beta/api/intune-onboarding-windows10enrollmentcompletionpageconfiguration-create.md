---
title: Windows10EnrollmentCompletionPageConfiguration erstellen
description: Erstellen eines neuen windows10EnrollmentCompletionPageConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0018e99738e09317835af3fe79505c9723c5e6a5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140292"
---
# <a name="create-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="f1108-103">Windows10EnrollmentCompletionPageConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="f1108-103">Create windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="f1108-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f1108-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1108-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f1108-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1108-106">Erstellen eines neuen [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f1108-106">Create a new [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1108-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f1108-107">Prerequisites</span></span>
<span data-ttu-id="f1108-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f1108-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f1108-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f1108-110">Permission type</span></span>|<span data-ttu-id="f1108-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f1108-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1108-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f1108-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f1108-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1108-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f1108-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f1108-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1108-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f1108-115">Not supported.</span></span>|
|<span data-ttu-id="f1108-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f1108-116">Application</span></span>|<span data-ttu-id="f1108-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f1108-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1108-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1108-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f1108-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f1108-119">Request headers</span></span>
|<span data-ttu-id="f1108-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f1108-120">Header</span></span>|<span data-ttu-id="f1108-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f1108-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1108-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1108-122">Authorization</span></span>|<span data-ttu-id="f1108-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f1108-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1108-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f1108-124">Accept</span></span>|<span data-ttu-id="f1108-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f1108-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1108-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f1108-126">Request body</span></span>
<span data-ttu-id="f1108-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das windows10EnrollmentCompletionPageConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="f1108-127">In the request body, supply a JSON representation for the windows10EnrollmentCompletionPageConfiguration object.</span></span>

<span data-ttu-id="f1108-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windows10EnrollmentCompletionPageConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="f1108-128">The following table shows the properties that are required when you create the windows10EnrollmentCompletionPageConfiguration.</span></span>

|<span data-ttu-id="f1108-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f1108-129">Property</span></span>|<span data-ttu-id="f1108-130">Typ</span><span class="sxs-lookup"><span data-stu-id="f1108-130">Type</span></span>|<span data-ttu-id="f1108-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f1108-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1108-132">id</span><span class="sxs-lookup"><span data-stu-id="f1108-132">id</span></span>|<span data-ttu-id="f1108-133">string</span><span class="sxs-lookup"><span data-stu-id="f1108-133">String</span></span>|<span data-ttu-id="f1108-134">ID der von [DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) geerbten Konfiguration der Registrierungs Status Seite</span><span class="sxs-lookup"><span data-stu-id="f1108-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f1108-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f1108-135">displayName</span></span>|<span data-ttu-id="f1108-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f1108-136">String</span></span>|<span data-ttu-id="f1108-137">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1108-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f1108-138">description</span><span class="sxs-lookup"><span data-stu-id="f1108-138">description</span></span>|<span data-ttu-id="f1108-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f1108-139">String</span></span>|<span data-ttu-id="f1108-140">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1108-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f1108-141">Priorität</span><span class="sxs-lookup"><span data-stu-id="f1108-141">priority</span></span>|<span data-ttu-id="f1108-142">Int32</span><span class="sxs-lookup"><span data-stu-id="f1108-142">Int32</span></span>|<span data-ttu-id="f1108-143">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1108-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f1108-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f1108-144">createdDateTime</span></span>|<span data-ttu-id="f1108-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1108-145">DateTimeOffset</span></span>|<span data-ttu-id="f1108-146">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1108-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f1108-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1108-147">lastModifiedDateTime</span></span>|<span data-ttu-id="f1108-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1108-148">DateTimeOffset</span></span>|<span data-ttu-id="f1108-149">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1108-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f1108-150">Version</span><span class="sxs-lookup"><span data-stu-id="f1108-150">version</span></span>|<span data-ttu-id="f1108-151">Int32</span><span class="sxs-lookup"><span data-stu-id="f1108-151">Int32</span></span>|<span data-ttu-id="f1108-152">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1108-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f1108-153">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="f1108-153">showInstallationProgress</span></span>|<span data-ttu-id="f1108-154">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f1108-154">Boolean</span></span>|<span data-ttu-id="f1108-155">Anzeigen oder Ausblenden des Installationsfortschritts für den Benutzer</span><span class="sxs-lookup"><span data-stu-id="f1108-155">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="f1108-156">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="f1108-156">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="f1108-157">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f1108-157">Boolean</span></span>|<span data-ttu-id="f1108-158">Wiederholen des Setups bei Installationsfehlers für den Benutzer</span><span class="sxs-lookup"><span data-stu-id="f1108-158">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="f1108-159">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="f1108-159">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="f1108-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f1108-160">Boolean</span></span>|<span data-ttu-id="f1108-161">Gerätezurücksetzung bei Installationsfehlers zulassen oder blockieren</span><span class="sxs-lookup"><span data-stu-id="f1108-161">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="f1108-162">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="f1108-162">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="f1108-163">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f1108-163">Boolean</span></span>|<span data-ttu-id="f1108-164">Zulassen oder Blockieren der Protokollsammlung bei Installations Ausfällen</span><span class="sxs-lookup"><span data-stu-id="f1108-164">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="f1108-165">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="f1108-165">customErrorMessage</span></span>|<span data-ttu-id="f1108-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f1108-166">String</span></span>|<span data-ttu-id="f1108-167">Festlegen der benutzerdefinierten Fehlermeldung beim Installationsfehler</span><span class="sxs-lookup"><span data-stu-id="f1108-167">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="f1108-168">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="f1108-168">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="f1108-169">Int32</span><span class="sxs-lookup"><span data-stu-id="f1108-169">Int32</span></span>|<span data-ttu-id="f1108-170">Festlegen des Installationsfortschritts-Timeouts in Minuten</span><span class="sxs-lookup"><span data-stu-id="f1108-170">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="f1108-171">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="f1108-171">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="f1108-172">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f1108-172">Boolean</span></span>|<span data-ttu-id="f1108-173">Zulassen, dass der Benutzer das Gerät bei der Installation weiterhin verwendet</span><span class="sxs-lookup"><span data-stu-id="f1108-173">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="f1108-174">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="f1108-174">selectedMobileAppIds</span></span>|<span data-ttu-id="f1108-175">String collection</span><span class="sxs-lookup"><span data-stu-id="f1108-175">String collection</span></span>|<span data-ttu-id="f1108-176">Ausgewählte Anwendungen zum Nachverfolgen des Installationsstatus</span><span class="sxs-lookup"><span data-stu-id="f1108-176">Selected applications to track the installation status</span></span>|



## <a name="response"></a><span data-ttu-id="f1108-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1108-177">Response</span></span>
<span data-ttu-id="f1108-178">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f1108-178">If successful, this method returns a `201 Created` response code and a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1108-179">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f1108-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1108-180">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1108-180">Request</span></span>
<span data-ttu-id="f1108-181">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f1108-181">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="f1108-182">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1108-182">Response</span></span>
<span data-ttu-id="f1108-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f1108-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




