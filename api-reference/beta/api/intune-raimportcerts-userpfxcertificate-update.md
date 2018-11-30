---
title: UserPFXCertificate aktualisieren
description: Aktualisieren Sie die Eigenschaften eines UserPFXCertificate-Objekts.
ms.openlocfilehash: 9fde1e8ff073df7acf76119ace0848616424951a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27057927"
---
# <a name="update-userpfxcertificate"></a><span data-ttu-id="8e9fa-103">UserPFXCertificate aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8e9fa-103">Update userPFXCertificate</span></span>

> <span data-ttu-id="8e9fa-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8e9fa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e9fa-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8e9fa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8e9fa-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8e9fa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e9fa-107">Aktualisieren Sie die Eigenschaften eines [UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="8e9fa-107">Update the properties of a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8e9fa-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8e9fa-108">Prerequisites</span></span>
<span data-ttu-id="8e9fa-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e9fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e9fa-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8e9fa-111">Permission type</span></span>|<span data-ttu-id="8e9fa-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8e9fa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e9fa-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8e9fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8e9fa-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e9fa-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8e9fa-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8e9fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e9fa-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8e9fa-116">Not supported.</span></span>|
|<span data-ttu-id="8e9fa-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8e9fa-117">Application</span></span>|<span data-ttu-id="8e9fa-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8e9fa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e9fa-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8e9fa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="8e9fa-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8e9fa-120">Request headers</span></span>
|<span data-ttu-id="8e9fa-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8e9fa-121">Header</span></span>|<span data-ttu-id="8e9fa-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8e9fa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e9fa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e9fa-123">Authorization</span></span>|<span data-ttu-id="8e9fa-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8e9fa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e9fa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8e9fa-125">Accept</span></span>|<span data-ttu-id="8e9fa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8e9fa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e9fa-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8e9fa-127">Request body</span></span>
<span data-ttu-id="8e9fa-128">Geben Sie im Textkörper Anforderung für das Objekt [UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="8e9fa-128">In the request body, supply a JSON representation for the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

<span data-ttu-id="8e9fa-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="8e9fa-129">The following table shows the properties that are required when you create the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).</span></span>

|<span data-ttu-id="8e9fa-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8e9fa-130">Property</span></span>|<span data-ttu-id="8e9fa-131">Typ</span><span class="sxs-lookup"><span data-stu-id="8e9fa-131">Type</span></span>|<span data-ttu-id="8e9fa-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8e9fa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e9fa-133">id</span><span class="sxs-lookup"><span data-stu-id="8e9fa-133">id</span></span>|<span data-ttu-id="8e9fa-134">String</span><span class="sxs-lookup"><span data-stu-id="8e9fa-134">String</span></span>|<span data-ttu-id="8e9fa-135">Eindeutiger Bezeichner für das PFX-Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="8e9fa-135">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="8e9fa-136">Fingerabdruck</span><span class="sxs-lookup"><span data-stu-id="8e9fa-136">thumbprint</span></span>|<span data-ttu-id="8e9fa-137">String</span><span class="sxs-lookup"><span data-stu-id="8e9fa-137">String</span></span>|<span data-ttu-id="8e9fa-138">SHA-1-Fingerabdruck des Zertifikats PFX.</span><span class="sxs-lookup"><span data-stu-id="8e9fa-138">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="8e9fa-139">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="8e9fa-139">intendedPurpose</span></span>|[<span data-ttu-id="8e9fa-140">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="8e9fa-140">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="8e9fa-141">Des Zertifikats beabsichtigten Zweck aus der Punkt der Ansicht der Bereitstellung.</span><span class="sxs-lookup"><span data-stu-id="8e9fa-141">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="8e9fa-142">Mögliche Werte sind: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn` und `wifi`.</span><span class="sxs-lookup"><span data-stu-id="8e9fa-142">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="8e9fa-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8e9fa-143">userPrincipalName</span></span>|<span data-ttu-id="8e9fa-144">String</span><span class="sxs-lookup"><span data-stu-id="8e9fa-144">String</span></span>|<span data-ttu-id="8e9fa-145">Benutzerprinzipalname des PFX-Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="8e9fa-145">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="8e9fa-146">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8e9fa-146">startDateTime</span></span>|<span data-ttu-id="8e9fa-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e9fa-147">DateTimeOffset</span></span>|<span data-ttu-id="8e9fa-148">Gültigkeitsdauer der starten Datum/Uhrzeit.</span><span class="sxs-lookup"><span data-stu-id="8e9fa-148">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="8e9fa-149">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8e9fa-149">expirationDateTime</span></span>|<span data-ttu-id="8e9fa-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e9fa-150">DateTimeOffset</span></span>|<span data-ttu-id="8e9fa-151">Des Zertifikats Gültigkeit Ablauf Datum/Uhrzeit.</span><span class="sxs-lookup"><span data-stu-id="8e9fa-151">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="8e9fa-152">providerName</span><span class="sxs-lookup"><span data-stu-id="8e9fa-152">providerName</span></span>|<span data-ttu-id="8e9fa-153">String</span><span class="sxs-lookup"><span data-stu-id="8e9fa-153">String</span></span>|<span data-ttu-id="8e9fa-154">Kryptografieanbieter zum Verschlüsseln von diesem Blob verwendet.</span><span class="sxs-lookup"><span data-stu-id="8e9fa-154">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="8e9fa-155">Schlüsselname</span><span class="sxs-lookup"><span data-stu-id="8e9fa-155">keyName</span></span>|<span data-ttu-id="8e9fa-156">String</span><span class="sxs-lookup"><span data-stu-id="8e9fa-156">String</span></span>|<span data-ttu-id="8e9fa-157">Name des Schlüssels (innerhalb der Anbieter) verwendet, um den Blob zu verschlüsseln.</span><span class="sxs-lookup"><span data-stu-id="8e9fa-157">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="8e9fa-158">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="8e9fa-158">paddingScheme</span></span>|[<span data-ttu-id="8e9fa-159">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="8e9fa-159">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="8e9fa-160">Abstand bei der Verschlüsselung/Entschlüsselung der vom Anbieter verwendete Schema.</span><span class="sxs-lookup"><span data-stu-id="8e9fa-160">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="8e9fa-161">Mögliche Werte sind: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384` und `oaepSha512`.</span><span class="sxs-lookup"><span data-stu-id="8e9fa-161">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="8e9fa-162">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="8e9fa-162">encryptedPfxBlob</span></span>|<span data-ttu-id="8e9fa-163">Binär</span><span class="sxs-lookup"><span data-stu-id="8e9fa-163">Binary</span></span>|<span data-ttu-id="8e9fa-164">Blob für verschlüsselte PFX.</span><span class="sxs-lookup"><span data-stu-id="8e9fa-164">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="8e9fa-165">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="8e9fa-165">encryptedPfxPassword</span></span>|<span data-ttu-id="8e9fa-166">String</span><span class="sxs-lookup"><span data-stu-id="8e9fa-166">String</span></span>|<span data-ttu-id="8e9fa-167">Verschlüsselte PFX-Kennwort ein.</span><span class="sxs-lookup"><span data-stu-id="8e9fa-167">Encrypted PFX password.</span></span>|
|<span data-ttu-id="8e9fa-168">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8e9fa-168">createdDateTime</span></span>|<span data-ttu-id="8e9fa-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e9fa-169">DateTimeOffset</span></span>|<span data-ttu-id="8e9fa-170">Datum/Uhrzeit, wenn dieses PFX-Zertifikat importiert wurde.</span><span class="sxs-lookup"><span data-stu-id="8e9fa-170">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="8e9fa-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e9fa-171">lastModifiedDateTime</span></span>|<span data-ttu-id="8e9fa-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e9fa-172">DateTimeOffset</span></span>|<span data-ttu-id="8e9fa-173">Datum/Uhrzeit der letzten dieses PFX-Zertifikat Änderung.</span><span class="sxs-lookup"><span data-stu-id="8e9fa-173">Date/time when this PFX certificate was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="8e9fa-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="8e9fa-174">Response</span></span>
<span data-ttu-id="8e9fa-175">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="8e9fa-175">If successful, this method returns a `200 OK` response code and an updated [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e9fa-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8e9fa-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="8e9fa-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8e9fa-177">Request</span></span>
<span data-ttu-id="8e9fa-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8e9fa-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates/{userPFXCertificateId}
Content-type: application/json
Content-length: 530

{
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
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```

### <a name="response"></a><span data-ttu-id="8e9fa-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="8e9fa-179">Response</span></span>
<span data-ttu-id="8e9fa-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8e9fa-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





