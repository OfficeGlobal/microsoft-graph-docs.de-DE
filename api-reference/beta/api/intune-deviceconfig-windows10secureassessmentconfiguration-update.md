---
title: Aktualisieren von „windows10SecureAssessmentConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs windows10SecureAssessmentConfiguration.
author: tfitzmac
ms.openlocfilehash: 903a5f16f35456aecc6285f87f371a73ebee25ae
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304991"
---
# <a name="update-windows10secureassessmentconfiguration"></a><span data-ttu-id="39f14-103">Aktualisieren von „windows10SecureAssessmentConfiguration“</span><span class="sxs-lookup"><span data-stu-id="39f14-103">Update windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="39f14-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="39f14-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="39f14-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="39f14-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="39f14-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="39f14-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="39f14-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39f14-107">Update the properties of a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="39f14-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="39f14-108">Prerequisites</span></span>
<span data-ttu-id="39f14-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39f14-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39f14-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="39f14-111">Permission type</span></span>|<span data-ttu-id="39f14-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="39f14-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39f14-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="39f14-113">Delegated (work or school account)</span></span>|<span data-ttu-id="39f14-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39f14-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="39f14-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="39f14-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39f14-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="39f14-116">Not supported.</span></span>|
|<span data-ttu-id="39f14-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="39f14-117">Application</span></span>|<span data-ttu-id="39f14-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="39f14-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39f14-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="39f14-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="39f14-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="39f14-120">Request headers</span></span>
|<span data-ttu-id="39f14-121">Header</span><span class="sxs-lookup"><span data-stu-id="39f14-121">Header</span></span>|<span data-ttu-id="39f14-122">Wert</span><span class="sxs-lookup"><span data-stu-id="39f14-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39f14-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="39f14-123">Authorization</span></span>|<span data-ttu-id="39f14-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="39f14-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39f14-125">Accept</span><span class="sxs-lookup"><span data-stu-id="39f14-125">Accept</span></span>|<span data-ttu-id="39f14-126">application/json</span><span class="sxs-lookup"><span data-stu-id="39f14-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39f14-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="39f14-127">Request body</span></span>
<span data-ttu-id="39f14-128">Geben Sie als Anforderungstext eine JSON-Darstellung von Objekten des Typs [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="39f14-128">In the request body, supply a JSON representation for the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

<span data-ttu-id="39f14-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="39f14-129">The following table shows the properties that are required when you create the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span></span>

|<span data-ttu-id="39f14-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="39f14-130">Property</span></span>|<span data-ttu-id="39f14-131">Typ</span><span class="sxs-lookup"><span data-stu-id="39f14-131">Type</span></span>|<span data-ttu-id="39f14-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="39f14-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39f14-133">id</span><span class="sxs-lookup"><span data-stu-id="39f14-133">id</span></span>|<span data-ttu-id="39f14-134">String</span><span class="sxs-lookup"><span data-stu-id="39f14-134">String</span></span>|<span data-ttu-id="39f14-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="39f14-135">Key of the entity.</span></span> <span data-ttu-id="39f14-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39f14-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39f14-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="39f14-137">lastModifiedDateTime</span></span>|<span data-ttu-id="39f14-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39f14-138">DateTimeOffset</span></span>|<span data-ttu-id="39f14-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="39f14-139">DateTime the object was last modified.</span></span> <span data-ttu-id="39f14-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39f14-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39f14-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="39f14-141">roleScopeTagIds</span></span>|<span data-ttu-id="39f14-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="39f14-142">String collection</span></span>|<span data-ttu-id="39f14-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="39f14-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="39f14-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39f14-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39f14-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="39f14-145">supportsScopeTags</span></span>|<span data-ttu-id="39f14-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="39f14-146">Boolean</span></span>|<span data-ttu-id="39f14-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="39f14-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="39f14-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="39f14-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="39f14-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="39f14-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="39f14-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="39f14-150">This property is read-only.</span></span> <span data-ttu-id="39f14-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39f14-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39f14-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="39f14-152">createdDateTime</span></span>|<span data-ttu-id="39f14-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39f14-153">DateTimeOffset</span></span>|<span data-ttu-id="39f14-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="39f14-154">DateTime the object was created.</span></span> <span data-ttu-id="39f14-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39f14-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39f14-156">description</span><span class="sxs-lookup"><span data-stu-id="39f14-156">description</span></span>|<span data-ttu-id="39f14-157">String</span><span class="sxs-lookup"><span data-stu-id="39f14-157">String</span></span>|<span data-ttu-id="39f14-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="39f14-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="39f14-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39f14-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39f14-160">displayName</span><span class="sxs-lookup"><span data-stu-id="39f14-160">displayName</span></span>|<span data-ttu-id="39f14-161">String</span><span class="sxs-lookup"><span data-stu-id="39f14-161">String</span></span>|<span data-ttu-id="39f14-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="39f14-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="39f14-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39f14-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39f14-164">Version</span><span class="sxs-lookup"><span data-stu-id="39f14-164">version</span></span>|<span data-ttu-id="39f14-165">Int32</span><span class="sxs-lookup"><span data-stu-id="39f14-165">Int32</span></span>|<span data-ttu-id="39f14-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="39f14-166">Version of the device configuration.</span></span> <span data-ttu-id="39f14-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39f14-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39f14-168">launchUri</span><span class="sxs-lookup"><span data-stu-id="39f14-168">launchUri</span></span>|<span data-ttu-id="39f14-169">String</span><span class="sxs-lookup"><span data-stu-id="39f14-169">String</span></span>|<span data-ttu-id="39f14-170">URL zu einer Bewertung, die automatisch geladen wird, sobald der Browser für sichere Bewertungen gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="39f14-170">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="39f14-171">Die URL muss eine gültige URL sein (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="39f14-171">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="39f14-172">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="39f14-172">configurationAccount</span></span>|<span data-ttu-id="39f14-173">String</span><span class="sxs-lookup"><span data-stu-id="39f14-173">String</span></span>|<span data-ttu-id="39f14-174">Konto, mit dem das Windows-Gerät für den Test konfiguriert wurde.</span><span class="sxs-lookup"><span data-stu-id="39f14-174">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="39f14-175">Der Benutzer kann ein Domänenkonto (Domäne\Benutzername), ein AAD-Konto (benutzername@mandant.com) oder ein lokales Konto (Benutzername) sein.</span><span class="sxs-lookup"><span data-stu-id="39f14-175">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="39f14-176">configurationAccountType</span><span class="sxs-lookup"><span data-stu-id="39f14-176">configurationAccountType</span></span>|[<span data-ttu-id="39f14-177">secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="39f14-177">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="39f14-178">Die Kontenart verwendet, um durch ConfigurationAccount.</span><span class="sxs-lookup"><span data-stu-id="39f14-178">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="39f14-179">Mögliche Werte sind: `azureADAccount`, `domainAccount` und `localAccount`.</span><span class="sxs-lookup"><span data-stu-id="39f14-179">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`.</span></span>|
|<span data-ttu-id="39f14-180">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="39f14-180">allowPrinting</span></span>|<span data-ttu-id="39f14-181">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="39f14-181">Boolean</span></span>|<span data-ttu-id="39f14-182">Gibt an, ob während des Tests über die App gedruckt werden darf.</span><span class="sxs-lookup"><span data-stu-id="39f14-182">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="39f14-183">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="39f14-183">allowScreenCapture</span></span>|<span data-ttu-id="39f14-184">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="39f14-184">Boolean</span></span>|<span data-ttu-id="39f14-185">Gibt an, ob während des Tests über die App Screenshots angefertigt werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="39f14-185">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="39f14-186">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="39f14-186">allowTextSuggestion</span></span>|<span data-ttu-id="39f14-187">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="39f14-187">Boolean</span></span>|<span data-ttu-id="39f14-188">Gibt an, ob während des Tests Wortvorschläge angezeigt werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="39f14-188">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="39f14-189">Antwort</span><span class="sxs-lookup"><span data-stu-id="39f14-189">Response</span></span>
<span data-ttu-id="39f14-190">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="39f14-190">If successful, this method returns a `200 OK` response code and an updated [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39f14-191">Beispiel</span><span class="sxs-lookup"><span data-stu-id="39f14-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="39f14-192">Anforderung</span><span class="sxs-lookup"><span data-stu-id="39f14-192">Request</span></span>
<span data-ttu-id="39f14-193">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="39f14-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 486

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="39f14-194">Antwort</span><span class="sxs-lookup"><span data-stu-id="39f14-194">Response</span></span>
<span data-ttu-id="39f14-p114">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="39f14-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





