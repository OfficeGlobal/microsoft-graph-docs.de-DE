---
title: IosScepCertificateProfile aktualisieren
description: Aktualisieren Sie die Eigenschaften eines IosScepCertificateProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1cb0158eff965e2076d7a081d23c7eda793722a5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914528"
---
# <a name="update-iosscepcertificateprofile"></a><span data-ttu-id="b4712-103">IosScepCertificateProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b4712-103">Update iosScepCertificateProfile</span></span>

> <span data-ttu-id="b4712-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b4712-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b4712-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b4712-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b4712-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b4712-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4712-107">Aktualisieren Sie die Eigenschaften eines [IosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b4712-107">Update the properties of a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b4712-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b4712-108">Prerequisites</span></span>
<span data-ttu-id="b4712-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4712-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4712-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b4712-111">Permission type</span></span>|<span data-ttu-id="b4712-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b4712-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4712-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b4712-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b4712-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4712-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b4712-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b4712-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4712-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4712-116">Not supported.</span></span>|
|<span data-ttu-id="b4712-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b4712-117">Application</span></span>|<span data-ttu-id="b4712-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4712-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4712-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4712-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b4712-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b4712-120">Request headers</span></span>
|<span data-ttu-id="b4712-121">Header</span><span class="sxs-lookup"><span data-stu-id="b4712-121">Header</span></span>|<span data-ttu-id="b4712-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b4712-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4712-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4712-123">Authorization</span></span>|<span data-ttu-id="b4712-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b4712-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4712-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b4712-125">Accept</span></span>|<span data-ttu-id="b4712-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b4712-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4712-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b4712-127">Request body</span></span>
<span data-ttu-id="b4712-128">Geben Sie im Textkörper Anforderung für das Objekt [IosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="b4712-128">In the request body, supply a JSON representation for the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="b4712-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [IosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="b4712-129">The following table shows the properties that are required when you create the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="b4712-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b4712-130">Property</span></span>|<span data-ttu-id="b4712-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b4712-131">Type</span></span>|<span data-ttu-id="b4712-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4712-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4712-133">id</span><span class="sxs-lookup"><span data-stu-id="b4712-133">id</span></span>|<span data-ttu-id="b4712-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4712-134">String</span></span>|<span data-ttu-id="b4712-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b4712-135">Key of the entity.</span></span> <span data-ttu-id="b4712-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4712-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4712-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4712-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b4712-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4712-138">DateTimeOffset</span></span>|<span data-ttu-id="b4712-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b4712-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b4712-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4712-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4712-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b4712-141">roleScopeTagIds</span></span>|<span data-ttu-id="b4712-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="b4712-142">String collection</span></span>|<span data-ttu-id="b4712-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="b4712-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b4712-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4712-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4712-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b4712-145">supportsScopeTags</span></span>|<span data-ttu-id="b4712-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b4712-146">Boolean</span></span>|<span data-ttu-id="b4712-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b4712-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b4712-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="b4712-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b4712-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="b4712-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b4712-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b4712-150">This property is read-only.</span></span> <span data-ttu-id="b4712-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4712-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4712-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b4712-152">createdDateTime</span></span>|<span data-ttu-id="b4712-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4712-153">DateTimeOffset</span></span>|<span data-ttu-id="b4712-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b4712-154">DateTime the object was created.</span></span> <span data-ttu-id="b4712-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4712-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4712-156">description</span><span class="sxs-lookup"><span data-stu-id="b4712-156">description</span></span>|<span data-ttu-id="b4712-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4712-157">String</span></span>|<span data-ttu-id="b4712-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b4712-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b4712-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4712-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4712-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b4712-160">displayName</span></span>|<span data-ttu-id="b4712-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4712-161">String</span></span>|<span data-ttu-id="b4712-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b4712-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b4712-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4712-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4712-164">Version</span><span class="sxs-lookup"><span data-stu-id="b4712-164">version</span></span>|<span data-ttu-id="b4712-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b4712-165">Int32</span></span>|<span data-ttu-id="b4712-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="b4712-166">Version of the device configuration.</span></span> <span data-ttu-id="b4712-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4712-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4712-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="b4712-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="b4712-169">Int32</span><span class="sxs-lookup"><span data-stu-id="b4712-169">Int32</span></span>|<span data-ttu-id="b4712-170">Zertifikat Erneuerung Schwellenwertprozentsatz.</span><span class="sxs-lookup"><span data-stu-id="b4712-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="b4712-171">Gültige Werte 1 bis 99 Inherited aus [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b4712-171">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b4712-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b4712-172">subjectNameFormat</span></span>|[<span data-ttu-id="b4712-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b4712-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="b4712-174">Format des Antragstellernamen Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="b4712-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="b4712-175">Geerbt von [IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b4712-175">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="b4712-176">Mögliche Werte sind: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI` und `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="b4712-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="b4712-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b4712-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="b4712-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b4712-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="b4712-179">Alternativer Antragstellername Zertifikattyp.</span><span class="sxs-lookup"><span data-stu-id="b4712-179">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="b4712-180">Geerbt von [IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b4712-180">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="b4712-181">Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="b4712-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="b4712-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="b4712-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="b4712-183">Int32</span><span class="sxs-lookup"><span data-stu-id="b4712-183">Int32</span></span>|<span data-ttu-id="b4712-184">Wert für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="b4712-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="b4712-185">Geerbt von [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b4712-185">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b4712-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b4712-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="b4712-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b4712-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="b4712-188">Skalierung für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="b4712-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="b4712-189">Geerbt von [IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b4712-189">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="b4712-190">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="b4712-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="b4712-191">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="b4712-191">scepServerUrls</span></span>|<span data-ttu-id="b4712-192">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="b4712-192">String collection</span></span>|<span data-ttu-id="b4712-193">SCEP Server URL(s) hinzu.</span><span class="sxs-lookup"><span data-stu-id="b4712-193">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="b4712-194">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="b4712-194">subjectNameFormatString</span></span>|<span data-ttu-id="b4712-195">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4712-195">String</span></span>|<span data-ttu-id="b4712-196">Benutzerdefiniertes Format zur Verwendung mit SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="b4712-196">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="b4712-197">Beispiel: CN = {{EmailAddress}} E = {{EmailAddress}}, OU = Unternehmensbenutzer, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="b4712-197">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="b4712-198">Schlüsselverwendung</span><span class="sxs-lookup"><span data-stu-id="b4712-198">keyUsage</span></span>|[<span data-ttu-id="b4712-199">keyUsages</span><span class="sxs-lookup"><span data-stu-id="b4712-199">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="b4712-200">SCEP Enhanced Key Usage.</span><span class="sxs-lookup"><span data-stu-id="b4712-200">SCEP Key Usage.</span></span> <span data-ttu-id="b4712-201">Mögliche Werte sind: `keyEncipherment` und `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="b4712-201">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="b4712-202">keySize</span><span class="sxs-lookup"><span data-stu-id="b4712-202">keySize</span></span>|[<span data-ttu-id="b4712-203">keySize</span><span class="sxs-lookup"><span data-stu-id="b4712-203">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="b4712-204">Wichtige SCEP-Größe.</span><span class="sxs-lookup"><span data-stu-id="b4712-204">SCEP Key Size.</span></span> <span data-ttu-id="b4712-205">Mögliche Werte sind: `size1024` und `size2048`.</span><span class="sxs-lookup"><span data-stu-id="b4712-205">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="b4712-206">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="b4712-206">extendedKeyUsages</span></span>|<span data-ttu-id="b4712-207">[ExtendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b4712-207">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="b4712-208">Erweiterte Schlüsselverwendung (EKU)-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="b4712-208">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="b4712-209">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="b4712-209">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b4712-210">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="b4712-210">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="b4712-211">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4712-211">String</span></span>|<span data-ttu-id="b4712-212">Benutzerdefinierte Zeichenfolge, die die AAD-Attribut definiert.</span><span class="sxs-lookup"><span data-stu-id="b4712-212">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="b4712-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="b4712-213">certificateStore</span></span>|[<span data-ttu-id="b4712-214">certificateStore</span><span class="sxs-lookup"><span data-stu-id="b4712-214">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="b4712-215">Ziel-Zertifikatspeicher.</span><span class="sxs-lookup"><span data-stu-id="b4712-215">Target store certificate.</span></span> <span data-ttu-id="b4712-216">Mögliche Werte sind: `user` und `machine`.</span><span class="sxs-lookup"><span data-stu-id="b4712-216">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="b4712-217">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="b4712-217">customSubjectAlternativeNames</span></span>|<span data-ttu-id="b4712-218">[CustomSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b4712-218">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="b4712-219">Benutzerdefinierte Subject Name Alterantive Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="b4712-219">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="b4712-220">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="b4712-220">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="b4712-221">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4712-221">Response</span></span>
<span data-ttu-id="b4712-222">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [IosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b4712-222">If successful, this method returns a `200 OK` response code and an updated [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4712-223">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b4712-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="b4712-224">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4712-224">Request</span></span>
<span data-ttu-id="b4712-225">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b4712-225">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1159

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
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b4712-226">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4712-226">Response</span></span>
<span data-ttu-id="b4712-p122">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b4712-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1331

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
  "id": "0deb8dbf-8dbf-0deb-bf8d-eb0dbf8deb0d",
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
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ]
}
```





