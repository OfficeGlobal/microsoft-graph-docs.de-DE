---
title: Erstellen von „windows10SecureAssessmentConfiguration“
description: Erstellen eines neuen windows10SecureAssessmentConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c0e8b430023563ddb770b2cf7d4693814f01b4a7
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252273"
---
# <a name="create-windows10secureassessmentconfiguration"></a><span data-ttu-id="3292e-103">Erstellen von „windows10SecureAssessmentConfiguration“</span><span class="sxs-lookup"><span data-stu-id="3292e-103">Create windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="3292e-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3292e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3292e-105">Erstellen eines neuen [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3292e-105">Create a new [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3292e-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3292e-106">Prerequisites</span></span>
<span data-ttu-id="3292e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3292e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3292e-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3292e-109">Permission type</span></span>|<span data-ttu-id="3292e-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3292e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3292e-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3292e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3292e-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3292e-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3292e-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3292e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3292e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3292e-114">Not supported.</span></span>|
|<span data-ttu-id="3292e-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3292e-115">Application</span></span>|<span data-ttu-id="3292e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3292e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3292e-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3292e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3292e-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3292e-118">Request headers</span></span>
|<span data-ttu-id="3292e-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3292e-119">Header</span></span>|<span data-ttu-id="3292e-120">Wert</span><span class="sxs-lookup"><span data-stu-id="3292e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3292e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3292e-121">Authorization</span></span>|<span data-ttu-id="3292e-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3292e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3292e-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3292e-123">Accept</span></span>|<span data-ttu-id="3292e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3292e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3292e-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3292e-125">Request body</span></span>
<span data-ttu-id="3292e-126">Geben Sie im Anforderungstext eine JSON-Darstellung des windows10SecureAssessmentConfiguration-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="3292e-126">In the request body, supply a JSON representation for the windows10SecureAssessmentConfiguration object.</span></span>

<span data-ttu-id="3292e-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windows10SecureAssessmentConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="3292e-127">The following table shows the properties that are required when you create the windows10SecureAssessmentConfiguration.</span></span>

|<span data-ttu-id="3292e-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3292e-128">Property</span></span>|<span data-ttu-id="3292e-129">Typ</span><span class="sxs-lookup"><span data-stu-id="3292e-129">Type</span></span>|<span data-ttu-id="3292e-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3292e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3292e-131">id</span><span class="sxs-lookup"><span data-stu-id="3292e-131">id</span></span>|<span data-ttu-id="3292e-132">string</span><span class="sxs-lookup"><span data-stu-id="3292e-132">String</span></span>|<span data-ttu-id="3292e-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="3292e-133">Key of the entity.</span></span> <span data-ttu-id="3292e-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3292e-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3292e-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3292e-135">lastModifiedDateTime</span></span>|<span data-ttu-id="3292e-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3292e-136">DateTimeOffset</span></span>|<span data-ttu-id="3292e-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="3292e-137">DateTime the object was last modified.</span></span> <span data-ttu-id="3292e-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3292e-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3292e-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3292e-139">createdDateTime</span></span>|<span data-ttu-id="3292e-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3292e-140">DateTimeOffset</span></span>|<span data-ttu-id="3292e-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="3292e-141">DateTime the object was created.</span></span> <span data-ttu-id="3292e-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3292e-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3292e-143">description</span><span class="sxs-lookup"><span data-stu-id="3292e-143">description</span></span>|<span data-ttu-id="3292e-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3292e-144">String</span></span>|<span data-ttu-id="3292e-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="3292e-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3292e-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3292e-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3292e-147">displayName</span><span class="sxs-lookup"><span data-stu-id="3292e-147">displayName</span></span>|<span data-ttu-id="3292e-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3292e-148">String</span></span>|<span data-ttu-id="3292e-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="3292e-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3292e-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3292e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3292e-151">Version</span><span class="sxs-lookup"><span data-stu-id="3292e-151">version</span></span>|<span data-ttu-id="3292e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="3292e-152">Int32</span></span>|<span data-ttu-id="3292e-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="3292e-153">Version of the device configuration.</span></span> <span data-ttu-id="3292e-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3292e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3292e-155">launchUri</span><span class="sxs-lookup"><span data-stu-id="3292e-155">launchUri</span></span>|<span data-ttu-id="3292e-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3292e-156">String</span></span>|<span data-ttu-id="3292e-157">URL zu einer Bewertung, die automatisch geladen wird, sobald der Browser für sichere Bewertungen gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="3292e-157">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="3292e-158">Die URL muss eine gültige URL sein (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="3292e-158">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="3292e-159">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="3292e-159">configurationAccount</span></span>|<span data-ttu-id="3292e-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3292e-160">String</span></span>|<span data-ttu-id="3292e-161">Konto, mit dem das Windows-Gerät für den Test konfiguriert wurde.</span><span class="sxs-lookup"><span data-stu-id="3292e-161">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="3292e-162">Der Benutzer kann ein Domänenkonto (Domäne\Benutzername), ein AAD-Konto (benutzername@mandant.com) oder ein lokales Konto (Benutzername) sein.</span><span class="sxs-lookup"><span data-stu-id="3292e-162">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="3292e-163">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="3292e-163">allowPrinting</span></span>|<span data-ttu-id="3292e-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="3292e-164">Boolean</span></span>|<span data-ttu-id="3292e-165">Gibt an, ob während des Tests über die App gedruckt werden darf.</span><span class="sxs-lookup"><span data-stu-id="3292e-165">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="3292e-166">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="3292e-166">allowScreenCapture</span></span>|<span data-ttu-id="3292e-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="3292e-167">Boolean</span></span>|<span data-ttu-id="3292e-168">Gibt an, ob während des Tests über die App Screenshots angefertigt werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="3292e-168">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="3292e-169">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="3292e-169">allowTextSuggestion</span></span>|<span data-ttu-id="3292e-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="3292e-170">Boolean</span></span>|<span data-ttu-id="3292e-171">Gibt an, ob während des Tests Wortvorschläge angezeigt werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="3292e-171">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="3292e-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="3292e-172">Response</span></span>
<span data-ttu-id="3292e-173">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3292e-173">If successful, this method returns a `201 Created` response code and a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3292e-174">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3292e-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="3292e-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3292e-175">Request</span></span>
<span data-ttu-id="3292e-176">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3292e-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 359

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```

### <a name="response"></a><span data-ttu-id="3292e-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="3292e-177">Response</span></span>
<span data-ttu-id="3292e-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3292e-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 531

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "id": "f60d71be-71be-f60d-be71-0df6be710df6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```



