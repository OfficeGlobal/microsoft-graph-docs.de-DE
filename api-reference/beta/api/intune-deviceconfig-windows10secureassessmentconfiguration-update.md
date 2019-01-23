---
title: Aktualisieren von „windows10SecureAssessmentConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs windows10SecureAssessmentConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4503276def73977eb623eb472b7dd9fcf1446e6f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421410"
---
# <a name="update-windows10secureassessmentconfiguration"></a><span data-ttu-id="6391d-103">Aktualisieren von „windows10SecureAssessmentConfiguration“</span><span class="sxs-lookup"><span data-stu-id="6391d-103">Update windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="6391d-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="6391d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6391d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6391d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6391d-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6391d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6391d-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6391d-107">Update the properties of a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6391d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6391d-108">Prerequisites</span></span>
<span data-ttu-id="6391d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6391d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6391d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6391d-111">Permission type</span></span>|<span data-ttu-id="6391d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6391d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6391d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6391d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6391d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6391d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6391d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6391d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6391d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6391d-116">Not supported.</span></span>|
|<span data-ttu-id="6391d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6391d-117">Application</span></span>|<span data-ttu-id="6391d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6391d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6391d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6391d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6391d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6391d-120">Request headers</span></span>
|<span data-ttu-id="6391d-121">Header</span><span class="sxs-lookup"><span data-stu-id="6391d-121">Header</span></span>|<span data-ttu-id="6391d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="6391d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6391d-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="6391d-123">Authorization</span></span>|<span data-ttu-id="6391d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6391d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6391d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6391d-125">Accept</span></span>|<span data-ttu-id="6391d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6391d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6391d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6391d-127">Request body</span></span>
<span data-ttu-id="6391d-128">Geben Sie als Anforderungstext eine JSON-Darstellung von Objekten des Typs [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="6391d-128">In the request body, supply a JSON representation for the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

<span data-ttu-id="6391d-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="6391d-129">The following table shows the properties that are required when you create the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span></span>

|<span data-ttu-id="6391d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6391d-130">Property</span></span>|<span data-ttu-id="6391d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="6391d-131">Type</span></span>|<span data-ttu-id="6391d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6391d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6391d-133">id</span><span class="sxs-lookup"><span data-stu-id="6391d-133">id</span></span>|<span data-ttu-id="6391d-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6391d-134">String</span></span>|<span data-ttu-id="6391d-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6391d-135">Key of the entity.</span></span> <span data-ttu-id="6391d-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6391d-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6391d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6391d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6391d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6391d-138">DateTimeOffset</span></span>|<span data-ttu-id="6391d-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="6391d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6391d-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6391d-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6391d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6391d-141">roleScopeTagIds</span></span>|<span data-ttu-id="6391d-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="6391d-142">String collection</span></span>|<span data-ttu-id="6391d-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="6391d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6391d-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6391d-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6391d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6391d-145">supportsScopeTags</span></span>|<span data-ttu-id="6391d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="6391d-146">Boolean</span></span>|<span data-ttu-id="6391d-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6391d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6391d-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="6391d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6391d-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="6391d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6391d-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6391d-150">This property is read-only.</span></span> <span data-ttu-id="6391d-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6391d-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6391d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6391d-152">createdDateTime</span></span>|<span data-ttu-id="6391d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6391d-153">DateTimeOffset</span></span>|<span data-ttu-id="6391d-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="6391d-154">DateTime the object was created.</span></span> <span data-ttu-id="6391d-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6391d-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6391d-156">description</span><span class="sxs-lookup"><span data-stu-id="6391d-156">description</span></span>|<span data-ttu-id="6391d-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6391d-157">String</span></span>|<span data-ttu-id="6391d-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="6391d-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6391d-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6391d-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6391d-160">displayName</span><span class="sxs-lookup"><span data-stu-id="6391d-160">displayName</span></span>|<span data-ttu-id="6391d-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6391d-161">String</span></span>|<span data-ttu-id="6391d-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="6391d-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6391d-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6391d-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6391d-164">Version</span><span class="sxs-lookup"><span data-stu-id="6391d-164">version</span></span>|<span data-ttu-id="6391d-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6391d-165">Int32</span></span>|<span data-ttu-id="6391d-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="6391d-166">Version of the device configuration.</span></span> <span data-ttu-id="6391d-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6391d-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6391d-168">launchUri</span><span class="sxs-lookup"><span data-stu-id="6391d-168">launchUri</span></span>|<span data-ttu-id="6391d-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6391d-169">String</span></span>|<span data-ttu-id="6391d-170">URL zu einer Bewertung, die automatisch geladen wird, sobald der Browser für sichere Bewertungen gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="6391d-170">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="6391d-171">Die URL muss eine gültige URL sein (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="6391d-171">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="6391d-172">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="6391d-172">configurationAccount</span></span>|<span data-ttu-id="6391d-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6391d-173">String</span></span>|<span data-ttu-id="6391d-174">Konto, mit dem das Windows-Gerät für den Test konfiguriert wurde.</span><span class="sxs-lookup"><span data-stu-id="6391d-174">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="6391d-175">Der Benutzer kann ein Domänenkonto (Domäne\Benutzername), ein AAD-Konto (benutzername@mandant.com) oder ein lokales Konto (Benutzername) sein.</span><span class="sxs-lookup"><span data-stu-id="6391d-175">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="6391d-176">configurationAccountType</span><span class="sxs-lookup"><span data-stu-id="6391d-176">configurationAccountType</span></span>|[<span data-ttu-id="6391d-177">secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="6391d-177">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="6391d-178">Die Kontenart verwendet, um durch ConfigurationAccount.</span><span class="sxs-lookup"><span data-stu-id="6391d-178">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="6391d-179">Mögliche Werte sind: `azureADAccount`, `domainAccount` und `localAccount`.</span><span class="sxs-lookup"><span data-stu-id="6391d-179">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`.</span></span>|
|<span data-ttu-id="6391d-180">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="6391d-180">allowPrinting</span></span>|<span data-ttu-id="6391d-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="6391d-181">Boolean</span></span>|<span data-ttu-id="6391d-182">Gibt an, ob während des Tests über die App gedruckt werden darf.</span><span class="sxs-lookup"><span data-stu-id="6391d-182">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="6391d-183">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="6391d-183">allowScreenCapture</span></span>|<span data-ttu-id="6391d-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="6391d-184">Boolean</span></span>|<span data-ttu-id="6391d-185">Gibt an, ob während des Tests über die App Screenshots angefertigt werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="6391d-185">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="6391d-186">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="6391d-186">allowTextSuggestion</span></span>|<span data-ttu-id="6391d-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="6391d-187">Boolean</span></span>|<span data-ttu-id="6391d-188">Gibt an, ob während des Tests Wortvorschläge angezeigt werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="6391d-188">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="6391d-189">Antwort</span><span class="sxs-lookup"><span data-stu-id="6391d-189">Response</span></span>
<span data-ttu-id="6391d-190">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6391d-190">If successful, this method returns a `200 OK` response code and an updated [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6391d-191">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6391d-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="6391d-192">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6391d-192">Request</span></span>
<span data-ttu-id="6391d-193">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6391d-193">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6391d-194">Antwort</span><span class="sxs-lookup"><span data-stu-id="6391d-194">Response</span></span>
<span data-ttu-id="6391d-p114">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6391d-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




