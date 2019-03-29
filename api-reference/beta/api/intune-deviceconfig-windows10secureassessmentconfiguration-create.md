---
title: Erstellen von „windows10SecureAssessmentConfiguration“
description: Erstellt neue Objekte des Typs windows10SecureAssessmentConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f0f5428d517433bf499cf22d85c6a589ea331d66
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975903"
---
# <a name="create-windows10secureassessmentconfiguration"></a><span data-ttu-id="dfd85-103">Erstellen von „windows10SecureAssessmentConfiguration“</span><span class="sxs-lookup"><span data-stu-id="dfd85-103">Create windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="dfd85-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dfd85-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dfd85-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="dfd85-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfd85-106">Erstellen eines neuen [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="dfd85-106">Create a new [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dfd85-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="dfd85-107">Prerequisites</span></span>
<span data-ttu-id="dfd85-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfd85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfd85-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dfd85-110">Permission type</span></span>|<span data-ttu-id="dfd85-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dfd85-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dfd85-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dfd85-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dfd85-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfd85-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dfd85-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dfd85-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dfd85-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dfd85-115">Not supported.</span></span>|
|<span data-ttu-id="dfd85-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dfd85-116">Application</span></span>|<span data-ttu-id="dfd85-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dfd85-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dfd85-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dfd85-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="dfd85-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dfd85-119">Request headers</span></span>
|<span data-ttu-id="dfd85-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="dfd85-120">Header</span></span>|<span data-ttu-id="dfd85-121">Wert</span><span class="sxs-lookup"><span data-stu-id="dfd85-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dfd85-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dfd85-122">Authorization</span></span>|<span data-ttu-id="dfd85-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="dfd85-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dfd85-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="dfd85-124">Accept</span></span>|<span data-ttu-id="dfd85-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dfd85-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfd85-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dfd85-126">Request body</span></span>
<span data-ttu-id="dfd85-127">Geben Sie im Anforderungstext eine JSON-Darstellung des windows10SecureAssessmentConfiguration-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="dfd85-127">In the request body, supply a JSON representation for the windows10SecureAssessmentConfiguration object.</span></span>

<span data-ttu-id="dfd85-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windows10SecureAssessmentConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="dfd85-128">The following table shows the properties that are required when you create the windows10SecureAssessmentConfiguration.</span></span>

|<span data-ttu-id="dfd85-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dfd85-129">Property</span></span>|<span data-ttu-id="dfd85-130">Typ</span><span class="sxs-lookup"><span data-stu-id="dfd85-130">Type</span></span>|<span data-ttu-id="dfd85-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dfd85-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfd85-132">id</span><span class="sxs-lookup"><span data-stu-id="dfd85-132">id</span></span>|<span data-ttu-id="dfd85-133">String</span><span class="sxs-lookup"><span data-stu-id="dfd85-133">String</span></span>|<span data-ttu-id="dfd85-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="dfd85-134">Key of the entity.</span></span> <span data-ttu-id="dfd85-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dfd85-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfd85-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dfd85-136">lastModifiedDateTime</span></span>|<span data-ttu-id="dfd85-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfd85-137">DateTimeOffset</span></span>|<span data-ttu-id="dfd85-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="dfd85-138">DateTime the object was last modified.</span></span> <span data-ttu-id="dfd85-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dfd85-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfd85-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="dfd85-140">roleScopeTagIds</span></span>|<span data-ttu-id="dfd85-141">String collection</span><span class="sxs-lookup"><span data-stu-id="dfd85-141">String collection</span></span>|<span data-ttu-id="dfd85-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="dfd85-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="dfd85-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dfd85-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfd85-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="dfd85-144">supportsScopeTags</span></span>|<span data-ttu-id="dfd85-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dfd85-145">Boolean</span></span>|<span data-ttu-id="dfd85-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dfd85-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="dfd85-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="dfd85-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="dfd85-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="dfd85-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="dfd85-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="dfd85-149">This property is read-only.</span></span> <span data-ttu-id="dfd85-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dfd85-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfd85-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dfd85-151">createdDateTime</span></span>|<span data-ttu-id="dfd85-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfd85-152">DateTimeOffset</span></span>|<span data-ttu-id="dfd85-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="dfd85-153">DateTime the object was created.</span></span> <span data-ttu-id="dfd85-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dfd85-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfd85-155">description</span><span class="sxs-lookup"><span data-stu-id="dfd85-155">description</span></span>|<span data-ttu-id="dfd85-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dfd85-156">String</span></span>|<span data-ttu-id="dfd85-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="dfd85-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dfd85-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dfd85-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfd85-159">displayName</span><span class="sxs-lookup"><span data-stu-id="dfd85-159">displayName</span></span>|<span data-ttu-id="dfd85-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dfd85-160">String</span></span>|<span data-ttu-id="dfd85-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="dfd85-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dfd85-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfd85-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfd85-163">Version</span><span class="sxs-lookup"><span data-stu-id="dfd85-163">version</span></span>|<span data-ttu-id="dfd85-164">Int32</span><span class="sxs-lookup"><span data-stu-id="dfd85-164">Int32</span></span>|<span data-ttu-id="dfd85-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="dfd85-165">Version of the device configuration.</span></span> <span data-ttu-id="dfd85-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dfd85-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfd85-167">launchUri</span><span class="sxs-lookup"><span data-stu-id="dfd85-167">launchUri</span></span>|<span data-ttu-id="dfd85-168">String</span><span class="sxs-lookup"><span data-stu-id="dfd85-168">String</span></span>|<span data-ttu-id="dfd85-169">URL zu einer Bewertung, die automatisch geladen wird, sobald der Browser für sichere Bewertungen gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="dfd85-169">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="dfd85-170">Die URL muss eine gültige URL sein (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="dfd85-170">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="dfd85-171">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="dfd85-171">configurationAccount</span></span>|<span data-ttu-id="dfd85-172">String</span><span class="sxs-lookup"><span data-stu-id="dfd85-172">String</span></span>|<span data-ttu-id="dfd85-173">Konto, mit dem das Windows-Gerät für den Test konfiguriert wurde.</span><span class="sxs-lookup"><span data-stu-id="dfd85-173">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="dfd85-174">Der Benutzer kann ein Domänenkonto (Domäne\Benutzername), ein AAD-Konto (benutzername@mandant.com) oder ein lokales Konto (Benutzername) sein.</span><span class="sxs-lookup"><span data-stu-id="dfd85-174">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="dfd85-175">configurationAccountType</span><span class="sxs-lookup"><span data-stu-id="dfd85-175">configurationAccountType</span></span>|[<span data-ttu-id="dfd85-176">secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="dfd85-176">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="dfd85-177">Der Kontotyp, der von ConfigurationAccount verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="dfd85-177">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="dfd85-178">Mögliche Werte sind: `azureADAccount`, `domainAccount` und `localAccount`.</span><span class="sxs-lookup"><span data-stu-id="dfd85-178">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`.</span></span>|
|<span data-ttu-id="dfd85-179">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="dfd85-179">allowPrinting</span></span>|<span data-ttu-id="dfd85-180">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dfd85-180">Boolean</span></span>|<span data-ttu-id="dfd85-181">Gibt an, ob während des Tests über die App gedruckt werden darf.</span><span class="sxs-lookup"><span data-stu-id="dfd85-181">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="dfd85-182">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="dfd85-182">allowScreenCapture</span></span>|<span data-ttu-id="dfd85-183">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="dfd85-183">Boolean</span></span>|<span data-ttu-id="dfd85-184">Gibt an, ob während des Tests über die App Screenshots angefertigt werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="dfd85-184">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="dfd85-185">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="dfd85-185">allowTextSuggestion</span></span>|<span data-ttu-id="dfd85-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfd85-186">Boolean</span></span>|<span data-ttu-id="dfd85-187">Gibt an, ob während des Tests Wortvorschläge angezeigt werden dürfen.</span><span class="sxs-lookup"><span data-stu-id="dfd85-187">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="dfd85-188">Antwort</span><span class="sxs-lookup"><span data-stu-id="dfd85-188">Response</span></span>
<span data-ttu-id="dfd85-189">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dfd85-189">If successful, this method returns a `201 Created` response code and a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfd85-190">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dfd85-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="dfd85-191">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dfd85-191">Request</span></span>
<span data-ttu-id="dfd85-192">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dfd85-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="dfd85-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="dfd85-193">Response</span></span>
<span data-ttu-id="dfd85-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dfd85-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




