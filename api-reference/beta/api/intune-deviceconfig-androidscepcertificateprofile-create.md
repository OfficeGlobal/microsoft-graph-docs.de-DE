---
title: Erstellen von androidScepCertificateProfile
description: Erstellen eines neuen AndroidScepCertificateProfile-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e1e208882f0524acd26e390b82a7624995603b42
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425085"
---
# <a name="create-androidscepcertificateprofile"></a><span data-ttu-id="a4b19-103">Erstellen von androidScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="a4b19-103">Create androidScepCertificateProfile</span></span>

> <span data-ttu-id="a4b19-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="a4b19-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a4b19-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a4b19-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a4b19-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a4b19-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4b19-107">Erstellen eines neuen [AndroidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="a4b19-107">Create a new [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4b19-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a4b19-108">Prerequisites</span></span>
<span data-ttu-id="a4b19-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a4b19-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a4b19-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a4b19-111">Permission type</span></span>|<span data-ttu-id="a4b19-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a4b19-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4b19-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a4b19-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a4b19-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4b19-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a4b19-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a4b19-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4b19-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a4b19-116">Not supported.</span></span>|
|<span data-ttu-id="a4b19-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a4b19-117">Application</span></span>|<span data-ttu-id="a4b19-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a4b19-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4b19-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a4b19-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a4b19-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a4b19-120">Request headers</span></span>
|<span data-ttu-id="a4b19-121">Header</span><span class="sxs-lookup"><span data-stu-id="a4b19-121">Header</span></span>|<span data-ttu-id="a4b19-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a4b19-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4b19-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a4b19-123">Authorization</span></span>|<span data-ttu-id="a4b19-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a4b19-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4b19-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a4b19-125">Accept</span></span>|<span data-ttu-id="a4b19-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a4b19-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4b19-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a4b19-127">Request body</span></span>
<span data-ttu-id="a4b19-128">Geben Sie im Textkörper Anforderung für das Objekt AndroidScepCertificateProfile eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="a4b19-128">In the request body, supply a JSON representation for the androidScepCertificateProfile object.</span></span>

<span data-ttu-id="a4b19-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AndroidScepCertificateProfile erstellen.</span><span class="sxs-lookup"><span data-stu-id="a4b19-129">The following table shows the properties that are required when you create the androidScepCertificateProfile.</span></span>

|<span data-ttu-id="a4b19-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a4b19-130">Property</span></span>|<span data-ttu-id="a4b19-131">Typ</span><span class="sxs-lookup"><span data-stu-id="a4b19-131">Type</span></span>|<span data-ttu-id="a4b19-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a4b19-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4b19-133">id</span><span class="sxs-lookup"><span data-stu-id="a4b19-133">id</span></span>|<span data-ttu-id="a4b19-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a4b19-134">String</span></span>|<span data-ttu-id="a4b19-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a4b19-135">Key of the entity.</span></span> <span data-ttu-id="a4b19-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4b19-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4b19-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a4b19-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a4b19-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4b19-138">DateTimeOffset</span></span>|<span data-ttu-id="a4b19-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a4b19-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a4b19-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4b19-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4b19-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a4b19-141">roleScopeTagIds</span></span>|<span data-ttu-id="a4b19-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="a4b19-142">String collection</span></span>|<span data-ttu-id="a4b19-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="a4b19-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a4b19-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4b19-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4b19-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a4b19-145">supportsScopeTags</span></span>|<span data-ttu-id="a4b19-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4b19-146">Boolean</span></span>|<span data-ttu-id="a4b19-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a4b19-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a4b19-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="a4b19-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a4b19-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="a4b19-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a4b19-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a4b19-150">This property is read-only.</span></span> <span data-ttu-id="a4b19-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4b19-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4b19-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a4b19-152">createdDateTime</span></span>|<span data-ttu-id="a4b19-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4b19-153">DateTimeOffset</span></span>|<span data-ttu-id="a4b19-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a4b19-154">DateTime the object was created.</span></span> <span data-ttu-id="a4b19-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4b19-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4b19-156">description</span><span class="sxs-lookup"><span data-stu-id="a4b19-156">description</span></span>|<span data-ttu-id="a4b19-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a4b19-157">String</span></span>|<span data-ttu-id="a4b19-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a4b19-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a4b19-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4b19-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4b19-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a4b19-160">displayName</span></span>|<span data-ttu-id="a4b19-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a4b19-161">String</span></span>|<span data-ttu-id="a4b19-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a4b19-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a4b19-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4b19-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4b19-164">Version</span><span class="sxs-lookup"><span data-stu-id="a4b19-164">version</span></span>|<span data-ttu-id="a4b19-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a4b19-165">Int32</span></span>|<span data-ttu-id="a4b19-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="a4b19-166">Version of the device configuration.</span></span> <span data-ttu-id="a4b19-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4b19-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4b19-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="a4b19-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="a4b19-169">Int32</span><span class="sxs-lookup"><span data-stu-id="a4b19-169">Int32</span></span>|<span data-ttu-id="a4b19-170">Zertifikat Erneuerung Schwellenwertprozentsatz.</span><span class="sxs-lookup"><span data-stu-id="a4b19-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="a4b19-171">Gültige Werte 1 bis 99 Inherited aus [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a4b19-171">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a4b19-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a4b19-172">subjectNameFormat</span></span>|[<span data-ttu-id="a4b19-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a4b19-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="a4b19-174">Format des Antragstellernamen Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="a4b19-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="a4b19-175">Geerbt von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a4b19-175">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="a4b19-176">Mögliche Werte: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="a4b19-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="a4b19-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a4b19-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="a4b19-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a4b19-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="a4b19-179">Subject Alternative Name Zertifikattyp.</span><span class="sxs-lookup"><span data-stu-id="a4b19-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="a4b19-180">Geerbt von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a4b19-180">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="a4b19-181">Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="a4b19-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="a4b19-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="a4b19-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="a4b19-183">Int32</span><span class="sxs-lookup"><span data-stu-id="a4b19-183">Int32</span></span>|<span data-ttu-id="a4b19-184">Wert für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="a4b19-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="a4b19-185">Geerbt von [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a4b19-185">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a4b19-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a4b19-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="a4b19-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a4b19-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="a4b19-188">Skalierung für die Gültigkeitsdauer des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="a4b19-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="a4b19-189">Geerbt von [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a4b19-189">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="a4b19-190">Mögliche Werte sind: `days`, `months` und `years`.</span><span class="sxs-lookup"><span data-stu-id="a4b19-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="a4b19-191">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="a4b19-191">extendedKeyUsages</span></span>|<span data-ttu-id="a4b19-192">[ExtendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="a4b19-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="a4b19-193">Erweiterte Schlüsselverwendung (EKU)-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="a4b19-193">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="a4b19-194">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="a4b19-194">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="a4b19-195">Geerbt von [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a4b19-195">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a4b19-196">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="a4b19-196">scepServerUrls</span></span>|<span data-ttu-id="a4b19-197">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="a4b19-197">String collection</span></span>|<span data-ttu-id="a4b19-198">SCEP Server URL(s) hinzu</span><span class="sxs-lookup"><span data-stu-id="a4b19-198">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="a4b19-199">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="a4b19-199">subjectNameFormatString</span></span>|<span data-ttu-id="a4b19-200">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a4b19-200">String</span></span>|<span data-ttu-id="a4b19-201">Benutzerdefiniertes Format zur Verwendung mit SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="a4b19-201">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="a4b19-202">Beispiel: CN = {{EmailAddress}} E = {{EmailAddress}}, OU = Unternehmensbenutzer, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="a4b19-202">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="a4b19-203">Schlüsselverwendung</span><span class="sxs-lookup"><span data-stu-id="a4b19-203">keyUsage</span></span>|[<span data-ttu-id="a4b19-204">keyUsages</span><span class="sxs-lookup"><span data-stu-id="a4b19-204">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="a4b19-205">SCEP Enhanced Key Usage.</span><span class="sxs-lookup"><span data-stu-id="a4b19-205">SCEP Key Usage.</span></span> <span data-ttu-id="a4b19-206">Mögliche Werte sind: `keyEncipherment` und `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="a4b19-206">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="a4b19-207">keySize</span><span class="sxs-lookup"><span data-stu-id="a4b19-207">keySize</span></span>|[<span data-ttu-id="a4b19-208">keySize</span><span class="sxs-lookup"><span data-stu-id="a4b19-208">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="a4b19-209">Wichtige SCEP-Größe.</span><span class="sxs-lookup"><span data-stu-id="a4b19-209">SCEP Key Size.</span></span> <span data-ttu-id="a4b19-210">Mögliche Werte sind: `size1024` und `size2048`.</span><span class="sxs-lookup"><span data-stu-id="a4b19-210">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="a4b19-211">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="a4b19-211">hashAlgorithm</span></span>|[<span data-ttu-id="a4b19-212">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="a4b19-212">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="a4b19-213">SCEP Hashalgorithmus.</span><span class="sxs-lookup"><span data-stu-id="a4b19-213">SCEP Hash Algorithm.</span></span> <span data-ttu-id="a4b19-214">Mögliche Werte sind: `sha1` und `sha2`.</span><span class="sxs-lookup"><span data-stu-id="a4b19-214">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="a4b19-215">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="a4b19-215">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="a4b19-216">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a4b19-216">String</span></span>|<span data-ttu-id="a4b19-217">Benutzerdefinierte Zeichenfolge, die die AAD-Attribut definiert.</span><span class="sxs-lookup"><span data-stu-id="a4b19-217">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="a4b19-218">Antwort</span><span class="sxs-lookup"><span data-stu-id="a4b19-218">Response</span></span>
<span data-ttu-id="a4b19-219">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AndroidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="a4b19-219">If successful, this method returns a `201 Created` response code and a [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4b19-220">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a4b19-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4b19-221">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a4b19-221">Request</span></span>
<span data-ttu-id="a4b19-222">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a4b19-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 974

{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="a4b19-223">Antwort</span><span class="sxs-lookup"><span data-stu-id="a4b19-223">Response</span></span>
<span data-ttu-id="a4b19-p121">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a4b19-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




