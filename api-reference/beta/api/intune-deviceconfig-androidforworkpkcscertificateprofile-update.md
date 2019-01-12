---
title: AndroidForWorkPkcsCertificateProfile aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidForWorkPkcsCertificateProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5056ec1e4cc3efe39334fa7e08b8744d6c5ecce2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948422"
---
# <a name="update-androidforworkpkcscertificateprofile"></a><span data-ttu-id="33786-103">AndroidForWorkPkcsCertificateProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="33786-103">Update androidForWorkPkcsCertificateProfile</span></span>

> <span data-ttu-id="33786-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="33786-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33786-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="33786-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="33786-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="33786-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="33786-107">Aktualisieren Sie die Eigenschaften eines [AndroidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="33786-107">Update the properties of a [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="33786-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="33786-108">Prerequisites</span></span>
<span data-ttu-id="33786-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33786-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33786-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="33786-111">Permission type</span></span>|<span data-ttu-id="33786-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="33786-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33786-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="33786-113">Delegated (work or school account)</span></span>|<span data-ttu-id="33786-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33786-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="33786-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="33786-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33786-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="33786-116">Not supported.</span></span>|
|<span data-ttu-id="33786-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="33786-117">Application</span></span>|<span data-ttu-id="33786-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="33786-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33786-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="33786-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="33786-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="33786-120">Request headers</span></span>
|<span data-ttu-id="33786-121">Header</span><span class="sxs-lookup"><span data-stu-id="33786-121">Header</span></span>|<span data-ttu-id="33786-122">Wert</span><span class="sxs-lookup"><span data-stu-id="33786-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33786-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="33786-123">Authorization</span></span>|<span data-ttu-id="33786-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="33786-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33786-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="33786-125">Accept</span></span>|<span data-ttu-id="33786-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33786-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33786-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="33786-127">Request body</span></span>
<span data-ttu-id="33786-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="33786-128">In the request body, supply a JSON representation for the [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="33786-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="33786-129">The following table shows the properties that are required when you create the [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md).</span></span>

|<span data-ttu-id="33786-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="33786-130">Property</span></span>|<span data-ttu-id="33786-131">Typ</span><span class="sxs-lookup"><span data-stu-id="33786-131">Type</span></span>|<span data-ttu-id="33786-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="33786-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33786-133">id</span><span class="sxs-lookup"><span data-stu-id="33786-133">id</span></span>|<span data-ttu-id="33786-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33786-134">String</span></span>|<span data-ttu-id="33786-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="33786-135">Key of the entity.</span></span> <span data-ttu-id="33786-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33786-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33786-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="33786-137">lastModifiedDateTime</span></span>|<span data-ttu-id="33786-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33786-138">DateTimeOffset</span></span>|<span data-ttu-id="33786-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="33786-139">DateTime the object was last modified.</span></span> <span data-ttu-id="33786-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33786-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33786-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="33786-141">roleScopeTagIds</span></span>|<span data-ttu-id="33786-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="33786-142">String collection</span></span>|<span data-ttu-id="33786-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="33786-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="33786-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33786-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33786-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="33786-145">supportsScopeTags</span></span>|<span data-ttu-id="33786-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="33786-146">Boolean</span></span>|<span data-ttu-id="33786-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="33786-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="33786-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="33786-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="33786-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="33786-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="33786-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="33786-150">This property is read-only.</span></span> <span data-ttu-id="33786-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33786-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33786-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="33786-152">createdDateTime</span></span>|<span data-ttu-id="33786-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33786-153">DateTimeOffset</span></span>|<span data-ttu-id="33786-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="33786-154">DateTime the object was created.</span></span> <span data-ttu-id="33786-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33786-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33786-156">description</span><span class="sxs-lookup"><span data-stu-id="33786-156">description</span></span>|<span data-ttu-id="33786-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33786-157">String</span></span>|<span data-ttu-id="33786-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="33786-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="33786-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33786-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33786-160">displayName</span><span class="sxs-lookup"><span data-stu-id="33786-160">displayName</span></span>|<span data-ttu-id="33786-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33786-161">String</span></span>|<span data-ttu-id="33786-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="33786-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="33786-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33786-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33786-164">Version</span><span class="sxs-lookup"><span data-stu-id="33786-164">version</span></span>|<span data-ttu-id="33786-165">Int32</span><span class="sxs-lookup"><span data-stu-id="33786-165">Int32</span></span>|<span data-ttu-id="33786-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="33786-166">Version of the device configuration.</span></span> <span data-ttu-id="33786-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33786-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33786-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="33786-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="33786-169">Int32</span><span class="sxs-lookup"><span data-stu-id="33786-169">Int32</span></span>|<span data-ttu-id="33786-170">Zertifikat Erneuerung Schwellenwertprozentsatz.</span><span class="sxs-lookup"><span data-stu-id="33786-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="33786-171">Gültige Werte 1 bis 99 Inherited aus [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="33786-171">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="33786-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="33786-172">subjectNameFormat</span></span>|[<span data-ttu-id="33786-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="33786-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="33786-174">Format des Antragstellernamen Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="33786-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="33786-175">Geerbt von [AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="33786-175">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="33786-176">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="33786-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="33786-177">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="33786-177">certificateValidityPeriodValue</span></span>|<span data-ttu-id="33786-178">Int32</span><span class="sxs-lookup"><span data-stu-id="33786-178">Int32</span></span>|<span data-ttu-id="33786-179">Wert für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="33786-179">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="33786-180">Geerbt von [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="33786-180">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="33786-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="33786-181">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="33786-182">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="33786-182">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="33786-183">Skalierung für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="33786-183">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="33786-184">Geerbt von [AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="33786-184">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="33786-185">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="33786-185">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="33786-186">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="33786-186">extendedKeyUsages</span></span>|<span data-ttu-id="33786-187">[ExtendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="33786-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="33786-188">Erweiterte Schlüsselverwendung (EKU)-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="33786-188">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="33786-189">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="33786-189">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="33786-190">Geerbt von [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="33786-190">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="33786-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="33786-191">certificationAuthority</span></span>|<span data-ttu-id="33786-192">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33786-192">String</span></span>|<span data-ttu-id="33786-193">PKCS-Zertifizierungsstelle</span><span class="sxs-lookup"><span data-stu-id="33786-193">PKCS Certification Authority</span></span>|
|<span data-ttu-id="33786-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="33786-194">certificationAuthorityName</span></span>|<span data-ttu-id="33786-195">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33786-195">String</span></span>|<span data-ttu-id="33786-196">Name der Zertifizierungsstelle PKCS</span><span class="sxs-lookup"><span data-stu-id="33786-196">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="33786-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="33786-197">certificateTemplateName</span></span>|<span data-ttu-id="33786-198">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33786-198">String</span></span>|<span data-ttu-id="33786-199">Name der PKCS Zertifikatsvorlage</span><span class="sxs-lookup"><span data-stu-id="33786-199">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="33786-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="33786-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="33786-201">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33786-201">String</span></span>|<span data-ttu-id="33786-202">Benutzerdefinierte Zeichenfolge, die die AAD-Attribut definiert.</span><span class="sxs-lookup"><span data-stu-id="33786-202">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="33786-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="33786-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="33786-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="33786-204">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="33786-205">Subject Alternative Name Zertifikattyp.</span><span class="sxs-lookup"><span data-stu-id="33786-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="33786-206">Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="33786-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="33786-207">Antwort</span><span class="sxs-lookup"><span data-stu-id="33786-207">Response</span></span>
<span data-ttu-id="33786-208">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="33786-208">If successful, this method returns a `200 OK` response code and an updated [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33786-209">Beispiel</span><span class="sxs-lookup"><span data-stu-id="33786-209">Example</span></span>
### <a name="request"></a><span data-ttu-id="33786-210">Anforderung</span><span class="sxs-lookup"><span data-stu-id="33786-210">Request</span></span>
<span data-ttu-id="33786-211">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="33786-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 954

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

### <a name="response"></a><span data-ttu-id="33786-212">Antwort</span><span class="sxs-lookup"><span data-stu-id="33786-212">Response</span></span>
<span data-ttu-id="33786-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="33786-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





