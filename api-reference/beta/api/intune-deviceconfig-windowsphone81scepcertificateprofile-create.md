---
title: Erstellen von windowsPhone81SCEPCertificateProfile
description: Erstellen eines neuen windowsPhone81SCEPCertificateProfile-Objekts.
ms.openlocfilehash: 16e06b5b323fb0ce12593e7ec5561a92f1fe2b80
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060114"
---
# <a name="create-windowsphone81scepcertificateprofile"></a><span data-ttu-id="ac9ec-103">Erstellen von windowsPhone81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="ac9ec-103">Create windowsPhone81SCEPCertificateProfile</span></span>

> <span data-ttu-id="ac9ec-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ac9ec-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ac9ec-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ac9ec-107">Erstellen eines neuen [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-107">Create a new [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ac9ec-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ac9ec-108">Prerequisites</span></span>
<span data-ttu-id="ac9ec-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac9ec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac9ec-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ac9ec-111">Permission type</span></span>|<span data-ttu-id="ac9ec-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ac9ec-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac9ec-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ac9ec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ac9ec-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac9ec-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ac9ec-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ac9ec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac9ec-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ac9ec-116">Not supported.</span></span>|
|<span data-ttu-id="ac9ec-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ac9ec-117">Application</span></span>|<span data-ttu-id="ac9ec-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ac9ec-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac9ec-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ac9ec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ac9ec-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ac9ec-120">Request headers</span></span>
|<span data-ttu-id="ac9ec-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ac9ec-121">Header</span></span>|<span data-ttu-id="ac9ec-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ac9ec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac9ec-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac9ec-123">Authorization</span></span>|<span data-ttu-id="ac9ec-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ac9ec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac9ec-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ac9ec-125">Accept</span></span>|<span data-ttu-id="ac9ec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ac9ec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac9ec-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ac9ec-127">Request body</span></span>
<span data-ttu-id="ac9ec-128">Geben Sie im Textkörper Anforderung für das Objekt windowsPhone81SCEPCertificateProfile eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-128">In the request body, supply a JSON representation for the windowsPhone81SCEPCertificateProfile object.</span></span>

<span data-ttu-id="ac9ec-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die windowsPhone81SCEPCertificateProfile erstellen.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-129">The following table shows the properties that are required when you create the windowsPhone81SCEPCertificateProfile.</span></span>

|<span data-ttu-id="ac9ec-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ac9ec-130">Property</span></span>|<span data-ttu-id="ac9ec-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ac9ec-131">Type</span></span>|<span data-ttu-id="ac9ec-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ac9ec-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac9ec-133">id</span><span class="sxs-lookup"><span data-stu-id="ac9ec-133">id</span></span>|<span data-ttu-id="ac9ec-134">String</span><span class="sxs-lookup"><span data-stu-id="ac9ec-134">String</span></span>|<span data-ttu-id="ac9ec-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ac9ec-135">Key of the entity.</span></span> <span data-ttu-id="ac9ec-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac9ec-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac9ec-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ac9ec-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ac9ec-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac9ec-138">DateTimeOffset</span></span>|<span data-ttu-id="ac9ec-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ac9ec-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac9ec-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac9ec-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ac9ec-141">roleScopeTagIds</span></span>|<span data-ttu-id="ac9ec-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="ac9ec-142">String collection</span></span>|<span data-ttu-id="ac9ec-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ac9ec-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac9ec-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac9ec-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ac9ec-145">supportsScopeTags</span></span>|<span data-ttu-id="ac9ec-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="ac9ec-146">Boolean</span></span>|<span data-ttu-id="ac9ec-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ac9ec-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ac9ec-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ac9ec-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-150">This property is read-only.</span></span> <span data-ttu-id="ac9ec-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac9ec-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac9ec-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ac9ec-152">createdDateTime</span></span>|<span data-ttu-id="ac9ec-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac9ec-153">DateTimeOffset</span></span>|<span data-ttu-id="ac9ec-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-154">DateTime the object was created.</span></span> <span data-ttu-id="ac9ec-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac9ec-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac9ec-156">description</span><span class="sxs-lookup"><span data-stu-id="ac9ec-156">description</span></span>|<span data-ttu-id="ac9ec-157">String</span><span class="sxs-lookup"><span data-stu-id="ac9ec-157">String</span></span>|<span data-ttu-id="ac9ec-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ac9ec-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ac9ec-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac9ec-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac9ec-160">displayName</span><span class="sxs-lookup"><span data-stu-id="ac9ec-160">displayName</span></span>|<span data-ttu-id="ac9ec-161">String</span><span class="sxs-lookup"><span data-stu-id="ac9ec-161">String</span></span>|<span data-ttu-id="ac9ec-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="ac9ec-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ac9ec-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac9ec-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac9ec-164">Version</span><span class="sxs-lookup"><span data-stu-id="ac9ec-164">version</span></span>|<span data-ttu-id="ac9ec-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ac9ec-165">Int32</span></span>|<span data-ttu-id="ac9ec-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-166">Version of the device configuration.</span></span> <span data-ttu-id="ac9ec-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac9ec-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac9ec-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="ac9ec-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="ac9ec-169">Int32</span><span class="sxs-lookup"><span data-stu-id="ac9ec-169">Int32</span></span>|<span data-ttu-id="ac9ec-170">Zertifikat Erneuerung Schwellenwertprozentsatz.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="ac9ec-171">Geerbt von [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ac9ec-171">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="ac9ec-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="ac9ec-172">keyStorageProvider</span></span>|[<span data-ttu-id="ac9ec-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="ac9ec-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="ac9ec-174">Wichtige Speicheranbieter (KSP).</span><span class="sxs-lookup"><span data-stu-id="ac9ec-174">Key Storage Provider (KSP).</span></span> <span data-ttu-id="ac9ec-175">Geerbt von [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ac9ec-175">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="ac9ec-176">Mögliche Werte: sind `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail` und `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-176">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="ac9ec-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="ac9ec-177">subjectNameFormat</span></span>|[<span data-ttu-id="ac9ec-178">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="ac9ec-178">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="ac9ec-179">Format des Antragstellernamen Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-179">Certificate Subject Name Format.</span></span> <span data-ttu-id="ac9ec-180">Geerbt von [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ac9ec-180">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="ac9ec-181">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-181">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="ac9ec-182">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ac9ec-182">subjectAlternativeNameType</span></span>|[<span data-ttu-id="ac9ec-183">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ac9ec-183">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="ac9ec-184">Subject Alternative Name Zertifikattyp.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-184">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="ac9ec-185">Geerbt von [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ac9ec-185">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="ac9ec-186">Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-186">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="ac9ec-187">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="ac9ec-187">certificateValidityPeriodValue</span></span>|<span data-ttu-id="ac9ec-188">Int32</span><span class="sxs-lookup"><span data-stu-id="ac9ec-188">Int32</span></span>|<span data-ttu-id="ac9ec-189">Der Wert für das Zertifikat Validtiy Zeitraum.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-189">Value for the Certificate Validtiy Period.</span></span> <span data-ttu-id="ac9ec-190">Geerbt von [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ac9ec-190">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="ac9ec-191">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ac9ec-191">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="ac9ec-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ac9ec-192">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="ac9ec-193">Skalierung für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-193">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="ac9ec-194">Geerbt von [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ac9ec-194">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="ac9ec-195">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-195">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="ac9ec-196">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="ac9ec-196">extendedKeyUsages</span></span>|<span data-ttu-id="ac9ec-197">[ExtendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="ac9ec-197">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="ac9ec-198">Erweiterte Schlüsselverwendung (EKU)-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-198">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="ac9ec-199">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-199">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="ac9ec-200">Geerbt von [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ac9ec-200">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="ac9ec-201">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="ac9ec-201">scepServerUrls</span></span>|<span data-ttu-id="ac9ec-202">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="ac9ec-202">String collection</span></span>|<span data-ttu-id="ac9ec-203">SCEP Server URL(s) hinzu.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-203">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="ac9ec-204">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="ac9ec-204">subjectNameFormatString</span></span>|<span data-ttu-id="ac9ec-205">String</span><span class="sxs-lookup"><span data-stu-id="ac9ec-205">String</span></span>|<span data-ttu-id="ac9ec-206">Benutzerdefiniertes Format zur Verwendung mit SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-206">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="ac9ec-207">Beispiel: CN = {{EmailAddress}} E = {{EmailAddress}}, OU = Unternehmensbenutzer, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="ac9ec-207">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="ac9ec-208">Schlüsselverwendung</span><span class="sxs-lookup"><span data-stu-id="ac9ec-208">keyUsage</span></span>|[<span data-ttu-id="ac9ec-209">keyUsages</span><span class="sxs-lookup"><span data-stu-id="ac9ec-209">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="ac9ec-210">SCEP Enhanced Key Usage.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-210">SCEP Key Usage.</span></span> <span data-ttu-id="ac9ec-211">Mögliche Werte sind: `keyEncipherment` und `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-211">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="ac9ec-212">keySize</span><span class="sxs-lookup"><span data-stu-id="ac9ec-212">keySize</span></span>|[<span data-ttu-id="ac9ec-213">keySize</span><span class="sxs-lookup"><span data-stu-id="ac9ec-213">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="ac9ec-214">Wichtige SCEP-Größe.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-214">SCEP Key Size.</span></span> <span data-ttu-id="ac9ec-215">Mögliche Werte sind: `size1024` und `size2048`.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-215">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="ac9ec-216">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="ac9ec-216">hashAlgorithm</span></span>|[<span data-ttu-id="ac9ec-217">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="ac9ec-217">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="ac9ec-218">SCEP Hashalgorithmus.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-218">SCEP Hash Algorithm.</span></span> <span data-ttu-id="ac9ec-219">Mögliche Werte sind: `sha1` und `sha2`.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-219">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="ac9ec-220">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="ac9ec-220">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="ac9ec-221">String</span><span class="sxs-lookup"><span data-stu-id="ac9ec-221">String</span></span>|<span data-ttu-id="ac9ec-222">Benutzerdefinierte Zeichenfolge, die die AAD-Attribut definiert.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-222">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="ac9ec-223">Antwort</span><span class="sxs-lookup"><span data-stu-id="ac9ec-223">Response</span></span>
<span data-ttu-id="ac9ec-224">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-224">If successful, this method returns a `201 Created` response code and a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac9ec-225">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ac9ec-225">Example</span></span>
### <a name="request"></a><span data-ttu-id="ac9ec-226">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ac9ec-226">Request</span></span>
<span data-ttu-id="ac9ec-227">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-227">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1096

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="ac9ec-228">Antwort</span><span class="sxs-lookup"><span data-stu-id="ac9ec-228">Response</span></span>
<span data-ttu-id="ac9ec-p122">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ac9ec-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





