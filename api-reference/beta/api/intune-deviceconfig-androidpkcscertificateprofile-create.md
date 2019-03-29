---
title: Androidpkcscertificateprofile hinzugefügt erstellen
description: Erstellen eines neuen Androidpkcscertificateprofile hinzugefügt-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de7020d0415628e7283ff98c273dbaa481e2ea8d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973523"
---
# <a name="create-androidpkcscertificateprofile"></a><span data-ttu-id="9c413-103">Androidpkcscertificateprofile hinzugefügt erstellen</span><span class="sxs-lookup"><span data-stu-id="9c413-103">Create androidPkcsCertificateProfile</span></span>

> <span data-ttu-id="9c413-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9c413-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c413-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9c413-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c413-106">Erstellen eines neuen [androidpkcscertificateprofile hinzugefügt](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="9c413-106">Create a new [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c413-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9c413-107">Prerequisites</span></span>
<span data-ttu-id="9c413-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c413-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c413-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9c413-110">Permission type</span></span>|<span data-ttu-id="9c413-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9c413-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c413-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9c413-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9c413-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c413-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9c413-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9c413-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c413-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9c413-115">Not supported.</span></span>|
|<span data-ttu-id="9c413-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9c413-116">Application</span></span>|<span data-ttu-id="9c413-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9c413-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c413-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9c413-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9c413-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9c413-119">Request headers</span></span>
|<span data-ttu-id="9c413-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9c413-120">Header</span></span>|<span data-ttu-id="9c413-121">Wert</span><span class="sxs-lookup"><span data-stu-id="9c413-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c413-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c413-122">Authorization</span></span>|<span data-ttu-id="9c413-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9c413-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c413-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9c413-124">Accept</span></span>|<span data-ttu-id="9c413-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9c413-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c413-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9c413-126">Request body</span></span>
<span data-ttu-id="9c413-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das Androidpkcscertificateprofile hinzugefügt-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="9c413-127">In the request body, supply a JSON representation for the androidPkcsCertificateProfile object.</span></span>

<span data-ttu-id="9c413-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der Androidpkcscertificateprofile hinzugefügt erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="9c413-128">The following table shows the properties that are required when you create the androidPkcsCertificateProfile.</span></span>

|<span data-ttu-id="9c413-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9c413-129">Property</span></span>|<span data-ttu-id="9c413-130">Typ</span><span class="sxs-lookup"><span data-stu-id="9c413-130">Type</span></span>|<span data-ttu-id="9c413-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9c413-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c413-132">id</span><span class="sxs-lookup"><span data-stu-id="9c413-132">id</span></span>|<span data-ttu-id="9c413-133">String</span><span class="sxs-lookup"><span data-stu-id="9c413-133">String</span></span>|<span data-ttu-id="9c413-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9c413-134">Key of the entity.</span></span> <span data-ttu-id="9c413-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9c413-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c413-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9c413-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9c413-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c413-137">DateTimeOffset</span></span>|<span data-ttu-id="9c413-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="9c413-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9c413-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9c413-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c413-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="9c413-140">roleScopeTagIds</span></span>|<span data-ttu-id="9c413-141">String collection</span><span class="sxs-lookup"><span data-stu-id="9c413-141">String collection</span></span>|<span data-ttu-id="9c413-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="9c413-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9c413-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9c413-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c413-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9c413-144">supportsScopeTags</span></span>|<span data-ttu-id="9c413-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9c413-145">Boolean</span></span>|<span data-ttu-id="9c413-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9c413-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9c413-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="9c413-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9c413-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="9c413-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9c413-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9c413-149">This property is read-only.</span></span> <span data-ttu-id="9c413-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9c413-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c413-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9c413-151">createdDateTime</span></span>|<span data-ttu-id="9c413-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c413-152">DateTimeOffset</span></span>|<span data-ttu-id="9c413-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="9c413-153">DateTime the object was created.</span></span> <span data-ttu-id="9c413-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9c413-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c413-155">description</span><span class="sxs-lookup"><span data-stu-id="9c413-155">description</span></span>|<span data-ttu-id="9c413-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9c413-156">String</span></span>|<span data-ttu-id="9c413-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="9c413-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9c413-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9c413-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c413-159">displayName</span><span class="sxs-lookup"><span data-stu-id="9c413-159">displayName</span></span>|<span data-ttu-id="9c413-160">String</span><span class="sxs-lookup"><span data-stu-id="9c413-160">String</span></span>|<span data-ttu-id="9c413-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="9c413-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9c413-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9c413-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c413-163">Version</span><span class="sxs-lookup"><span data-stu-id="9c413-163">version</span></span>|<span data-ttu-id="9c413-164">Int32</span><span class="sxs-lookup"><span data-stu-id="9c413-164">Int32</span></span>|<span data-ttu-id="9c413-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="9c413-165">Version of the device configuration.</span></span> <span data-ttu-id="9c413-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9c413-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c413-167">Eigenschaften renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="9c413-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="9c413-168">Int32</span><span class="sxs-lookup"><span data-stu-id="9c413-168">Int32</span></span>|<span data-ttu-id="9c413-169">Schwellenwert für die Zertifikaterneuerung.</span><span class="sxs-lookup"><span data-stu-id="9c413-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="9c413-170">Gültige Werte 1 bis 99 geerbt von [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9c413-170">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="9c413-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="9c413-171">subjectNameFormat</span></span>|[<span data-ttu-id="9c413-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="9c413-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="9c413-173">Format des Zertifikatsantrags Teller namens.</span><span class="sxs-lookup"><span data-stu-id="9c413-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="9c413-174">Von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="9c413-174">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="9c413-175">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="9c413-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="9c413-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="9c413-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="9c413-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="9c413-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="9c413-178">Alternativer Namenstyp des Zertifikats betreffs.</span><span class="sxs-lookup"><span data-stu-id="9c413-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="9c413-179">Von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="9c413-179">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="9c413-180">Mögliche Werte: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="9c413-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="9c413-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="9c413-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="9c413-182">Int32</span><span class="sxs-lookup"><span data-stu-id="9c413-182">Int32</span></span>|<span data-ttu-id="9c413-183">Wert für den Gültigkeitszeitraum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="9c413-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="9c413-184">Geerbt von [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9c413-184">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="9c413-185">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="9c413-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="9c413-186">Certificatevalidityperiodscale wurden</span><span class="sxs-lookup"><span data-stu-id="9c413-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="9c413-187">Skalierung für den Gültigkeitszeitraum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="9c413-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="9c413-188">Von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="9c413-188">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="9c413-189">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="9c413-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="9c413-190">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="9c413-190">extendedKeyUsages</span></span>|<span data-ttu-id="9c413-191">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="9c413-191">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="9c413-192">EKU-Einstellungen (Extended Key Usage).</span><span class="sxs-lookup"><span data-stu-id="9c413-192">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="9c413-193">Diese Sammlung darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="9c413-193">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="9c413-194">Geerbt von [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9c413-194">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="9c413-195">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="9c413-195">certificationAuthority</span></span>|<span data-ttu-id="9c413-196">String</span><span class="sxs-lookup"><span data-stu-id="9c413-196">String</span></span>|<span data-ttu-id="9c413-197">PKCS-ZertifizierungsStelle</span><span class="sxs-lookup"><span data-stu-id="9c413-197">PKCS Certification Authority</span></span>|
|<span data-ttu-id="9c413-198">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="9c413-198">certificationAuthorityName</span></span>|<span data-ttu-id="9c413-199">String</span><span class="sxs-lookup"><span data-stu-id="9c413-199">String</span></span>|<span data-ttu-id="9c413-200">Name der PKCS-ZertifizierungsStelle</span><span class="sxs-lookup"><span data-stu-id="9c413-200">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="9c413-201">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="9c413-201">certificateTemplateName</span></span>|<span data-ttu-id="9c413-202">String</span><span class="sxs-lookup"><span data-stu-id="9c413-202">String</span></span>|<span data-ttu-id="9c413-203">Name der PKCS-Zertifikatvorlage</span><span class="sxs-lookup"><span data-stu-id="9c413-203">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="9c413-204">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="9c413-204">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="9c413-205">String</span><span class="sxs-lookup"><span data-stu-id="9c413-205">String</span></span>|<span data-ttu-id="9c413-206">Benutzerdefinierte Zeichenfolge, die das AAD-Attribut definiert.</span><span class="sxs-lookup"><span data-stu-id="9c413-206">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="9c413-207">Antwort</span><span class="sxs-lookup"><span data-stu-id="9c413-207">Response</span></span>
<span data-ttu-id="9c413-208">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [androidpkcscertificateprofile hinzugefügt](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9c413-208">If successful, this method returns a `201 Created` response code and a [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c413-209">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9c413-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c413-210">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9c413-210">Request</span></span>
<span data-ttu-id="9c413-211">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9c413-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 958

{
  "@odata.type": "#microsoft.graph.androidPkcsCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="9c413-212">Antwort</span><span class="sxs-lookup"><span data-stu-id="9c413-212">Response</span></span>
<span data-ttu-id="9c413-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9c413-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1130

{
  "@odata.type": "#microsoft.graph.androidPkcsCertificateProfile",
  "id": "bb55705b-705b-bb55-5b70-55bb5b7055bb",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```




