---
title: Erstellen von iosEduDeviceConfiguration
description: Erstellen eines neuen IosEduDeviceConfiguration-Objekts.
author: tfitzmac
ms.openlocfilehash: f43fc2f753f4d1c5d83aef0b50f10a2cfabe0b84
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333929"
---
# <a name="create-iosedudeviceconfiguration"></a><span data-ttu-id="33570-103">Erstellen von iosEduDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="33570-103">Create iosEduDeviceConfiguration</span></span>

> <span data-ttu-id="33570-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="33570-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33570-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="33570-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="33570-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="33570-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="33570-107">Erstellen eines neuen [IosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="33570-107">Create a new [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="33570-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="33570-108">Prerequisites</span></span>
<span data-ttu-id="33570-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33570-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33570-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="33570-111">Permission type</span></span>|<span data-ttu-id="33570-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="33570-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33570-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="33570-113">Delegated (work or school account)</span></span>|<span data-ttu-id="33570-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33570-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="33570-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="33570-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33570-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="33570-116">Not supported.</span></span>|
|<span data-ttu-id="33570-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="33570-117">Application</span></span>|<span data-ttu-id="33570-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="33570-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33570-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="33570-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="33570-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="33570-120">Request headers</span></span>
|<span data-ttu-id="33570-121">Header</span><span class="sxs-lookup"><span data-stu-id="33570-121">Header</span></span>|<span data-ttu-id="33570-122">Wert</span><span class="sxs-lookup"><span data-stu-id="33570-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33570-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="33570-123">Authorization</span></span>|<span data-ttu-id="33570-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="33570-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33570-125">Accept</span><span class="sxs-lookup"><span data-stu-id="33570-125">Accept</span></span>|<span data-ttu-id="33570-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33570-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33570-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="33570-127">Request body</span></span>
<span data-ttu-id="33570-128">Geben Sie im Textkörper Anforderung für das Objekt IosEduDeviceConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="33570-128">In the request body, supply a JSON representation for the iosEduDeviceConfiguration object.</span></span>

<span data-ttu-id="33570-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die IosEduDeviceConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="33570-129">The following table shows the properties that are required when you create the iosEduDeviceConfiguration.</span></span>

|<span data-ttu-id="33570-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="33570-130">Property</span></span>|<span data-ttu-id="33570-131">Typ</span><span class="sxs-lookup"><span data-stu-id="33570-131">Type</span></span>|<span data-ttu-id="33570-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="33570-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33570-133">id</span><span class="sxs-lookup"><span data-stu-id="33570-133">id</span></span>|<span data-ttu-id="33570-134">String</span><span class="sxs-lookup"><span data-stu-id="33570-134">String</span></span>|<span data-ttu-id="33570-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="33570-135">Key of the entity.</span></span> <span data-ttu-id="33570-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33570-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33570-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="33570-137">lastModifiedDateTime</span></span>|<span data-ttu-id="33570-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33570-138">DateTimeOffset</span></span>|<span data-ttu-id="33570-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="33570-139">DateTime the object was last modified.</span></span> <span data-ttu-id="33570-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33570-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33570-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="33570-141">roleScopeTagIds</span></span>|<span data-ttu-id="33570-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="33570-142">String collection</span></span>|<span data-ttu-id="33570-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="33570-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="33570-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33570-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33570-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="33570-145">supportsScopeTags</span></span>|<span data-ttu-id="33570-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="33570-146">Boolean</span></span>|<span data-ttu-id="33570-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="33570-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="33570-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="33570-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="33570-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="33570-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="33570-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="33570-150">This property is read-only.</span></span> <span data-ttu-id="33570-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33570-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33570-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="33570-152">createdDateTime</span></span>|<span data-ttu-id="33570-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33570-153">DateTimeOffset</span></span>|<span data-ttu-id="33570-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="33570-154">DateTime the object was created.</span></span> <span data-ttu-id="33570-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33570-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33570-156">description</span><span class="sxs-lookup"><span data-stu-id="33570-156">description</span></span>|<span data-ttu-id="33570-157">String</span><span class="sxs-lookup"><span data-stu-id="33570-157">String</span></span>|<span data-ttu-id="33570-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="33570-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="33570-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33570-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33570-160">displayName</span><span class="sxs-lookup"><span data-stu-id="33570-160">displayName</span></span>|<span data-ttu-id="33570-161">String</span><span class="sxs-lookup"><span data-stu-id="33570-161">String</span></span>|<span data-ttu-id="33570-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="33570-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="33570-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33570-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33570-164">Version</span><span class="sxs-lookup"><span data-stu-id="33570-164">version</span></span>|<span data-ttu-id="33570-165">Int32</span><span class="sxs-lookup"><span data-stu-id="33570-165">Int32</span></span>|<span data-ttu-id="33570-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="33570-166">Version of the device configuration.</span></span> <span data-ttu-id="33570-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33570-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33570-168">teacherCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="33570-168">teacherCertificateSettings</span></span>|[<span data-ttu-id="33570-169">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="33570-169">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="33570-170">Die Trusted Root und PFX-Zertifikate für Lehrer</span><span class="sxs-lookup"><span data-stu-id="33570-170">The Trusted Root and PFX certificates for Teacher</span></span>|
|<span data-ttu-id="33570-171">studentCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="33570-171">studentCertificateSettings</span></span>|[<span data-ttu-id="33570-172">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="33570-172">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="33570-173">Die Trusted Root und PFX-Zertifikate für Schüler</span><span class="sxs-lookup"><span data-stu-id="33570-173">The Trusted Root and PFX certificates for Student</span></span>|
|<span data-ttu-id="33570-174">deviceCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="33570-174">deviceCertificateSettings</span></span>|[<span data-ttu-id="33570-175">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="33570-175">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="33570-176">Die Trusted Root und PFX-Zertifikate für Geräte</span><span class="sxs-lookup"><span data-stu-id="33570-176">The Trusted Root and PFX certificates for Device</span></span>|



## <a name="response"></a><span data-ttu-id="33570-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="33570-177">Response</span></span>
<span data-ttu-id="33570-178">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [IosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="33570-178">If successful, this method returns a `201 Created` response code and a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33570-179">Beispiel</span><span class="sxs-lookup"><span data-stu-id="33570-179">Example</span></span>
### <a name="request"></a><span data-ttu-id="33570-180">Anforderung</span><span class="sxs-lookup"><span data-stu-id="33570-180">Request</span></span>
<span data-ttu-id="33570-181">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="33570-181">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1974

{
  "@odata.type": "#microsoft.graph.iosEduDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "teacherCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  },
  "studentCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  },
  "deviceCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  }
}
```

### <a name="response"></a><span data-ttu-id="33570-182">Antwort</span><span class="sxs-lookup"><span data-stu-id="33570-182">Response</span></span>
<span data-ttu-id="33570-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="33570-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2082

{
  "@odata.type": "#microsoft.graph.iosEduDeviceConfiguration",
  "id": "4c5df9b6-f9b6-4c5d-b6f9-5d4cb6f95d4c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "teacherCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  },
  "studentCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  },
  "deviceCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  }
}
```





