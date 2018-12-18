---
title: Erstellen von androidScepCertificateProfile
description: Erstellen eines neuen AndroidScepCertificateProfile-Objekts.
author: tfitzmac
ms.openlocfilehash: 7e00bd8e4b65c1785ea9ab27ec723f773ec220fb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349721"
---
# <a name="create-androidscepcertificateprofile"></a><span data-ttu-id="a72a2-103">Erstellen von androidScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="a72a2-103">Create androidScepCertificateProfile</span></span>

> <span data-ttu-id="a72a2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a72a2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a72a2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a72a2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a72a2-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a72a2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a72a2-107">Erstellen eines neuen [AndroidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="a72a2-107">Create a new [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a72a2-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a72a2-108">Prerequisites</span></span>
<span data-ttu-id="a72a2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a72a2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a72a2-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a72a2-111">Permission type</span></span>|<span data-ttu-id="a72a2-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a72a2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a72a2-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a72a2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a72a2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a72a2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a72a2-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a72a2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a72a2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a72a2-116">Not supported.</span></span>|
|<span data-ttu-id="a72a2-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a72a2-117">Application</span></span>|<span data-ttu-id="a72a2-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a72a2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a72a2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a72a2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a72a2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a72a2-120">Request headers</span></span>
|<span data-ttu-id="a72a2-121">Header</span><span class="sxs-lookup"><span data-stu-id="a72a2-121">Header</span></span>|<span data-ttu-id="a72a2-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a72a2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a72a2-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a72a2-123">Authorization</span></span>|<span data-ttu-id="a72a2-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a72a2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a72a2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a72a2-125">Accept</span></span>|<span data-ttu-id="a72a2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a72a2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a72a2-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a72a2-127">Request body</span></span>
<span data-ttu-id="a72a2-128">Geben Sie im Textkörper Anforderung für das Objekt AndroidScepCertificateProfile eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="a72a2-128">In the request body, supply a JSON representation for the androidScepCertificateProfile object.</span></span>

<span data-ttu-id="a72a2-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AndroidScepCertificateProfile erstellen.</span><span class="sxs-lookup"><span data-stu-id="a72a2-129">The following table shows the properties that are required when you create the androidScepCertificateProfile.</span></span>

|<span data-ttu-id="a72a2-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a72a2-130">Property</span></span>|<span data-ttu-id="a72a2-131">Typ</span><span class="sxs-lookup"><span data-stu-id="a72a2-131">Type</span></span>|<span data-ttu-id="a72a2-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a72a2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a72a2-133">id</span><span class="sxs-lookup"><span data-stu-id="a72a2-133">id</span></span>|<span data-ttu-id="a72a2-134">String</span><span class="sxs-lookup"><span data-stu-id="a72a2-134">String</span></span>|<span data-ttu-id="a72a2-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a72a2-135">Key of the entity.</span></span> <span data-ttu-id="a72a2-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a72a2-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a72a2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a72a2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a72a2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a72a2-138">DateTimeOffset</span></span>|<span data-ttu-id="a72a2-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a72a2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a72a2-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a72a2-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a72a2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a72a2-141">roleScopeTagIds</span></span>|<span data-ttu-id="a72a2-142">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="a72a2-142">String collection</span></span>|<span data-ttu-id="a72a2-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="a72a2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a72a2-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a72a2-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a72a2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a72a2-145">supportsScopeTags</span></span>|<span data-ttu-id="a72a2-146">Boolesch</span><span class="sxs-lookup"><span data-stu-id="a72a2-146">Boolean</span></span>|<span data-ttu-id="a72a2-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a72a2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a72a2-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="a72a2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a72a2-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="a72a2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a72a2-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a72a2-150">This property is read-only.</span></span> <span data-ttu-id="a72a2-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a72a2-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a72a2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a72a2-152">createdDateTime</span></span>|<span data-ttu-id="a72a2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a72a2-153">DateTimeOffset</span></span>|<span data-ttu-id="a72a2-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a72a2-154">DateTime the object was created.</span></span> <span data-ttu-id="a72a2-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a72a2-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a72a2-156">description</span><span class="sxs-lookup"><span data-stu-id="a72a2-156">description</span></span>|<span data-ttu-id="a72a2-157">String</span><span class="sxs-lookup"><span data-stu-id="a72a2-157">String</span></span>|<span data-ttu-id="a72a2-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a72a2-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a72a2-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a72a2-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a72a2-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a72a2-160">displayName</span></span>|<span data-ttu-id="a72a2-161">String</span><span class="sxs-lookup"><span data-stu-id="a72a2-161">String</span></span>|<span data-ttu-id="a72a2-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a72a2-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a72a2-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a72a2-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a72a2-164">Version</span><span class="sxs-lookup"><span data-stu-id="a72a2-164">version</span></span>|<span data-ttu-id="a72a2-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a72a2-165">Int32</span></span>|<span data-ttu-id="a72a2-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="a72a2-166">Version of the device configuration.</span></span> <span data-ttu-id="a72a2-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a72a2-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a72a2-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="a72a2-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="a72a2-169">Int32</span><span class="sxs-lookup"><span data-stu-id="a72a2-169">Int32</span></span>|<span data-ttu-id="a72a2-170">Zertifikat Erneuerung Schwellenwertprozentsatz.</span><span class="sxs-lookup"><span data-stu-id="a72a2-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="a72a2-171">Gültige Werte 1 bis 99 Inherited aus [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a72a2-171">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a72a2-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a72a2-172">subjectNameFormat</span></span>|[<span data-ttu-id="a72a2-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a72a2-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="a72a2-174">Format des Antragstellernamen Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="a72a2-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="a72a2-175">Geerbt von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a72a2-175">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="a72a2-176">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="a72a2-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="a72a2-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a72a2-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="a72a2-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a72a2-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="a72a2-179">Subject Alternative Name Zertifikattyp.</span><span class="sxs-lookup"><span data-stu-id="a72a2-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="a72a2-180">Geerbt von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a72a2-180">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="a72a2-181">Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="a72a2-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="a72a2-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="a72a2-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="a72a2-183">Int32</span><span class="sxs-lookup"><span data-stu-id="a72a2-183">Int32</span></span>|<span data-ttu-id="a72a2-184">Wert für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="a72a2-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="a72a2-185">Geerbt von [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a72a2-185">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a72a2-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a72a2-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="a72a2-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a72a2-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="a72a2-188">Skalierung für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="a72a2-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="a72a2-189">Geerbt von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a72a2-189">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="a72a2-190">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="a72a2-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="a72a2-191">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="a72a2-191">extendedKeyUsages</span></span>|<span data-ttu-id="a72a2-192">[ExtendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="a72a2-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="a72a2-193">Erweiterte Schlüsselverwendung (EKU)-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="a72a2-193">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="a72a2-194">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="a72a2-194">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="a72a2-195">Geerbt von [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a72a2-195">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a72a2-196">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="a72a2-196">scepServerUrls</span></span>|<span data-ttu-id="a72a2-197">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="a72a2-197">String collection</span></span>|<span data-ttu-id="a72a2-198">SCEP Server URL(s) hinzu</span><span class="sxs-lookup"><span data-stu-id="a72a2-198">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="a72a2-199">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="a72a2-199">subjectNameFormatString</span></span>|<span data-ttu-id="a72a2-200">String</span><span class="sxs-lookup"><span data-stu-id="a72a2-200">String</span></span>|<span data-ttu-id="a72a2-201">Benutzerdefiniertes Format zur Verwendung mit SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="a72a2-201">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="a72a2-202">Beispiel: CN = {{EmailAddress}} E = {{EmailAddress}}, OU = Unternehmensbenutzer, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="a72a2-202">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="a72a2-203">Schlüsselverwendung</span><span class="sxs-lookup"><span data-stu-id="a72a2-203">keyUsage</span></span>|[<span data-ttu-id="a72a2-204">keyUsages</span><span class="sxs-lookup"><span data-stu-id="a72a2-204">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="a72a2-205">SCEP Enhanced Key Usage.</span><span class="sxs-lookup"><span data-stu-id="a72a2-205">SCEP Key Usage.</span></span> <span data-ttu-id="a72a2-206">Mögliche Werte sind: `keyEncipherment` und `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="a72a2-206">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="a72a2-207">keySize</span><span class="sxs-lookup"><span data-stu-id="a72a2-207">keySize</span></span>|[<span data-ttu-id="a72a2-208">keySize</span><span class="sxs-lookup"><span data-stu-id="a72a2-208">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="a72a2-209">Wichtige SCEP-Größe.</span><span class="sxs-lookup"><span data-stu-id="a72a2-209">SCEP Key Size.</span></span> <span data-ttu-id="a72a2-210">Mögliche Werte sind: `size1024` und `size2048`.</span><span class="sxs-lookup"><span data-stu-id="a72a2-210">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="a72a2-211">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="a72a2-211">hashAlgorithm</span></span>|[<span data-ttu-id="a72a2-212">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="a72a2-212">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="a72a2-213">SCEP Hashalgorithmus.</span><span class="sxs-lookup"><span data-stu-id="a72a2-213">SCEP Hash Algorithm.</span></span> <span data-ttu-id="a72a2-214">Mögliche Werte sind: `sha1` und `sha2`.</span><span class="sxs-lookup"><span data-stu-id="a72a2-214">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="a72a2-215">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="a72a2-215">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="a72a2-216">String</span><span class="sxs-lookup"><span data-stu-id="a72a2-216">String</span></span>|<span data-ttu-id="a72a2-217">Benutzerdefinierte Zeichenfolge, die die AAD-Attribut definiert.</span><span class="sxs-lookup"><span data-stu-id="a72a2-217">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="a72a2-218">Antwort</span><span class="sxs-lookup"><span data-stu-id="a72a2-218">Response</span></span>
<span data-ttu-id="a72a2-219">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AndroidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="a72a2-219">If successful, this method returns a `201 Created` response code and a [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a72a2-220">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a72a2-220">Example</span></span>
### <a name="request"></a><span data-ttu-id="a72a2-221">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a72a2-221">Request</span></span>
<span data-ttu-id="a72a2-222">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a72a2-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1038

{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="a72a2-223">Antwort</span><span class="sxs-lookup"><span data-stu-id="a72a2-223">Response</span></span>
<span data-ttu-id="a72a2-p121">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a72a2-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1146

{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
  "id": "e9a0dbbd-dbbd-e9a0-bddb-a0e9bddba0e9",
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





