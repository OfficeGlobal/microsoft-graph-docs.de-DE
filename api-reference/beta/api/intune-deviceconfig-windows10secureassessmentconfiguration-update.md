---
title: Aktualisieren von „windows10SecureAssessmentConfiguration“
description: Aktualisiert die Eigenschaften von Objekten des Typs windows10SecureAssessmentConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3ebff2b3c12e605727fd0eeff5f953713d5303b8
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984464"
---
# <a name="update-windows10secureassessmentconfiguration"></a><span data-ttu-id="ee8af-103">Aktualisieren von „windows10SecureAssessmentConfiguration“</span><span class="sxs-lookup"><span data-stu-id="ee8af-103">Update windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="ee8af-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ee8af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee8af-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ee8af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee8af-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee8af-106">Update the properties of a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee8af-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ee8af-107">Prerequisites</span></span>
<span data-ttu-id="ee8af-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee8af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee8af-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ee8af-110">Permission type</span></span>|<span data-ttu-id="ee8af-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ee8af-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee8af-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ee8af-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ee8af-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee8af-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ee8af-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ee8af-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee8af-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ee8af-115">Not supported.</span></span>|
|<span data-ttu-id="ee8af-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ee8af-116">Application</span></span>|<span data-ttu-id="ee8af-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ee8af-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee8af-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ee8af-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ee8af-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ee8af-119">Request headers</span></span>
|<span data-ttu-id="ee8af-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ee8af-120">Header</span></span>|<span data-ttu-id="ee8af-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ee8af-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee8af-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee8af-122">Authorization</span></span>|<span data-ttu-id="ee8af-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ee8af-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee8af-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ee8af-124">Accept</span></span>|<span data-ttu-id="ee8af-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ee8af-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee8af-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ee8af-126">Request body</span></span>
<span data-ttu-id="ee8af-127">Geben Sie als Anforderungstext eine JSON-Darstellung von Objekten des Typs [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="ee8af-127">In the request body, supply a JSON representation for the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

<span data-ttu-id="ee8af-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="ee8af-128">The following table shows the properties that are required when you create the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span></span>

|<span data-ttu-id="ee8af-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ee8af-129">Property</span></span>|<span data-ttu-id="ee8af-130">Typ</span><span class="sxs-lookup"><span data-stu-id="ee8af-130">Type</span></span>|<span data-ttu-id="ee8af-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ee8af-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee8af-132">id</span><span class="sxs-lookup"><span data-stu-id="ee8af-132">id</span></span>|<span data-ttu-id="ee8af-133">String</span><span class="sxs-lookup"><span data-stu-id="ee8af-133">String</span></span>|<span data-ttu-id="ee8af-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ee8af-134">Key of the entity.</span></span> <span data-ttu-id="ee8af-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee8af-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee8af-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee8af-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ee8af-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee8af-137">DateTimeOffset</span></span>|<span data-ttu-id="ee8af-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ee8af-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ee8af-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee8af-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee8af-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="ee8af-140">roleScopeTagIds</span></span>|<span data-ttu-id="ee8af-141">String collection</span><span class="sxs-lookup"><span data-stu-id="ee8af-141">String collection</span></span>|<span data-ttu-id="ee8af-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="ee8af-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ee8af-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee8af-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee8af-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ee8af-144">supportsScopeTags</span></span>|<span data-ttu-id="ee8af-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ee8af-145">Boolean</span></span>|<span data-ttu-id="ee8af-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ee8af-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ee8af-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="ee8af-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ee8af-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="ee8af-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ee8af-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ee8af-149">This property is read-only.</span></span> <span data-ttu-id="ee8af-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee8af-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee8af-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ee8af-151">createdDateTime</span></span>|<span data-ttu-id="ee8af-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee8af-152">DateTimeOffset</span></span>|<span data-ttu-id="ee8af-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ee8af-153">DateTime the object was created.</span></span> <span data-ttu-id="ee8af-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee8af-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee8af-155">description</span><span class="sxs-lookup"><span data-stu-id="ee8af-155">description</span></span>|<span data-ttu-id="ee8af-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ee8af-156">String</span></span>|<span data-ttu-id="ee8af-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ee8af-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ee8af-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee8af-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee8af-159">displayName</span><span class="sxs-lookup"><span data-stu-id="ee8af-159">displayName</span></span>|<span data-ttu-id="ee8af-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ee8af-160">String</span></span>|<span data-ttu-id="ee8af-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ee8af-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ee8af-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ee8af-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee8af-163">Version</span><span class="sxs-lookup"><span data-stu-id="ee8af-163">version</span></span>|<span data-ttu-id="ee8af-164">Int32</span><span class="sxs-lookup"><span data-stu-id="ee8af-164">Int32</span></span>|<span data-ttu-id="ee8af-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="ee8af-165">Version of the device configuration.</span></span> <span data-ttu-id="ee8af-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee8af-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee8af-167">launchUri</span><span class="sxs-lookup"><span data-stu-id="ee8af-167">launchUri</span></span>|<span data-ttu-id="ee8af-168">String</span><span class="sxs-lookup"><span data-stu-id="ee8af-168">String</span></span>|<span data-ttu-id="ee8af-169">URL zu einer Bewertung, die automatisch geladen wird, sobald der Browser für sichere Bewertungen gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="ee8af-169">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="ee8af-170">Die URL muss eine gültige URL sein (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="ee8af-170">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="ee8af-171">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="ee8af-171">configurationAccount</span></span>|<span data-ttu-id="ee8af-172">String</span><span class="sxs-lookup"><span data-stu-id="ee8af-172">String</span></span>|<span data-ttu-id="ee8af-173">Konto, mit dem das Windows-Gerät für den Test konfiguriert wurde.</span><span class="sxs-lookup"><span data-stu-id="ee8af-173">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="ee8af-174">Der Benutzer kann ein Domänenkonto (Domäne\Benutzername), ein AAD-Konto (benutzername@mandant.com) oder ein lokales Konto (Benutzername) sein.</span><span class="sxs-lookup"><span data-stu-id="ee8af-174">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="ee8af-175">configurationAccountType</span><span class="sxs-lookup"><span data-stu-id="ee8af-175">configurationAccountType</span></span>|[<span data-ttu-id="ee8af-176">secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="ee8af-176">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="ee8af-177">Der Kontotyp, der von ConfigurationAccount verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="ee8af-177">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="ee8af-178">Mögliche Werte sind: `azureADAccount`, `domainAccount` und `localAccount`.</span><span class="sxs-lookup"><span data-stu-id="ee8af-178">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`.</span></span>|
|<span data-ttu-id="ee8af-179">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="ee8af-179">allowPrinting</span></span>|<span data-ttu-id="ee8af-180">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ee8af-180">Boolean</span></span>|<span data-ttu-id="ee8af-181">Gibt an, ob während des Tests über die App gedruckt werden darf.</span><span class="sxs-lookup"><span data-stu-id="ee8af-181">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="ee8af-182">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="ee8af-182">allowScreenCapture</span></span>|<span data-ttu-id="ee8af-183">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ee8af-183">Boolean</span></span>|<span data-ttu-id="ee8af-184">Gibt an, ob während des Tests über die App Screenshots angefertigt werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="ee8af-184">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="ee8af-185">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="ee8af-185">allowTextSuggestion</span></span>|<span data-ttu-id="ee8af-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee8af-186">Boolean</span></span>|<span data-ttu-id="ee8af-187">Gibt an, ob während des Tests Wortvorschläge angezeigt werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="ee8af-187">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="ee8af-188">Antwort</span><span class="sxs-lookup"><span data-stu-id="ee8af-188">Response</span></span>
<span data-ttu-id="ee8af-189">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ee8af-189">If successful, this method returns a `200 OK` response code and an updated [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee8af-190">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ee8af-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee8af-191">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ee8af-191">Request</span></span>
<span data-ttu-id="ee8af-192">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ee8af-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 499

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "configurationAccountType": "domainAccount",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```

### <a name="response"></a><span data-ttu-id="ee8af-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="ee8af-193">Response</span></span>
<span data-ttu-id="ee8af-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ee8af-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 671

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "id": "f60d71be-71be-f60d-be71-0df6be710df6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "configurationAccountType": "domainAccount",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```




