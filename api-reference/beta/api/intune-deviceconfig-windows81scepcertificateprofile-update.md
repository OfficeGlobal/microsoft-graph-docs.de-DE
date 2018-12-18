---
title: Windows81SCEPCertificateProfile aktualisieren
description: Aktualisieren Sie die Eigenschaften eines windows81SCEPCertificateProfile-Objekts.
author: tfitzmac
ms.openlocfilehash: 39571d85a1eb7d9a2d5d0a18f178fb2cb1be7e02
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338220"
---
# <a name="update-windows81scepcertificateprofile"></a><span data-ttu-id="489b3-103">Windows81SCEPCertificateProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="489b3-103">Update windows81SCEPCertificateProfile</span></span>

> <span data-ttu-id="489b3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="489b3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="489b3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="489b3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="489b3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="489b3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="489b3-107">Aktualisieren Sie die Eigenschaften eines [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="489b3-107">Update the properties of a [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="489b3-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="489b3-108">Prerequisites</span></span>
<span data-ttu-id="489b3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="489b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="489b3-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="489b3-111">Permission type</span></span>|<span data-ttu-id="489b3-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="489b3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="489b3-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="489b3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="489b3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="489b3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="489b3-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="489b3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="489b3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="489b3-116">Not supported.</span></span>|
|<span data-ttu-id="489b3-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="489b3-117">Application</span></span>|<span data-ttu-id="489b3-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="489b3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="489b3-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="489b3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="489b3-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="489b3-120">Request headers</span></span>
|<span data-ttu-id="489b3-121">Header</span><span class="sxs-lookup"><span data-stu-id="489b3-121">Header</span></span>|<span data-ttu-id="489b3-122">Wert</span><span class="sxs-lookup"><span data-stu-id="489b3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="489b3-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="489b3-123">Authorization</span></span>|<span data-ttu-id="489b3-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="489b3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="489b3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="489b3-125">Accept</span></span>|<span data-ttu-id="489b3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="489b3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="489b3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="489b3-127">Request body</span></span>
<span data-ttu-id="489b3-128">Geben Sie im Textkörper Anforderung für das Objekt [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="489b3-128">In the request body, supply a JSON representation for the [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

<span data-ttu-id="489b3-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="489b3-129">The following table shows the properties that are required when you create the [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md).</span></span>

|<span data-ttu-id="489b3-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="489b3-130">Property</span></span>|<span data-ttu-id="489b3-131">Typ</span><span class="sxs-lookup"><span data-stu-id="489b3-131">Type</span></span>|<span data-ttu-id="489b3-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="489b3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="489b3-133">id</span><span class="sxs-lookup"><span data-stu-id="489b3-133">id</span></span>|<span data-ttu-id="489b3-134">String</span><span class="sxs-lookup"><span data-stu-id="489b3-134">String</span></span>|<span data-ttu-id="489b3-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="489b3-135">Key of the entity.</span></span> <span data-ttu-id="489b3-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="489b3-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="489b3-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="489b3-137">lastModifiedDateTime</span></span>|<span data-ttu-id="489b3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="489b3-138">DateTimeOffset</span></span>|<span data-ttu-id="489b3-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="489b3-139">DateTime the object was last modified.</span></span> <span data-ttu-id="489b3-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="489b3-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="489b3-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="489b3-141">roleScopeTagIds</span></span>|<span data-ttu-id="489b3-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="489b3-142">String collection</span></span>|<span data-ttu-id="489b3-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="489b3-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="489b3-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="489b3-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="489b3-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="489b3-145">supportsScopeTags</span></span>|<span data-ttu-id="489b3-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="489b3-146">Boolean</span></span>|<span data-ttu-id="489b3-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="489b3-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="489b3-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="489b3-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="489b3-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="489b3-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="489b3-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="489b3-150">This property is read-only.</span></span> <span data-ttu-id="489b3-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="489b3-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="489b3-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="489b3-152">createdDateTime</span></span>|<span data-ttu-id="489b3-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="489b3-153">DateTimeOffset</span></span>|<span data-ttu-id="489b3-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="489b3-154">DateTime the object was created.</span></span> <span data-ttu-id="489b3-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="489b3-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="489b3-156">description</span><span class="sxs-lookup"><span data-stu-id="489b3-156">description</span></span>|<span data-ttu-id="489b3-157">String</span><span class="sxs-lookup"><span data-stu-id="489b3-157">String</span></span>|<span data-ttu-id="489b3-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="489b3-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="489b3-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="489b3-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="489b3-160">displayName</span><span class="sxs-lookup"><span data-stu-id="489b3-160">displayName</span></span>|<span data-ttu-id="489b3-161">String</span><span class="sxs-lookup"><span data-stu-id="489b3-161">String</span></span>|<span data-ttu-id="489b3-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="489b3-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="489b3-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="489b3-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="489b3-164">Version</span><span class="sxs-lookup"><span data-stu-id="489b3-164">version</span></span>|<span data-ttu-id="489b3-165">Int32</span><span class="sxs-lookup"><span data-stu-id="489b3-165">Int32</span></span>|<span data-ttu-id="489b3-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="489b3-166">Version of the device configuration.</span></span> <span data-ttu-id="489b3-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="489b3-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="489b3-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="489b3-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="489b3-169">Int32</span><span class="sxs-lookup"><span data-stu-id="489b3-169">Int32</span></span>|<span data-ttu-id="489b3-170">Zertifikat Erneuerung Schwellenwertprozentsatz.</span><span class="sxs-lookup"><span data-stu-id="489b3-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="489b3-171">Gültige Werte 1 bis 99 Inherited aus [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="489b3-171">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="489b3-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="489b3-172">keyStorageProvider</span></span>|[<span data-ttu-id="489b3-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="489b3-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="489b3-174">Schlüssel-Speicher-Anbieter (KSP) Inherited aus [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="489b3-174">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="489b3-175">Mögliche Werte: sind `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail` und `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="489b3-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="489b3-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="489b3-176">subjectNameFormat</span></span>|[<span data-ttu-id="489b3-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="489b3-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="489b3-178">Zertifikat Subject Name Format geerbt von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="489b3-178">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="489b3-179">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="489b3-179">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="489b3-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="489b3-180">subjectAlternativeNameType</span></span>|[<span data-ttu-id="489b3-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="489b3-181">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="489b3-182">Zertifikat Subject Alternative Name Typ geerbt von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="489b3-182">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="489b3-183">Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="489b3-183">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="489b3-184">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="489b3-184">certificateValidityPeriodValue</span></span>|<span data-ttu-id="489b3-185">Int32</span><span class="sxs-lookup"><span data-stu-id="489b3-185">Int32</span></span>|<span data-ttu-id="489b3-186">Wert für das Zertifikat Gültigkeit Zeitraum geerbt von [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="489b3-186">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="489b3-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="489b3-187">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="489b3-188">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="489b3-188">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="489b3-189">Skalierung für das Zertifikat Gültigkeit Zeitraum geerbt von [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="489b3-189">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="489b3-190">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="489b3-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="489b3-191">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="489b3-191">extendedKeyUsages</span></span>|<span data-ttu-id="489b3-192">[ExtendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="489b3-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="489b3-193">Erweiterte Schlüsselverwendung (EKU)-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="489b3-193">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="489b3-194">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="489b3-194">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="489b3-195">Geerbt von [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="489b3-195">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="489b3-196">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="489b3-196">customSubjectAlternativeNames</span></span>|<span data-ttu-id="489b3-197">[CustomSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="489b3-197">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="489b3-198">Benutzerdefinierte Subject Name Alterantive Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="489b3-198">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="489b3-199">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="489b3-199">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="489b3-200">Geerbt von [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="489b3-200">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="489b3-201">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="489b3-201">scepServerUrls</span></span>|<span data-ttu-id="489b3-202">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="489b3-202">String collection</span></span>|<span data-ttu-id="489b3-203">SCEP Server URL(s) hinzu.</span><span class="sxs-lookup"><span data-stu-id="489b3-203">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="489b3-204">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="489b3-204">subjectNameFormatString</span></span>|<span data-ttu-id="489b3-205">String</span><span class="sxs-lookup"><span data-stu-id="489b3-205">String</span></span>|<span data-ttu-id="489b3-206">Benutzerdefiniertes Format zur Verwendung mit SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="489b3-206">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="489b3-207">Beispiel: CN = {{EmailAddress}} E = {{EmailAddress}}, OU = Unternehmensbenutzer, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="489b3-207">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="489b3-208">Schlüsselverwendung</span><span class="sxs-lookup"><span data-stu-id="489b3-208">keyUsage</span></span>|[<span data-ttu-id="489b3-209">keyUsages</span><span class="sxs-lookup"><span data-stu-id="489b3-209">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="489b3-210">SCEP Enhanced Key Usage.</span><span class="sxs-lookup"><span data-stu-id="489b3-210">SCEP Key Usage.</span></span> <span data-ttu-id="489b3-211">Mögliche Werte sind: `keyEncipherment` und `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="489b3-211">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="489b3-212">keySize</span><span class="sxs-lookup"><span data-stu-id="489b3-212">keySize</span></span>|[<span data-ttu-id="489b3-213">keySize</span><span class="sxs-lookup"><span data-stu-id="489b3-213">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="489b3-214">Wichtige SCEP-Größe.</span><span class="sxs-lookup"><span data-stu-id="489b3-214">SCEP Key Size.</span></span> <span data-ttu-id="489b3-215">Mögliche Werte sind: `size1024` und `size2048`.</span><span class="sxs-lookup"><span data-stu-id="489b3-215">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="489b3-216">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="489b3-216">hashAlgorithm</span></span>|[<span data-ttu-id="489b3-217">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="489b3-217">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="489b3-218">SCEP Hashalgorithmus.</span><span class="sxs-lookup"><span data-stu-id="489b3-218">SCEP Hash Algorithm.</span></span> <span data-ttu-id="489b3-219">Mögliche Werte sind: `sha1` und `sha2`.</span><span class="sxs-lookup"><span data-stu-id="489b3-219">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="489b3-220">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="489b3-220">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="489b3-221">String</span><span class="sxs-lookup"><span data-stu-id="489b3-221">String</span></span>|<span data-ttu-id="489b3-222">Benutzerdefinierte Zeichenfolge, die die AAD-Attribut definiert.</span><span class="sxs-lookup"><span data-stu-id="489b3-222">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="489b3-223">certificateStore</span><span class="sxs-lookup"><span data-stu-id="489b3-223">certificateStore</span></span>|[<span data-ttu-id="489b3-224">certificateStore</span><span class="sxs-lookup"><span data-stu-id="489b3-224">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="489b3-225">Ziel-Zertifikatspeicher.</span><span class="sxs-lookup"><span data-stu-id="489b3-225">Target store certificate.</span></span> <span data-ttu-id="489b3-226">Mögliche Werte sind: `user` und `machine`.</span><span class="sxs-lookup"><span data-stu-id="489b3-226">Possible values are: `user`, `machine`.</span></span>|



## <a name="response"></a><span data-ttu-id="489b3-227">Antwort</span><span class="sxs-lookup"><span data-stu-id="489b3-227">Response</span></span>
<span data-ttu-id="489b3-228">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="489b3-228">If successful, this method returns a `200 OK` response code and an updated [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="489b3-229">Beispiel</span><span class="sxs-lookup"><span data-stu-id="489b3-229">Example</span></span>
### <a name="request"></a><span data-ttu-id="489b3-230">Anforderung</span><span class="sxs-lookup"><span data-stu-id="489b3-230">Request</span></span>
<span data-ttu-id="489b3-231">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="489b3-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1245

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
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine"
}
```

### <a name="response"></a><span data-ttu-id="489b3-232">Antwort</span><span class="sxs-lookup"><span data-stu-id="489b3-232">Response</span></span>
<span data-ttu-id="489b3-p123">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="489b3-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1423

{
  "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
  "id": "2daf8af2-8af2-2daf-f28a-af2df28aaf2d",
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
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine"
}
```





