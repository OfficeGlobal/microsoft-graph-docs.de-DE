---
title: Erstellen von windows10EnrollmentCompletionPageConfiguration
description: Erstellen eines neuen windows10EnrollmentCompletionPageConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: aa459255e48323c5f4e614dc9d12f8ae89d2f4e4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862727"
---
# <a name="create-windows10enrollmentcompletionpageconfiguration"></a><span data-ttu-id="d6df4-103">Erstellen von windows10EnrollmentCompletionPageConfiguration</span><span class="sxs-lookup"><span data-stu-id="d6df4-103">Create windows10EnrollmentCompletionPageConfiguration</span></span>

> <span data-ttu-id="d6df4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d6df4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6df4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d6df4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6df4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d6df4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6df4-107">Erstellen eines neuen [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d6df4-107">Create a new [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d6df4-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d6df4-108">Prerequisites</span></span>
<span data-ttu-id="d6df4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6df4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6df4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d6df4-111">Permission type</span></span>|<span data-ttu-id="d6df4-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d6df4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6df4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d6df4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d6df4-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6df4-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d6df4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d6df4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6df4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d6df4-116">Not supported.</span></span>|
|<span data-ttu-id="d6df4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d6df4-117">Application</span></span>|<span data-ttu-id="d6df4-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d6df4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6df4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d6df4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d6df4-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d6df4-120">Request headers</span></span>
|<span data-ttu-id="d6df4-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d6df4-121">Header</span></span>|<span data-ttu-id="d6df4-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d6df4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6df4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6df4-123">Authorization</span></span>|<span data-ttu-id="d6df4-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d6df4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6df4-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d6df4-125">Accept</span></span>|<span data-ttu-id="d6df4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6df4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6df4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d6df4-127">Request body</span></span>
<span data-ttu-id="d6df4-128">Geben Sie im Textkörper Anforderung für das Objekt windows10EnrollmentCompletionPageConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="d6df4-128">In the request body, supply a JSON representation for the windows10EnrollmentCompletionPageConfiguration object.</span></span>

<span data-ttu-id="d6df4-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die windows10EnrollmentCompletionPageConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="d6df4-129">The following table shows the properties that are required when you create the windows10EnrollmentCompletionPageConfiguration.</span></span>

|<span data-ttu-id="d6df4-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d6df4-130">Property</span></span>|<span data-ttu-id="d6df4-131">Typ</span><span class="sxs-lookup"><span data-stu-id="d6df4-131">Type</span></span>|<span data-ttu-id="d6df4-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d6df4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6df4-133">id</span><span class="sxs-lookup"><span data-stu-id="d6df4-133">id</span></span>|<span data-ttu-id="d6df4-134">String</span><span class="sxs-lookup"><span data-stu-id="d6df4-134">String</span></span>|<span data-ttu-id="d6df4-135">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6df4-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d6df4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d6df4-136">displayName</span></span>|<span data-ttu-id="d6df4-137">String</span><span class="sxs-lookup"><span data-stu-id="d6df4-137">String</span></span>|<span data-ttu-id="d6df4-138">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6df4-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d6df4-139">description</span><span class="sxs-lookup"><span data-stu-id="d6df4-139">description</span></span>|<span data-ttu-id="d6df4-140">String</span><span class="sxs-lookup"><span data-stu-id="d6df4-140">String</span></span>|<span data-ttu-id="d6df4-141">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6df4-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d6df4-142">Priorität</span><span class="sxs-lookup"><span data-stu-id="d6df4-142">priority</span></span>|<span data-ttu-id="d6df4-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d6df4-143">Int32</span></span>|<span data-ttu-id="d6df4-144">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6df4-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d6df4-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d6df4-145">createdDateTime</span></span>|<span data-ttu-id="d6df4-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6df4-146">DateTimeOffset</span></span>|<span data-ttu-id="d6df4-147">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6df4-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d6df4-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6df4-148">lastModifiedDateTime</span></span>|<span data-ttu-id="d6df4-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6df4-149">DateTimeOffset</span></span>|<span data-ttu-id="d6df4-150">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6df4-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d6df4-151">Version</span><span class="sxs-lookup"><span data-stu-id="d6df4-151">version</span></span>|<span data-ttu-id="d6df4-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d6df4-152">Int32</span></span>|<span data-ttu-id="d6df4-153">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6df4-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d6df4-154">showInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="d6df4-154">showInstallationProgress</span></span>|<span data-ttu-id="d6df4-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6df4-155">Boolean</span></span>|<span data-ttu-id="d6df4-156">Zeigen Sie an oder blenden Sie des installationsfortschritts für Benutzer aus</span><span class="sxs-lookup"><span data-stu-id="d6df4-156">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="d6df4-157">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="d6df4-157">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="d6df4-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6df4-158">Boolean</span></span>|<span data-ttu-id="d6df4-159">Ermöglicht es dem Benutzer, das von Setup auf Installationsfehler wiederholen</span><span class="sxs-lookup"><span data-stu-id="d6df4-159">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="d6df4-160">allowDeviceResetOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="d6df4-160">allowDeviceResetOnInstallFailure</span></span>|<span data-ttu-id="d6df4-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6df4-161">Boolean</span></span>|<span data-ttu-id="d6df4-162">Zulassen Sie oder blockieren Sie Gerät zurücksetzen auf Installationsfehler</span><span class="sxs-lookup"><span data-stu-id="d6df4-162">Allow or block device reset on installation failure</span></span>|
|<span data-ttu-id="d6df4-163">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="d6df4-163">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="d6df4-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6df4-164">Boolean</span></span>|<span data-ttu-id="d6df4-165">Zulassen Sie oder blockieren Sie Log-Auflistung auf Installationsfehler</span><span class="sxs-lookup"><span data-stu-id="d6df4-165">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="d6df4-166">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="d6df4-166">customErrorMessage</span></span>|<span data-ttu-id="d6df4-167">String</span><span class="sxs-lookup"><span data-stu-id="d6df4-167">String</span></span>|<span data-ttu-id="d6df4-168">Legen Sie benutzerdefinierte Fehlermeldung nach einem Installationsfehler anzeigen</span><span class="sxs-lookup"><span data-stu-id="d6df4-168">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="d6df4-169">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="d6df4-169">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="d6df4-170">Int32</span><span class="sxs-lookup"><span data-stu-id="d6df4-170">Int32</span></span>|<span data-ttu-id="d6df4-171">Legen Sie die Installation des Fortschritts Timeout in Minuten</span><span class="sxs-lookup"><span data-stu-id="d6df4-171">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="d6df4-172">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="d6df4-172">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="d6df4-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6df4-173">Boolean</span></span>|<span data-ttu-id="d6df4-174">Ermöglicht es dem Benutzer weiterhin verwenden das Gerät auf Installationsfehler</span><span class="sxs-lookup"><span data-stu-id="d6df4-174">Allow the user to continue using the device on installation failure</span></span>|
|<span data-ttu-id="d6df4-175">selectedMobileAppIds</span><span class="sxs-lookup"><span data-stu-id="d6df4-175">selectedMobileAppIds</span></span>|<span data-ttu-id="d6df4-176">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="d6df4-176">String collection</span></span>|<span data-ttu-id="d6df4-177">Ausgewählte Anwendungen zum Nachverfolgen des Installationsstatus</span><span class="sxs-lookup"><span data-stu-id="d6df4-177">Selected applications to track the installation status</span></span>|



## <a name="response"></a><span data-ttu-id="d6df4-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="d6df4-178">Response</span></span>
<span data-ttu-id="d6df4-179">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d6df4-179">If successful, this method returns a `201 Created` response code and a [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6df4-180">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d6df4-180">Example</span></span>
### <a name="request"></a><span data-ttu-id="d6df4-181">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d6df4-181">Request</span></span>
<span data-ttu-id="d6df4-182">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d6df4-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 647

{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
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

### <a name="response"></a><span data-ttu-id="d6df4-183">Antwort</span><span class="sxs-lookup"><span data-stu-id="d6df4-183">Response</span></span>
<span data-ttu-id="d6df4-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d6df4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





