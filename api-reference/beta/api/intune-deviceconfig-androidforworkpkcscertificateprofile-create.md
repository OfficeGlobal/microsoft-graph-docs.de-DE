---
title: Erstellen von androidForWorkPkcsCertificateProfile
description: Erstellen eines neuen AndroidForWorkPkcsCertificateProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2718dac1c4b624983f445afa351e8e80882cb0ff
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963850"
---
# <a name="create-androidforworkpkcscertificateprofile"></a><span data-ttu-id="50fe4-103">Erstellen von androidForWorkPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="50fe4-103">Create androidForWorkPkcsCertificateProfile</span></span>

> <span data-ttu-id="50fe4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="50fe4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="50fe4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="50fe4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="50fe4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="50fe4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="50fe4-107">Erstellen eines neuen [AndroidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="50fe4-107">Create a new [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="50fe4-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="50fe4-108">Prerequisites</span></span>
<span data-ttu-id="50fe4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50fe4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50fe4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="50fe4-111">Permission type</span></span>|<span data-ttu-id="50fe4-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="50fe4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50fe4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="50fe4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50fe4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50fe4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="50fe4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="50fe4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50fe4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50fe4-116">Not supported.</span></span>|
|<span data-ttu-id="50fe4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="50fe4-117">Application</span></span>|<span data-ttu-id="50fe4-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50fe4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50fe4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="50fe4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="50fe4-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="50fe4-120">Request headers</span></span>
|<span data-ttu-id="50fe4-121">Header</span><span class="sxs-lookup"><span data-stu-id="50fe4-121">Header</span></span>|<span data-ttu-id="50fe4-122">Wert</span><span class="sxs-lookup"><span data-stu-id="50fe4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50fe4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="50fe4-123">Authorization</span></span>|<span data-ttu-id="50fe4-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="50fe4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50fe4-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="50fe4-125">Accept</span></span>|<span data-ttu-id="50fe4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50fe4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50fe4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="50fe4-127">Request body</span></span>
<span data-ttu-id="50fe4-128">Geben Sie im Textkörper Anforderung für das Objekt AndroidForWorkPkcsCertificateProfile eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="50fe4-128">In the request body, supply a JSON representation for the androidForWorkPkcsCertificateProfile object.</span></span>

<span data-ttu-id="50fe4-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AndroidForWorkPkcsCertificateProfile erstellen.</span><span class="sxs-lookup"><span data-stu-id="50fe4-129">The following table shows the properties that are required when you create the androidForWorkPkcsCertificateProfile.</span></span>

|<span data-ttu-id="50fe4-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="50fe4-130">Property</span></span>|<span data-ttu-id="50fe4-131">Typ</span><span class="sxs-lookup"><span data-stu-id="50fe4-131">Type</span></span>|<span data-ttu-id="50fe4-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="50fe4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50fe4-133">id</span><span class="sxs-lookup"><span data-stu-id="50fe4-133">id</span></span>|<span data-ttu-id="50fe4-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="50fe4-134">String</span></span>|<span data-ttu-id="50fe4-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="50fe4-135">Key of the entity.</span></span> <span data-ttu-id="50fe4-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50fe4-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50fe4-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50fe4-137">lastModifiedDateTime</span></span>|<span data-ttu-id="50fe4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50fe4-138">DateTimeOffset</span></span>|<span data-ttu-id="50fe4-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="50fe4-139">DateTime the object was last modified.</span></span> <span data-ttu-id="50fe4-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50fe4-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50fe4-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="50fe4-141">roleScopeTagIds</span></span>|<span data-ttu-id="50fe4-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="50fe4-142">String collection</span></span>|<span data-ttu-id="50fe4-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="50fe4-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="50fe4-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50fe4-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50fe4-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="50fe4-145">supportsScopeTags</span></span>|<span data-ttu-id="50fe4-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="50fe4-146">Boolean</span></span>|<span data-ttu-id="50fe4-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="50fe4-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="50fe4-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="50fe4-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="50fe4-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="50fe4-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="50fe4-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="50fe4-150">This property is read-only.</span></span> <span data-ttu-id="50fe4-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50fe4-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50fe4-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="50fe4-152">createdDateTime</span></span>|<span data-ttu-id="50fe4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50fe4-153">DateTimeOffset</span></span>|<span data-ttu-id="50fe4-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="50fe4-154">DateTime the object was created.</span></span> <span data-ttu-id="50fe4-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50fe4-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50fe4-156">description</span><span class="sxs-lookup"><span data-stu-id="50fe4-156">description</span></span>|<span data-ttu-id="50fe4-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="50fe4-157">String</span></span>|<span data-ttu-id="50fe4-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="50fe4-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="50fe4-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50fe4-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50fe4-160">displayName</span><span class="sxs-lookup"><span data-stu-id="50fe4-160">displayName</span></span>|<span data-ttu-id="50fe4-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="50fe4-161">String</span></span>|<span data-ttu-id="50fe4-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="50fe4-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="50fe4-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50fe4-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50fe4-164">Version</span><span class="sxs-lookup"><span data-stu-id="50fe4-164">version</span></span>|<span data-ttu-id="50fe4-165">Int32</span><span class="sxs-lookup"><span data-stu-id="50fe4-165">Int32</span></span>|<span data-ttu-id="50fe4-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="50fe4-166">Version of the device configuration.</span></span> <span data-ttu-id="50fe4-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50fe4-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="50fe4-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="50fe4-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="50fe4-169">Int32</span><span class="sxs-lookup"><span data-stu-id="50fe4-169">Int32</span></span>|<span data-ttu-id="50fe4-170">Zertifikat Erneuerung Schwellenwertprozentsatz.</span><span class="sxs-lookup"><span data-stu-id="50fe4-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="50fe4-171">Gültige Werte 1 bis 99 Inherited aus [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="50fe4-171">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="50fe4-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="50fe4-172">subjectNameFormat</span></span>|[<span data-ttu-id="50fe4-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="50fe4-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="50fe4-174">Format des Antragstellernamen Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="50fe4-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="50fe4-175">Geerbt von [AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="50fe4-175">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="50fe4-176">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="50fe4-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="50fe4-177">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="50fe4-177">certificateValidityPeriodValue</span></span>|<span data-ttu-id="50fe4-178">Int32</span><span class="sxs-lookup"><span data-stu-id="50fe4-178">Int32</span></span>|<span data-ttu-id="50fe4-179">Wert für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="50fe4-179">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="50fe4-180">Geerbt von [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="50fe4-180">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="50fe4-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="50fe4-181">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="50fe4-182">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="50fe4-182">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="50fe4-183">Skalierung für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="50fe4-183">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="50fe4-184">Geerbt von [AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="50fe4-184">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="50fe4-185">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="50fe4-185">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="50fe4-186">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="50fe4-186">extendedKeyUsages</span></span>|<span data-ttu-id="50fe4-187">[ExtendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="50fe4-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="50fe4-188">Erweiterte Schlüsselverwendung (EKU)-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="50fe4-188">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="50fe4-189">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="50fe4-189">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="50fe4-190">Geerbt von [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="50fe4-190">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="50fe4-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="50fe4-191">certificationAuthority</span></span>|<span data-ttu-id="50fe4-192">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="50fe4-192">String</span></span>|<span data-ttu-id="50fe4-193">PKCS-Zertifizierungsstelle</span><span class="sxs-lookup"><span data-stu-id="50fe4-193">PKCS Certification Authority</span></span>|
|<span data-ttu-id="50fe4-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="50fe4-194">certificationAuthorityName</span></span>|<span data-ttu-id="50fe4-195">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="50fe4-195">String</span></span>|<span data-ttu-id="50fe4-196">Name der Zertifizierungsstelle PKCS</span><span class="sxs-lookup"><span data-stu-id="50fe4-196">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="50fe4-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="50fe4-197">certificateTemplateName</span></span>|<span data-ttu-id="50fe4-198">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="50fe4-198">String</span></span>|<span data-ttu-id="50fe4-199">Name der PKCS Zertifikatsvorlage</span><span class="sxs-lookup"><span data-stu-id="50fe4-199">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="50fe4-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="50fe4-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="50fe4-201">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="50fe4-201">String</span></span>|<span data-ttu-id="50fe4-202">Benutzerdefinierte Zeichenfolge, die die AAD-Attribut definiert.</span><span class="sxs-lookup"><span data-stu-id="50fe4-202">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="50fe4-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="50fe4-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="50fe4-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="50fe4-204">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="50fe4-205">Subject Alternative Name Zertifikattyp.</span><span class="sxs-lookup"><span data-stu-id="50fe4-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="50fe4-206">Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="50fe4-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="50fe4-207">Antwort</span><span class="sxs-lookup"><span data-stu-id="50fe4-207">Response</span></span>
<span data-ttu-id="50fe4-208">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AndroidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="50fe4-208">If successful, this method returns a `201 Created` response code and a [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50fe4-209">Beispiel</span><span class="sxs-lookup"><span data-stu-id="50fe4-209">Example</span></span>
### <a name="request"></a><span data-ttu-id="50fe4-210">Anforderung</span><span class="sxs-lookup"><span data-stu-id="50fe4-210">Request</span></span>
<span data-ttu-id="50fe4-211">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="50fe4-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1029

{
  "@odata.type": "#microsoft.graph.androidForWorkPkcsCertificateProfile",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "subjectNameFormat": "commonNameIncludingEmail",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectAlternativeNameType": "emailAddress"
}
```

### <a name="response"></a><span data-ttu-id="50fe4-212">Antwort</span><span class="sxs-lookup"><span data-stu-id="50fe4-212">Response</span></span>
<span data-ttu-id="50fe4-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="50fe4-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1137

{
  "@odata.type": "#microsoft.graph.androidForWorkPkcsCertificateProfile",
  "id": "0a2d7691-7691-0a2d-9176-2d0a91762d0a",
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
  "subjectNameFormat": "commonNameIncludingEmail",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectAlternativeNameType": "emailAddress"
}
```





