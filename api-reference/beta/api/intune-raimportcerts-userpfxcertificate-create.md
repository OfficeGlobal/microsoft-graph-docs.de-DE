---
title: Erstellen von userPFXCertificate
description: Erstellen eines neuen UserPFXCertificate-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8896e3bb300507f0d1a89892852a2e1d4865d9b3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418169"
---
# <a name="create-userpfxcertificate"></a><span data-ttu-id="096e5-103">Erstellen von userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="096e5-103">Create userPFXCertificate</span></span>

> <span data-ttu-id="096e5-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="096e5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="096e5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="096e5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="096e5-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="096e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="096e5-107">Erstellen eines neuen [UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="096e5-107">Create a new [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="096e5-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="096e5-108">Prerequisites</span></span>
<span data-ttu-id="096e5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="096e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="096e5-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="096e5-111">Permission type</span></span>|<span data-ttu-id="096e5-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="096e5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="096e5-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="096e5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="096e5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="096e5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="096e5-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="096e5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="096e5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="096e5-116">Not supported.</span></span>|
|<span data-ttu-id="096e5-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="096e5-117">Application</span></span>|<span data-ttu-id="096e5-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="096e5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="096e5-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="096e5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userPfxCertificates
```

## <a name="request-headers"></a><span data-ttu-id="096e5-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="096e5-120">Request headers</span></span>
|<span data-ttu-id="096e5-121">Header</span><span class="sxs-lookup"><span data-stu-id="096e5-121">Header</span></span>|<span data-ttu-id="096e5-122">Wert</span><span class="sxs-lookup"><span data-stu-id="096e5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="096e5-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="096e5-123">Authorization</span></span>|<span data-ttu-id="096e5-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="096e5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="096e5-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="096e5-125">Accept</span></span>|<span data-ttu-id="096e5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="096e5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="096e5-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="096e5-127">Request body</span></span>
<span data-ttu-id="096e5-128">Geben Sie im Textkörper Anforderung für das Objekt UserPFXCertificate eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="096e5-128">In the request body, supply a JSON representation for the userPFXCertificate object.</span></span>

<span data-ttu-id="096e5-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die UserPFXCertificate erstellen.</span><span class="sxs-lookup"><span data-stu-id="096e5-129">The following table shows the properties that are required when you create the userPFXCertificate.</span></span>

|<span data-ttu-id="096e5-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="096e5-130">Property</span></span>|<span data-ttu-id="096e5-131">Typ</span><span class="sxs-lookup"><span data-stu-id="096e5-131">Type</span></span>|<span data-ttu-id="096e5-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="096e5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="096e5-133">id</span><span class="sxs-lookup"><span data-stu-id="096e5-133">id</span></span>|<span data-ttu-id="096e5-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="096e5-134">String</span></span>|<span data-ttu-id="096e5-135">Eindeutiger Bezeichner für das PFX-Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="096e5-135">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="096e5-136">Fingerabdruck</span><span class="sxs-lookup"><span data-stu-id="096e5-136">thumbprint</span></span>|<span data-ttu-id="096e5-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="096e5-137">String</span></span>|<span data-ttu-id="096e5-138">SHA-1-Fingerabdruck des Zertifikats PFX.</span><span class="sxs-lookup"><span data-stu-id="096e5-138">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="096e5-139">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="096e5-139">intendedPurpose</span></span>|[<span data-ttu-id="096e5-140">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="096e5-140">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="096e5-141">Des Zertifikats beabsichtigten Zweck aus der Punkt der Ansicht der Bereitstellung.</span><span class="sxs-lookup"><span data-stu-id="096e5-141">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="096e5-142">Mögliche Werte sind: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn` und `wifi`.</span><span class="sxs-lookup"><span data-stu-id="096e5-142">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="096e5-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="096e5-143">userPrincipalName</span></span>|<span data-ttu-id="096e5-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="096e5-144">String</span></span>|<span data-ttu-id="096e5-145">Benutzerprinzipalname des PFX-Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="096e5-145">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="096e5-146">startDateTime</span><span class="sxs-lookup"><span data-stu-id="096e5-146">startDateTime</span></span>|<span data-ttu-id="096e5-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="096e5-147">DateTimeOffset</span></span>|<span data-ttu-id="096e5-148">Gültigkeitsdauer der starten Datum/Uhrzeit.</span><span class="sxs-lookup"><span data-stu-id="096e5-148">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="096e5-149">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="096e5-149">expirationDateTime</span></span>|<span data-ttu-id="096e5-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="096e5-150">DateTimeOffset</span></span>|<span data-ttu-id="096e5-151">Des Zertifikats Gültigkeit Ablauf Datum/Uhrzeit.</span><span class="sxs-lookup"><span data-stu-id="096e5-151">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="096e5-152">providerName</span><span class="sxs-lookup"><span data-stu-id="096e5-152">providerName</span></span>|<span data-ttu-id="096e5-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="096e5-153">String</span></span>|<span data-ttu-id="096e5-154">Kryptografieanbieter zum Verschlüsseln von diesem Blob verwendet.</span><span class="sxs-lookup"><span data-stu-id="096e5-154">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="096e5-155">Schlüsselname</span><span class="sxs-lookup"><span data-stu-id="096e5-155">keyName</span></span>|<span data-ttu-id="096e5-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="096e5-156">String</span></span>|<span data-ttu-id="096e5-157">Name des Schlüssels (innerhalb der Anbieter) verwendet, um den Blob zu verschlüsseln.</span><span class="sxs-lookup"><span data-stu-id="096e5-157">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="096e5-158">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="096e5-158">paddingScheme</span></span>|[<span data-ttu-id="096e5-159">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="096e5-159">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="096e5-160">Abstand bei der Verschlüsselung/Entschlüsselung der vom Anbieter verwendete Schema.</span><span class="sxs-lookup"><span data-stu-id="096e5-160">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="096e5-161">Mögliche Werte sind: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384` und `oaepSha512`.</span><span class="sxs-lookup"><span data-stu-id="096e5-161">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="096e5-162">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="096e5-162">encryptedPfxBlob</span></span>|<span data-ttu-id="096e5-163">Binär</span><span class="sxs-lookup"><span data-stu-id="096e5-163">Binary</span></span>|<span data-ttu-id="096e5-164">Blob für verschlüsselte PFX.</span><span class="sxs-lookup"><span data-stu-id="096e5-164">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="096e5-165">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="096e5-165">encryptedPfxPassword</span></span>|<span data-ttu-id="096e5-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="096e5-166">String</span></span>|<span data-ttu-id="096e5-167">Verschlüsselte PFX-Kennwort ein.</span><span class="sxs-lookup"><span data-stu-id="096e5-167">Encrypted PFX password.</span></span>|
|<span data-ttu-id="096e5-168">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="096e5-168">createdDateTime</span></span>|<span data-ttu-id="096e5-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="096e5-169">DateTimeOffset</span></span>|<span data-ttu-id="096e5-170">Datum/Uhrzeit, wenn dieses PFX-Zertifikat importiert wurde.</span><span class="sxs-lookup"><span data-stu-id="096e5-170">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="096e5-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="096e5-171">lastModifiedDateTime</span></span>|<span data-ttu-id="096e5-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="096e5-172">DateTimeOffset</span></span>|<span data-ttu-id="096e5-173">Datum/Uhrzeit der letzten dieses PFX-Zertifikat Änderung.</span><span class="sxs-lookup"><span data-stu-id="096e5-173">Date/time when this PFX certificate was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="096e5-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="096e5-174">Response</span></span>
<span data-ttu-id="096e5-175">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="096e5-175">If successful, this method returns a `201 Created` response code and a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="096e5-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="096e5-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="096e5-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="096e5-177">Request</span></span>
<span data-ttu-id="096e5-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="096e5-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates
Content-type: application/json
Content-length: 523

{
  "@odata.type": "#microsoft.graph.userPFXCertificate",
  "thumbprint": "Thumbprint value",
  "intendedPurpose": "smimeEncryption",
  "userPrincipalName": "User Principal Name value",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "providerName": "Provider Name value",
  "keyName": "Key Name value",
  "paddingScheme": "pkcs1",
  "encryptedPfxBlob": "ZW5jcnlwdGVkUGZ4QmxvYg==",
  "encryptedPfxPassword": "Encrypted Pfx Password value"
}
```

### <a name="response"></a><span data-ttu-id="096e5-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="096e5-179">Response</span></span>
<span data-ttu-id="096e5-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="096e5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 695

{
  "@odata.type": "#microsoft.graph.userPFXCertificate",
  "id": "045c159b-159b-045c-9b15-5c049b155c04",
  "thumbprint": "Thumbprint value",
  "intendedPurpose": "smimeEncryption",
  "userPrincipalName": "User Principal Name value",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "providerName": "Provider Name value",
  "keyName": "Key Name value",
  "paddingScheme": "pkcs1",
  "encryptedPfxBlob": "ZW5jcnlwdGVkUGZ4QmxvYg==",
  "encryptedPfxPassword": "Encrypted Pfx Password value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




