---
title: WindowsPhone81SCEPCertificateProfile erstellen
description: Erstellen eines neuen windowsPhone81SCEPCertificateProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4755179f8b659588ca8068f89735ce3637d92ef0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144884"
---
# <a name="create-windowsphone81scepcertificateprofile"></a><span data-ttu-id="02b1d-103">WindowsPhone81SCEPCertificateProfile erstellen</span><span class="sxs-lookup"><span data-stu-id="02b1d-103">Create windowsPhone81SCEPCertificateProfile</span></span>

> <span data-ttu-id="02b1d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02b1d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02b1d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="02b1d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02b1d-106">Erstellen eines neuen [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="02b1d-106">Create a new [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02b1d-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="02b1d-107">Prerequisites</span></span>
<span data-ttu-id="02b1d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="02b1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="02b1d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="02b1d-110">Permission type</span></span>|<span data-ttu-id="02b1d-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="02b1d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02b1d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="02b1d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="02b1d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02b1d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="02b1d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="02b1d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02b1d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="02b1d-115">Not supported.</span></span>|
|<span data-ttu-id="02b1d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="02b1d-116">Application</span></span>|<span data-ttu-id="02b1d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="02b1d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02b1d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="02b1d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="02b1d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="02b1d-119">Request headers</span></span>
|<span data-ttu-id="02b1d-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="02b1d-120">Header</span></span>|<span data-ttu-id="02b1d-121">Wert</span><span class="sxs-lookup"><span data-stu-id="02b1d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02b1d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="02b1d-122">Authorization</span></span>|<span data-ttu-id="02b1d-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="02b1d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02b1d-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="02b1d-124">Accept</span></span>|<span data-ttu-id="02b1d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="02b1d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02b1d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="02b1d-126">Request body</span></span>
<span data-ttu-id="02b1d-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das windowsPhone81SCEPCertificateProfile-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="02b1d-127">In the request body, supply a JSON representation for the windowsPhone81SCEPCertificateProfile object.</span></span>

<span data-ttu-id="02b1d-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsPhone81SCEPCertificateProfile erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="02b1d-128">The following table shows the properties that are required when you create the windowsPhone81SCEPCertificateProfile.</span></span>

|<span data-ttu-id="02b1d-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="02b1d-129">Property</span></span>|<span data-ttu-id="02b1d-130">Typ</span><span class="sxs-lookup"><span data-stu-id="02b1d-130">Type</span></span>|<span data-ttu-id="02b1d-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="02b1d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02b1d-132">id</span><span class="sxs-lookup"><span data-stu-id="02b1d-132">id</span></span>|<span data-ttu-id="02b1d-133">string</span><span class="sxs-lookup"><span data-stu-id="02b1d-133">String</span></span>|<span data-ttu-id="02b1d-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="02b1d-134">Key of the entity.</span></span> <span data-ttu-id="02b1d-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="02b1d-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02b1d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="02b1d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="02b1d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02b1d-137">DateTimeOffset</span></span>|<span data-ttu-id="02b1d-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="02b1d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="02b1d-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="02b1d-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02b1d-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="02b1d-140">roleScopeTagIds</span></span>|<span data-ttu-id="02b1d-141">String collection</span><span class="sxs-lookup"><span data-stu-id="02b1d-141">String collection</span></span>|<span data-ttu-id="02b1d-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="02b1d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="02b1d-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="02b1d-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02b1d-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="02b1d-144">supportsScopeTags</span></span>|<span data-ttu-id="02b1d-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="02b1d-145">Boolean</span></span>|<span data-ttu-id="02b1d-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="02b1d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="02b1d-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="02b1d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="02b1d-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="02b1d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="02b1d-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="02b1d-149">This property is read-only.</span></span> <span data-ttu-id="02b1d-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="02b1d-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02b1d-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="02b1d-151">createdDateTime</span></span>|<span data-ttu-id="02b1d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02b1d-152">DateTimeOffset</span></span>|<span data-ttu-id="02b1d-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="02b1d-153">DateTime the object was created.</span></span> <span data-ttu-id="02b1d-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="02b1d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02b1d-155">description</span><span class="sxs-lookup"><span data-stu-id="02b1d-155">description</span></span>|<span data-ttu-id="02b1d-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="02b1d-156">String</span></span>|<span data-ttu-id="02b1d-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="02b1d-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="02b1d-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="02b1d-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02b1d-159">displayName</span><span class="sxs-lookup"><span data-stu-id="02b1d-159">displayName</span></span>|<span data-ttu-id="02b1d-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="02b1d-160">String</span></span>|<span data-ttu-id="02b1d-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="02b1d-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="02b1d-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="02b1d-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02b1d-163">Version</span><span class="sxs-lookup"><span data-stu-id="02b1d-163">version</span></span>|<span data-ttu-id="02b1d-164">Int32</span><span class="sxs-lookup"><span data-stu-id="02b1d-164">Int32</span></span>|<span data-ttu-id="02b1d-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="02b1d-165">Version of the device configuration.</span></span> <span data-ttu-id="02b1d-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="02b1d-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02b1d-167">Eigenschaften renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="02b1d-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="02b1d-168">Int32</span><span class="sxs-lookup"><span data-stu-id="02b1d-168">Int32</span></span>|<span data-ttu-id="02b1d-169">Schwellenwert für die Zertifikaterneuerung.</span><span class="sxs-lookup"><span data-stu-id="02b1d-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="02b1d-170">Geerbt von [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="02b1d-170">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="02b1d-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="02b1d-171">keyStorageProvider</span></span>|[<span data-ttu-id="02b1d-172">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="02b1d-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="02b1d-173">Schlüsselspeicheranbieter (KSP).</span><span class="sxs-lookup"><span data-stu-id="02b1d-173">Key Storage Provider (KSP).</span></span> <span data-ttu-id="02b1d-174">Von [WindowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="02b1d-174">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="02b1d-175">Mögliche Werte: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="02b1d-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="02b1d-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="02b1d-176">subjectNameFormat</span></span>|[<span data-ttu-id="02b1d-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="02b1d-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="02b1d-178">Format des Zertifikatsantrags Teller namens.</span><span class="sxs-lookup"><span data-stu-id="02b1d-178">Certificate Subject Name Format.</span></span> <span data-ttu-id="02b1d-179">Von [WindowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="02b1d-179">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="02b1d-180">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="02b1d-180">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="02b1d-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="02b1d-181">subjectAlternativeNameType</span></span>|[<span data-ttu-id="02b1d-182">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="02b1d-182">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="02b1d-183">Alternativer Namenstyp des Zertifikats betreffs.</span><span class="sxs-lookup"><span data-stu-id="02b1d-183">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="02b1d-184">Von [WindowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="02b1d-184">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="02b1d-185">Mögliche Werte: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="02b1d-185">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="02b1d-186">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="02b1d-186">certificateValidityPeriodValue</span></span>|<span data-ttu-id="02b1d-187">Int32</span><span class="sxs-lookup"><span data-stu-id="02b1d-187">Int32</span></span>|<span data-ttu-id="02b1d-188">Wert für den Validtiy-Zeitraum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="02b1d-188">Value for the Certificate Validtiy Period.</span></span> <span data-ttu-id="02b1d-189">Geerbt von [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="02b1d-189">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="02b1d-190">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="02b1d-190">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="02b1d-191">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="02b1d-191">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="02b1d-192">Skalierung für den Gültigkeitszeitraum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="02b1d-192">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="02b1d-193">Von [WindowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="02b1d-193">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="02b1d-194">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="02b1d-194">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="02b1d-195">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="02b1d-195">extendedKeyUsages</span></span>|<span data-ttu-id="02b1d-196">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="02b1d-196">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="02b1d-197">EKU-Einstellungen (Extended Key Usage).</span><span class="sxs-lookup"><span data-stu-id="02b1d-197">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="02b1d-198">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="02b1d-198">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="02b1d-199">Geerbt von [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="02b1d-199">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="02b1d-200">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="02b1d-200">scepServerUrls</span></span>|<span data-ttu-id="02b1d-201">String collection</span><span class="sxs-lookup"><span data-stu-id="02b1d-201">String collection</span></span>|<span data-ttu-id="02b1d-202">SCEP-Server-URL (s).</span><span class="sxs-lookup"><span data-stu-id="02b1d-202">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="02b1d-203">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="02b1d-203">subjectNameFormatString</span></span>|<span data-ttu-id="02b1d-204">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="02b1d-204">String</span></span>|<span data-ttu-id="02b1d-205">Benutzerdefiniertes Format, das mit SubjectNameFormat = Custom verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="02b1d-205">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="02b1d-206">Beispiel: CN = {{Email Adresse}}, E = {Email Adresse}}, OU = Enterprise users, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="02b1d-206">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="02b1d-207">keyUsage</span><span class="sxs-lookup"><span data-stu-id="02b1d-207">keyUsage</span></span>|[<span data-ttu-id="02b1d-208">keyUsages</span><span class="sxs-lookup"><span data-stu-id="02b1d-208">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="02b1d-209">SCEP-Schlüsselverwendung.</span><span class="sxs-lookup"><span data-stu-id="02b1d-209">SCEP Key Usage.</span></span> <span data-ttu-id="02b1d-210">Mögliche Werte sind: `keyEncipherment` und `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="02b1d-210">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="02b1d-211">keySize</span><span class="sxs-lookup"><span data-stu-id="02b1d-211">keySize</span></span>|[<span data-ttu-id="02b1d-212">keySize</span><span class="sxs-lookup"><span data-stu-id="02b1d-212">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="02b1d-213">SCEP-Schlüsselgröße.</span><span class="sxs-lookup"><span data-stu-id="02b1d-213">SCEP Key Size.</span></span> <span data-ttu-id="02b1d-214">Mögliche Werte sind: `size1024` und `size2048`.</span><span class="sxs-lookup"><span data-stu-id="02b1d-214">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="02b1d-215">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="02b1d-215">hashAlgorithm</span></span>|[<span data-ttu-id="02b1d-216">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="02b1d-216">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="02b1d-217">SCEP-Hash Algorithmus.</span><span class="sxs-lookup"><span data-stu-id="02b1d-217">SCEP Hash Algorithm.</span></span> <span data-ttu-id="02b1d-218">Mögliche Werte sind: `sha1` und `sha2`.</span><span class="sxs-lookup"><span data-stu-id="02b1d-218">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="02b1d-219">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="02b1d-219">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="02b1d-220">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="02b1d-220">String</span></span>|<span data-ttu-id="02b1d-221">Benutzerdefinierte Zeichenfolge, die das AAD-Attribut definiert.</span><span class="sxs-lookup"><span data-stu-id="02b1d-221">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="02b1d-222">Antwort</span><span class="sxs-lookup"><span data-stu-id="02b1d-222">Response</span></span>
<span data-ttu-id="02b1d-223">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="02b1d-223">If successful, this method returns a `201 Created` response code and a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02b1d-224">Beispiel</span><span class="sxs-lookup"><span data-stu-id="02b1d-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="02b1d-225">Anforderung</span><span class="sxs-lookup"><span data-stu-id="02b1d-225">Request</span></span>
<span data-ttu-id="02b1d-226">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="02b1d-226">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1032

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="02b1d-227">Antwort</span><span class="sxs-lookup"><span data-stu-id="02b1d-227">Response</span></span>
<span data-ttu-id="02b1d-p121">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="02b1d-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




