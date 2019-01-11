---
title: Aktualisieren von „windows10SecureAssessmentConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs windows10SecureAssessmentConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e55b584972c59d061d20785f7877551836998ebb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844548"
---
# <a name="update-windows10secureassessmentconfiguration"></a><span data-ttu-id="4a065-103">Aktualisieren von „windows10SecureAssessmentConfiguration“</span><span class="sxs-lookup"><span data-stu-id="4a065-103">Update windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="4a065-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4a065-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4a065-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a065-105">Update the properties of a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4a065-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4a065-106">Prerequisites</span></span>
<span data-ttu-id="4a065-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a065-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a065-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4a065-109">Permission type</span></span>|<span data-ttu-id="4a065-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4a065-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a065-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4a065-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4a065-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a065-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4a065-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4a065-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a065-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4a065-114">Not supported.</span></span>|
|<span data-ttu-id="4a065-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4a065-115">Application</span></span>|<span data-ttu-id="4a065-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4a065-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a065-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a065-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4a065-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4a065-118">Request headers</span></span>
|<span data-ttu-id="4a065-119">Header</span><span class="sxs-lookup"><span data-stu-id="4a065-119">Header</span></span>|<span data-ttu-id="4a065-120">Wert</span><span class="sxs-lookup"><span data-stu-id="4a065-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a065-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a065-121">Authorization</span></span>|<span data-ttu-id="4a065-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4a065-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a065-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4a065-123">Accept</span></span>|<span data-ttu-id="4a065-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4a065-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a065-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4a065-125">Request body</span></span>
<span data-ttu-id="4a065-126">Geben Sie als Anforderungstext eine JSON-Darstellung von Objekten des Typs [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="4a065-126">In the request body, supply a JSON representation for the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

<span data-ttu-id="4a065-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="4a065-127">The following table shows the properties that are required when you create the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span></span>

|<span data-ttu-id="4a065-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4a065-128">Property</span></span>|<span data-ttu-id="4a065-129">Typ</span><span class="sxs-lookup"><span data-stu-id="4a065-129">Type</span></span>|<span data-ttu-id="4a065-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4a065-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a065-131">id</span><span class="sxs-lookup"><span data-stu-id="4a065-131">id</span></span>|<span data-ttu-id="4a065-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4a065-132">String</span></span>|<span data-ttu-id="4a065-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="4a065-133">Key of the entity.</span></span> <span data-ttu-id="4a065-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a065-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a065-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a065-135">lastModifiedDateTime</span></span>|<span data-ttu-id="4a065-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a065-136">DateTimeOffset</span></span>|<span data-ttu-id="4a065-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="4a065-137">DateTime the object was last modified.</span></span> <span data-ttu-id="4a065-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a065-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a065-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4a065-139">createdDateTime</span></span>|<span data-ttu-id="4a065-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a065-140">DateTimeOffset</span></span>|<span data-ttu-id="4a065-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="4a065-141">DateTime the object was created.</span></span> <span data-ttu-id="4a065-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a065-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a065-143">description</span><span class="sxs-lookup"><span data-stu-id="4a065-143">description</span></span>|<span data-ttu-id="4a065-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4a065-144">String</span></span>|<span data-ttu-id="4a065-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="4a065-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4a065-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a065-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a065-147">displayName</span><span class="sxs-lookup"><span data-stu-id="4a065-147">displayName</span></span>|<span data-ttu-id="4a065-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4a065-148">String</span></span>|<span data-ttu-id="4a065-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="4a065-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4a065-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a065-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a065-151">Version</span><span class="sxs-lookup"><span data-stu-id="4a065-151">version</span></span>|<span data-ttu-id="4a065-152">Int32</span><span class="sxs-lookup"><span data-stu-id="4a065-152">Int32</span></span>|<span data-ttu-id="4a065-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="4a065-153">Version of the device configuration.</span></span> <span data-ttu-id="4a065-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a065-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a065-155">launchUri</span><span class="sxs-lookup"><span data-stu-id="4a065-155">launchUri</span></span>|<span data-ttu-id="4a065-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4a065-156">String</span></span>|<span data-ttu-id="4a065-157">URL zu einer Bewertung, die automatisch geladen wird, sobald der Browser für sichere Bewertungen gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="4a065-157">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="4a065-158">Die URL muss eine gültige URL sein (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="4a065-158">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="4a065-159">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="4a065-159">configurationAccount</span></span>|<span data-ttu-id="4a065-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4a065-160">String</span></span>|<span data-ttu-id="4a065-161">Konto, mit dem das Windows-Gerät für den Test konfiguriert wurde.</span><span class="sxs-lookup"><span data-stu-id="4a065-161">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="4a065-162">Der Benutzer kann ein Domänenkonto (Domäne\Benutzername), ein AAD-Konto (benutzername@mandant.com) oder ein lokales Konto (Benutzername) sein.</span><span class="sxs-lookup"><span data-stu-id="4a065-162">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="4a065-163">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="4a065-163">allowPrinting</span></span>|<span data-ttu-id="4a065-164">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4a065-164">Boolean</span></span>|<span data-ttu-id="4a065-165">Gibt an, ob während des Tests über die App gedruckt werden darf.</span><span class="sxs-lookup"><span data-stu-id="4a065-165">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="4a065-166">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="4a065-166">allowScreenCapture</span></span>|<span data-ttu-id="4a065-167">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4a065-167">Boolean</span></span>|<span data-ttu-id="4a065-168">Gibt an, ob während des Tests über die App Screenshots angefertigt werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="4a065-168">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="4a065-169">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="4a065-169">allowTextSuggestion</span></span>|<span data-ttu-id="4a065-170">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4a065-170">Boolean</span></span>|<span data-ttu-id="4a065-171">Gibt an, ob während des Tests Wortvorschläge angezeigt werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="4a065-171">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="4a065-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a065-172">Response</span></span>
<span data-ttu-id="4a065-173">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4a065-173">If successful, this method returns a `200 OK` response code and an updated [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a065-174">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4a065-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="4a065-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a065-175">Request</span></span>
<span data-ttu-id="4a065-176">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4a065-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="4a065-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a065-177">Response</span></span>
<span data-ttu-id="4a065-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4a065-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



