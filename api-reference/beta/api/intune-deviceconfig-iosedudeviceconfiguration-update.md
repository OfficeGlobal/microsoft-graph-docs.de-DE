---
title: IosEduDeviceConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines iosEduDeviceConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ff10904bb7299dcacbdcc48e358e1a898ff3a5fc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171505"
---
# <a name="update-iosedudeviceconfiguration"></a><span data-ttu-id="6470f-103">IosEduDeviceConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6470f-103">Update iosEduDeviceConfiguration</span></span>

> <span data-ttu-id="6470f-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6470f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6470f-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6470f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6470f-106">Aktualisieren der Eigenschaften eines [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6470f-106">Update the properties of a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6470f-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6470f-107">Prerequisites</span></span>
<span data-ttu-id="6470f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6470f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6470f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6470f-110">Permission type</span></span>|<span data-ttu-id="6470f-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6470f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6470f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6470f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6470f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6470f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6470f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6470f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6470f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6470f-115">Not supported.</span></span>|
|<span data-ttu-id="6470f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6470f-116">Application</span></span>|<span data-ttu-id="6470f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6470f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6470f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6470f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6470f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6470f-119">Request headers</span></span>
|<span data-ttu-id="6470f-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6470f-120">Header</span></span>|<span data-ttu-id="6470f-121">Wert</span><span class="sxs-lookup"><span data-stu-id="6470f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6470f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6470f-122">Authorization</span></span>|<span data-ttu-id="6470f-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6470f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6470f-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6470f-124">Accept</span></span>|<span data-ttu-id="6470f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6470f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6470f-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6470f-126">Request body</span></span>
<span data-ttu-id="6470f-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="6470f-127">In the request body, supply a JSON representation for the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

<span data-ttu-id="6470f-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="6470f-128">The following table shows the properties that are required when you create the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md).</span></span>

|<span data-ttu-id="6470f-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6470f-129">Property</span></span>|<span data-ttu-id="6470f-130">Typ</span><span class="sxs-lookup"><span data-stu-id="6470f-130">Type</span></span>|<span data-ttu-id="6470f-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6470f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6470f-132">id</span><span class="sxs-lookup"><span data-stu-id="6470f-132">id</span></span>|<span data-ttu-id="6470f-133">string</span><span class="sxs-lookup"><span data-stu-id="6470f-133">String</span></span>|<span data-ttu-id="6470f-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6470f-134">Key of the entity.</span></span> <span data-ttu-id="6470f-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6470f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6470f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6470f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6470f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6470f-137">DateTimeOffset</span></span>|<span data-ttu-id="6470f-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="6470f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6470f-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6470f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6470f-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="6470f-140">roleScopeTagIds</span></span>|<span data-ttu-id="6470f-141">String collection</span><span class="sxs-lookup"><span data-stu-id="6470f-141">String collection</span></span>|<span data-ttu-id="6470f-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="6470f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6470f-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6470f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6470f-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6470f-144">supportsScopeTags</span></span>|<span data-ttu-id="6470f-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6470f-145">Boolean</span></span>|<span data-ttu-id="6470f-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6470f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6470f-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="6470f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6470f-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="6470f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6470f-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6470f-149">This property is read-only.</span></span> <span data-ttu-id="6470f-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6470f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6470f-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6470f-151">createdDateTime</span></span>|<span data-ttu-id="6470f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6470f-152">DateTimeOffset</span></span>|<span data-ttu-id="6470f-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="6470f-153">DateTime the object was created.</span></span> <span data-ttu-id="6470f-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6470f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6470f-155">description</span><span class="sxs-lookup"><span data-stu-id="6470f-155">description</span></span>|<span data-ttu-id="6470f-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6470f-156">String</span></span>|<span data-ttu-id="6470f-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="6470f-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6470f-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6470f-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6470f-159">displayName</span><span class="sxs-lookup"><span data-stu-id="6470f-159">displayName</span></span>|<span data-ttu-id="6470f-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6470f-160">String</span></span>|<span data-ttu-id="6470f-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="6470f-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6470f-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6470f-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6470f-163">Version</span><span class="sxs-lookup"><span data-stu-id="6470f-163">version</span></span>|<span data-ttu-id="6470f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="6470f-164">Int32</span></span>|<span data-ttu-id="6470f-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="6470f-165">Version of the device configuration.</span></span> <span data-ttu-id="6470f-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6470f-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6470f-167">teacherCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="6470f-167">teacherCertificateSettings</span></span>|[<span data-ttu-id="6470f-168">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="6470f-168">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="6470f-169">Die vertrauenswürdigen Stamm-und PFX-Zertifikate für Lehrer</span><span class="sxs-lookup"><span data-stu-id="6470f-169">The Trusted Root and PFX certificates for Teacher</span></span>|
|<span data-ttu-id="6470f-170">studentCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="6470f-170">studentCertificateSettings</span></span>|[<span data-ttu-id="6470f-171">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="6470f-171">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="6470f-172">Die vertrauenswürdigen Stamm-und PFX-Zertifikate für Schüler</span><span class="sxs-lookup"><span data-stu-id="6470f-172">The Trusted Root and PFX certificates for Student</span></span>|
|<span data-ttu-id="6470f-173">deviceCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="6470f-173">deviceCertificateSettings</span></span>|[<span data-ttu-id="6470f-174">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="6470f-174">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="6470f-175">Die vertrauenswürdigen Stamm-und PFX-Zertifikate für Device</span><span class="sxs-lookup"><span data-stu-id="6470f-175">The Trusted Root and PFX certificates for Device</span></span>|



## <a name="response"></a><span data-ttu-id="6470f-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="6470f-176">Response</span></span>
<span data-ttu-id="6470f-177">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6470f-177">If successful, this method returns a `200 OK` response code and an updated [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6470f-178">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6470f-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="6470f-179">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6470f-179">Request</span></span>
<span data-ttu-id="6470f-180">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6470f-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1910

{
  "@odata.type": "#microsoft.graph.iosEduDeviceConfiguration",
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

### <a name="response"></a><span data-ttu-id="6470f-181">Antwort</span><span class="sxs-lookup"><span data-stu-id="6470f-181">Response</span></span>
<span data-ttu-id="6470f-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6470f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




