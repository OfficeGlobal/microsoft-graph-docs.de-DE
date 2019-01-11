---
title: IosEduDeviceConfiguration aktualisieren
description: Aktualisieren Sie die Eigenschaften eines IosEduDeviceConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5cc4076f3888a162db345ddf83ac7f506abdbf3a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882446"
---
# <a name="update-iosedudeviceconfiguration"></a><span data-ttu-id="330d3-103">IosEduDeviceConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="330d3-103">Update iosEduDeviceConfiguration</span></span>

> <span data-ttu-id="330d3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="330d3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="330d3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="330d3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="330d3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="330d3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="330d3-107">Aktualisieren Sie die Eigenschaften eines [IosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="330d3-107">Update the properties of a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="330d3-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="330d3-108">Prerequisites</span></span>
<span data-ttu-id="330d3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="330d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="330d3-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="330d3-111">Permission type</span></span>|<span data-ttu-id="330d3-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="330d3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="330d3-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="330d3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="330d3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="330d3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="330d3-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="330d3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="330d3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="330d3-116">Not supported.</span></span>|
|<span data-ttu-id="330d3-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="330d3-117">Application</span></span>|<span data-ttu-id="330d3-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="330d3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="330d3-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="330d3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="330d3-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="330d3-120">Request headers</span></span>
|<span data-ttu-id="330d3-121">Header</span><span class="sxs-lookup"><span data-stu-id="330d3-121">Header</span></span>|<span data-ttu-id="330d3-122">Wert</span><span class="sxs-lookup"><span data-stu-id="330d3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="330d3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="330d3-123">Authorization</span></span>|<span data-ttu-id="330d3-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="330d3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="330d3-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="330d3-125">Accept</span></span>|<span data-ttu-id="330d3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="330d3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="330d3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="330d3-127">Request body</span></span>
<span data-ttu-id="330d3-128">Geben Sie im Textkörper Anforderung für das Objekt [IosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="330d3-128">In the request body, supply a JSON representation for the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

<span data-ttu-id="330d3-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [IosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="330d3-129">The following table shows the properties that are required when you create the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md).</span></span>

|<span data-ttu-id="330d3-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="330d3-130">Property</span></span>|<span data-ttu-id="330d3-131">Typ</span><span class="sxs-lookup"><span data-stu-id="330d3-131">Type</span></span>|<span data-ttu-id="330d3-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="330d3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="330d3-133">id</span><span class="sxs-lookup"><span data-stu-id="330d3-133">id</span></span>|<span data-ttu-id="330d3-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="330d3-134">String</span></span>|<span data-ttu-id="330d3-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="330d3-135">Key of the entity.</span></span> <span data-ttu-id="330d3-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="330d3-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="330d3-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="330d3-137">lastModifiedDateTime</span></span>|<span data-ttu-id="330d3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="330d3-138">DateTimeOffset</span></span>|<span data-ttu-id="330d3-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="330d3-139">DateTime the object was last modified.</span></span> <span data-ttu-id="330d3-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="330d3-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="330d3-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="330d3-141">roleScopeTagIds</span></span>|<span data-ttu-id="330d3-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="330d3-142">String collection</span></span>|<span data-ttu-id="330d3-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="330d3-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="330d3-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="330d3-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="330d3-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="330d3-145">supportsScopeTags</span></span>|<span data-ttu-id="330d3-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="330d3-146">Boolean</span></span>|<span data-ttu-id="330d3-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="330d3-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="330d3-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="330d3-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="330d3-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="330d3-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="330d3-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="330d3-150">This property is read-only.</span></span> <span data-ttu-id="330d3-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="330d3-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="330d3-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="330d3-152">createdDateTime</span></span>|<span data-ttu-id="330d3-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="330d3-153">DateTimeOffset</span></span>|<span data-ttu-id="330d3-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="330d3-154">DateTime the object was created.</span></span> <span data-ttu-id="330d3-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="330d3-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="330d3-156">description</span><span class="sxs-lookup"><span data-stu-id="330d3-156">description</span></span>|<span data-ttu-id="330d3-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="330d3-157">String</span></span>|<span data-ttu-id="330d3-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="330d3-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="330d3-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="330d3-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="330d3-160">displayName</span><span class="sxs-lookup"><span data-stu-id="330d3-160">displayName</span></span>|<span data-ttu-id="330d3-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="330d3-161">String</span></span>|<span data-ttu-id="330d3-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="330d3-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="330d3-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="330d3-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="330d3-164">Version</span><span class="sxs-lookup"><span data-stu-id="330d3-164">version</span></span>|<span data-ttu-id="330d3-165">Int32</span><span class="sxs-lookup"><span data-stu-id="330d3-165">Int32</span></span>|<span data-ttu-id="330d3-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="330d3-166">Version of the device configuration.</span></span> <span data-ttu-id="330d3-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="330d3-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="330d3-168">teacherCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="330d3-168">teacherCertificateSettings</span></span>|[<span data-ttu-id="330d3-169">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="330d3-169">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="330d3-170">Die Trusted Root und PFX-Zertifikate für Lehrer</span><span class="sxs-lookup"><span data-stu-id="330d3-170">The Trusted Root and PFX certificates for Teacher</span></span>|
|<span data-ttu-id="330d3-171">studentCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="330d3-171">studentCertificateSettings</span></span>|[<span data-ttu-id="330d3-172">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="330d3-172">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="330d3-173">Die Trusted Root und PFX-Zertifikate für Schüler</span><span class="sxs-lookup"><span data-stu-id="330d3-173">The Trusted Root and PFX certificates for Student</span></span>|
|<span data-ttu-id="330d3-174">deviceCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="330d3-174">deviceCertificateSettings</span></span>|[<span data-ttu-id="330d3-175">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="330d3-175">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="330d3-176">Die Trusted Root und PFX-Zertifikate für Geräte</span><span class="sxs-lookup"><span data-stu-id="330d3-176">The Trusted Root and PFX certificates for Device</span></span>|



## <a name="response"></a><span data-ttu-id="330d3-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="330d3-177">Response</span></span>
<span data-ttu-id="330d3-178">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [IosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="330d3-178">If successful, this method returns a `200 OK` response code and an updated [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="330d3-179">Beispiel</span><span class="sxs-lookup"><span data-stu-id="330d3-179">Example</span></span>
### <a name="request"></a><span data-ttu-id="330d3-180">Anforderung</span><span class="sxs-lookup"><span data-stu-id="330d3-180">Request</span></span>
<span data-ttu-id="330d3-181">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="330d3-181">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1910

{
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

### <a name="response"></a><span data-ttu-id="330d3-182">Antwort</span><span class="sxs-lookup"><span data-stu-id="330d3-182">Response</span></span>
<span data-ttu-id="330d3-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="330d3-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





