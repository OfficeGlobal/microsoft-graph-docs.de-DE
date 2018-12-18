---
title: WindowsPhone81SCEPCertificateProfile aktualisieren
description: Aktualisieren Sie die Eigenschaften eines windowsPhone81SCEPCertificateProfile-Objekts.
author: tfitzmac
ms.openlocfilehash: 595041128c49a5efc5f71ee991717df25f1da81e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321679"
---
# <a name="update-windowsphone81scepcertificateprofile"></a><span data-ttu-id="10333-103">WindowsPhone81SCEPCertificateProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="10333-103">Update windowsPhone81SCEPCertificateProfile</span></span>

> <span data-ttu-id="10333-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="10333-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="10333-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="10333-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="10333-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="10333-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10333-107">Aktualisieren Sie die Eigenschaften eines [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="10333-107">Update the properties of a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="10333-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="10333-108">Prerequisites</span></span>
<span data-ttu-id="10333-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10333-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10333-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="10333-111">Permission type</span></span>|<span data-ttu-id="10333-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="10333-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10333-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="10333-113">Delegated (work or school account)</span></span>|<span data-ttu-id="10333-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10333-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="10333-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="10333-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10333-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="10333-116">Not supported.</span></span>|
|<span data-ttu-id="10333-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="10333-117">Application</span></span>|<span data-ttu-id="10333-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="10333-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10333-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="10333-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="10333-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="10333-120">Request headers</span></span>
|<span data-ttu-id="10333-121">Header</span><span class="sxs-lookup"><span data-stu-id="10333-121">Header</span></span>|<span data-ttu-id="10333-122">Wert</span><span class="sxs-lookup"><span data-stu-id="10333-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10333-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="10333-123">Authorization</span></span>|<span data-ttu-id="10333-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="10333-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10333-125">Accept</span><span class="sxs-lookup"><span data-stu-id="10333-125">Accept</span></span>|<span data-ttu-id="10333-126">application/json</span><span class="sxs-lookup"><span data-stu-id="10333-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10333-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="10333-127">Request body</span></span>
<span data-ttu-id="10333-128">Geben Sie im Textkörper Anforderung für das Objekt [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="10333-128">In the request body, supply a JSON representation for the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

<span data-ttu-id="10333-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="10333-129">The following table shows the properties that are required when you create the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md).</span></span>

|<span data-ttu-id="10333-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="10333-130">Property</span></span>|<span data-ttu-id="10333-131">Typ</span><span class="sxs-lookup"><span data-stu-id="10333-131">Type</span></span>|<span data-ttu-id="10333-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="10333-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10333-133">id</span><span class="sxs-lookup"><span data-stu-id="10333-133">id</span></span>|<span data-ttu-id="10333-134">String</span><span class="sxs-lookup"><span data-stu-id="10333-134">String</span></span>|<span data-ttu-id="10333-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="10333-135">Key of the entity.</span></span> <span data-ttu-id="10333-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10333-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10333-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="10333-137">lastModifiedDateTime</span></span>|<span data-ttu-id="10333-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10333-138">DateTimeOffset</span></span>|<span data-ttu-id="10333-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="10333-139">DateTime the object was last modified.</span></span> <span data-ttu-id="10333-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10333-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10333-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="10333-141">roleScopeTagIds</span></span>|<span data-ttu-id="10333-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="10333-142">String collection</span></span>|<span data-ttu-id="10333-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="10333-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="10333-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10333-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10333-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="10333-145">supportsScopeTags</span></span>|<span data-ttu-id="10333-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="10333-146">Boolean</span></span>|<span data-ttu-id="10333-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="10333-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="10333-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="10333-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="10333-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="10333-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="10333-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="10333-150">This property is read-only.</span></span> <span data-ttu-id="10333-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10333-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10333-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="10333-152">createdDateTime</span></span>|<span data-ttu-id="10333-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10333-153">DateTimeOffset</span></span>|<span data-ttu-id="10333-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="10333-154">DateTime the object was created.</span></span> <span data-ttu-id="10333-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10333-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10333-156">description</span><span class="sxs-lookup"><span data-stu-id="10333-156">description</span></span>|<span data-ttu-id="10333-157">String</span><span class="sxs-lookup"><span data-stu-id="10333-157">String</span></span>|<span data-ttu-id="10333-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="10333-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="10333-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10333-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10333-160">displayName</span><span class="sxs-lookup"><span data-stu-id="10333-160">displayName</span></span>|<span data-ttu-id="10333-161">String</span><span class="sxs-lookup"><span data-stu-id="10333-161">String</span></span>|<span data-ttu-id="10333-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="10333-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="10333-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10333-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10333-164">Version</span><span class="sxs-lookup"><span data-stu-id="10333-164">version</span></span>|<span data-ttu-id="10333-165">Int32</span><span class="sxs-lookup"><span data-stu-id="10333-165">Int32</span></span>|<span data-ttu-id="10333-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="10333-166">Version of the device configuration.</span></span> <span data-ttu-id="10333-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10333-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10333-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="10333-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="10333-169">Int32</span><span class="sxs-lookup"><span data-stu-id="10333-169">Int32</span></span>|<span data-ttu-id="10333-170">Zertifikat Erneuerung Schwellenwertprozentsatz.</span><span class="sxs-lookup"><span data-stu-id="10333-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="10333-171">Geerbt von [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="10333-171">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="10333-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="10333-172">keyStorageProvider</span></span>|[<span data-ttu-id="10333-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="10333-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="10333-174">Wichtige Speicheranbieter (KSP).</span><span class="sxs-lookup"><span data-stu-id="10333-174">Key Storage Provider (KSP).</span></span> <span data-ttu-id="10333-175">Geerbt von [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="10333-175">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="10333-176">Mögliche Werte: sind `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail` und `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="10333-176">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="10333-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="10333-177">subjectNameFormat</span></span>|[<span data-ttu-id="10333-178">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="10333-178">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="10333-179">Format des Antragstellernamen Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="10333-179">Certificate Subject Name Format.</span></span> <span data-ttu-id="10333-180">Geerbt von [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="10333-180">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="10333-181">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="10333-181">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="10333-182">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="10333-182">subjectAlternativeNameType</span></span>|[<span data-ttu-id="10333-183">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="10333-183">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="10333-184">Subject Alternative Name Zertifikattyp.</span><span class="sxs-lookup"><span data-stu-id="10333-184">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="10333-185">Geerbt von [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="10333-185">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="10333-186">Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="10333-186">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="10333-187">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="10333-187">certificateValidityPeriodValue</span></span>|<span data-ttu-id="10333-188">Int32</span><span class="sxs-lookup"><span data-stu-id="10333-188">Int32</span></span>|<span data-ttu-id="10333-189">Der Wert für das Zertifikat Validtiy Zeitraum.</span><span class="sxs-lookup"><span data-stu-id="10333-189">Value for the Certificate Validtiy Period.</span></span> <span data-ttu-id="10333-190">Geerbt von [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="10333-190">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="10333-191">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="10333-191">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="10333-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="10333-192">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="10333-193">Skalierung für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="10333-193">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="10333-194">Geerbt von [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="10333-194">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="10333-195">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="10333-195">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="10333-196">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="10333-196">extendedKeyUsages</span></span>|<span data-ttu-id="10333-197">[ExtendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="10333-197">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="10333-198">Erweiterte Schlüsselverwendung (EKU)-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="10333-198">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="10333-199">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="10333-199">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="10333-200">Geerbt von [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="10333-200">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="10333-201">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="10333-201">scepServerUrls</span></span>|<span data-ttu-id="10333-202">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="10333-202">String collection</span></span>|<span data-ttu-id="10333-203">SCEP Server URL(s) hinzu.</span><span class="sxs-lookup"><span data-stu-id="10333-203">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="10333-204">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="10333-204">subjectNameFormatString</span></span>|<span data-ttu-id="10333-205">String</span><span class="sxs-lookup"><span data-stu-id="10333-205">String</span></span>|<span data-ttu-id="10333-206">Benutzerdefiniertes Format zur Verwendung mit SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="10333-206">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="10333-207">Beispiel: CN = {{EmailAddress}} E = {{EmailAddress}}, OU = Unternehmensbenutzer, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="10333-207">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="10333-208">Schlüsselverwendung</span><span class="sxs-lookup"><span data-stu-id="10333-208">keyUsage</span></span>|[<span data-ttu-id="10333-209">keyUsages</span><span class="sxs-lookup"><span data-stu-id="10333-209">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="10333-210">SCEP Enhanced Key Usage.</span><span class="sxs-lookup"><span data-stu-id="10333-210">SCEP Key Usage.</span></span> <span data-ttu-id="10333-211">Mögliche Werte sind: `keyEncipherment` und `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="10333-211">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="10333-212">keySize</span><span class="sxs-lookup"><span data-stu-id="10333-212">keySize</span></span>|[<span data-ttu-id="10333-213">keySize</span><span class="sxs-lookup"><span data-stu-id="10333-213">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="10333-214">Wichtige SCEP-Größe.</span><span class="sxs-lookup"><span data-stu-id="10333-214">SCEP Key Size.</span></span> <span data-ttu-id="10333-215">Mögliche Werte sind: `size1024` und `size2048`.</span><span class="sxs-lookup"><span data-stu-id="10333-215">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="10333-216">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="10333-216">hashAlgorithm</span></span>|[<span data-ttu-id="10333-217">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="10333-217">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="10333-218">SCEP Hashalgorithmus.</span><span class="sxs-lookup"><span data-stu-id="10333-218">SCEP Hash Algorithm.</span></span> <span data-ttu-id="10333-219">Mögliche Werte sind: `sha1` und `sha2`.</span><span class="sxs-lookup"><span data-stu-id="10333-219">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="10333-220">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="10333-220">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="10333-221">String</span><span class="sxs-lookup"><span data-stu-id="10333-221">String</span></span>|<span data-ttu-id="10333-222">Benutzerdefinierte Zeichenfolge, die die AAD-Attribut definiert.</span><span class="sxs-lookup"><span data-stu-id="10333-222">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="10333-223">Antwort</span><span class="sxs-lookup"><span data-stu-id="10333-223">Response</span></span>
<span data-ttu-id="10333-224">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="10333-224">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10333-225">Beispiel</span><span class="sxs-lookup"><span data-stu-id="10333-225">Example</span></span>
### <a name="request"></a><span data-ttu-id="10333-226">Anforderung</span><span class="sxs-lookup"><span data-stu-id="10333-226">Request</span></span>
<span data-ttu-id="10333-227">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="10333-227">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1021

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="10333-228">Antwort</span><span class="sxs-lookup"><span data-stu-id="10333-228">Response</span></span>
<span data-ttu-id="10333-p122">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="10333-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1204

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
  "id": "f070e30e-e30e-f070-0ee3-70f00ee370f0",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```





