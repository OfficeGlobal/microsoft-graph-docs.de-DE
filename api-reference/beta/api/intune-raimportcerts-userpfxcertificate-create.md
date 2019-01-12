---
title: Erstellen von userPFXCertificate
description: Erstellen eines neuen UserPFXCertificate-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d98275975a0d9e46251521b76b55b0e8d67d226b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984486"
---
# <a name="create-userpfxcertificate"></a><span data-ttu-id="8b948-103">Erstellen von userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="8b948-103">Create userPFXCertificate</span></span>

> <span data-ttu-id="8b948-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8b948-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b948-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8b948-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8b948-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8b948-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8b948-107">Erstellen eines neuen [UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="8b948-107">Create a new [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8b948-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8b948-108">Prerequisites</span></span>
<span data-ttu-id="8b948-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b948-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b948-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8b948-111">Permission type</span></span>|<span data-ttu-id="8b948-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8b948-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b948-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8b948-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8b948-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b948-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8b948-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8b948-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b948-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8b948-116">Not supported.</span></span>|
|<span data-ttu-id="8b948-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8b948-117">Application</span></span>|<span data-ttu-id="8b948-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8b948-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b948-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b948-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userPfxCertificates
```

## <a name="request-headers"></a><span data-ttu-id="8b948-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8b948-120">Request headers</span></span>
|<span data-ttu-id="8b948-121">Header</span><span class="sxs-lookup"><span data-stu-id="8b948-121">Header</span></span>|<span data-ttu-id="8b948-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8b948-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b948-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b948-123">Authorization</span></span>|<span data-ttu-id="8b948-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8b948-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b948-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8b948-125">Accept</span></span>|<span data-ttu-id="8b948-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8b948-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b948-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8b948-127">Request body</span></span>
<span data-ttu-id="8b948-128">Geben Sie im Textkörper Anforderung für das Objekt UserPFXCertificate eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="8b948-128">In the request body, supply a JSON representation for the userPFXCertificate object.</span></span>

<span data-ttu-id="8b948-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die UserPFXCertificate erstellen.</span><span class="sxs-lookup"><span data-stu-id="8b948-129">The following table shows the properties that are required when you create the userPFXCertificate.</span></span>

|<span data-ttu-id="8b948-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8b948-130">Property</span></span>|<span data-ttu-id="8b948-131">Typ</span><span class="sxs-lookup"><span data-stu-id="8b948-131">Type</span></span>|<span data-ttu-id="8b948-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8b948-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b948-133">id</span><span class="sxs-lookup"><span data-stu-id="8b948-133">id</span></span>|<span data-ttu-id="8b948-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8b948-134">String</span></span>|<span data-ttu-id="8b948-135">Eindeutiger Bezeichner für das PFX-Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="8b948-135">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="8b948-136">Fingerabdruck</span><span class="sxs-lookup"><span data-stu-id="8b948-136">thumbprint</span></span>|<span data-ttu-id="8b948-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8b948-137">String</span></span>|<span data-ttu-id="8b948-138">SHA-1-Fingerabdruck des Zertifikats PFX.</span><span class="sxs-lookup"><span data-stu-id="8b948-138">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="8b948-139">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="8b948-139">intendedPurpose</span></span>|[<span data-ttu-id="8b948-140">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="8b948-140">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="8b948-141">Des Zertifikats beabsichtigten Zweck aus der Punkt der Ansicht der Bereitstellung.</span><span class="sxs-lookup"><span data-stu-id="8b948-141">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="8b948-142">Mögliche Werte sind: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn` und `wifi`.</span><span class="sxs-lookup"><span data-stu-id="8b948-142">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="8b948-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8b948-143">userPrincipalName</span></span>|<span data-ttu-id="8b948-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8b948-144">String</span></span>|<span data-ttu-id="8b948-145">Benutzerprinzipalname des PFX-Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="8b948-145">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="8b948-146">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8b948-146">startDateTime</span></span>|<span data-ttu-id="8b948-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b948-147">DateTimeOffset</span></span>|<span data-ttu-id="8b948-148">Gültigkeitsdauer der starten Datum/Uhrzeit.</span><span class="sxs-lookup"><span data-stu-id="8b948-148">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="8b948-149">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8b948-149">expirationDateTime</span></span>|<span data-ttu-id="8b948-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b948-150">DateTimeOffset</span></span>|<span data-ttu-id="8b948-151">Des Zertifikats Gültigkeit Ablauf Datum/Uhrzeit.</span><span class="sxs-lookup"><span data-stu-id="8b948-151">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="8b948-152">providerName</span><span class="sxs-lookup"><span data-stu-id="8b948-152">providerName</span></span>|<span data-ttu-id="8b948-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8b948-153">String</span></span>|<span data-ttu-id="8b948-154">Kryptografieanbieter zum Verschlüsseln von diesem Blob verwendet.</span><span class="sxs-lookup"><span data-stu-id="8b948-154">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="8b948-155">Schlüsselname</span><span class="sxs-lookup"><span data-stu-id="8b948-155">keyName</span></span>|<span data-ttu-id="8b948-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8b948-156">String</span></span>|<span data-ttu-id="8b948-157">Name des Schlüssels (innerhalb der Anbieter) verwendet, um den Blob zu verschlüsseln.</span><span class="sxs-lookup"><span data-stu-id="8b948-157">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="8b948-158">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="8b948-158">paddingScheme</span></span>|[<span data-ttu-id="8b948-159">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="8b948-159">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="8b948-160">Abstand bei der Verschlüsselung/Entschlüsselung der vom Anbieter verwendete Schema.</span><span class="sxs-lookup"><span data-stu-id="8b948-160">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="8b948-161">Mögliche Werte sind: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384` und `oaepSha512`.</span><span class="sxs-lookup"><span data-stu-id="8b948-161">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="8b948-162">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="8b948-162">encryptedPfxBlob</span></span>|<span data-ttu-id="8b948-163">Binär</span><span class="sxs-lookup"><span data-stu-id="8b948-163">Binary</span></span>|<span data-ttu-id="8b948-164">Blob für verschlüsselte PFX.</span><span class="sxs-lookup"><span data-stu-id="8b948-164">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="8b948-165">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="8b948-165">encryptedPfxPassword</span></span>|<span data-ttu-id="8b948-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8b948-166">String</span></span>|<span data-ttu-id="8b948-167">Verschlüsselte PFX-Kennwort ein.</span><span class="sxs-lookup"><span data-stu-id="8b948-167">Encrypted PFX password.</span></span>|
|<span data-ttu-id="8b948-168">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8b948-168">createdDateTime</span></span>|<span data-ttu-id="8b948-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b948-169">DateTimeOffset</span></span>|<span data-ttu-id="8b948-170">Datum/Uhrzeit, wenn dieses PFX-Zertifikat importiert wurde.</span><span class="sxs-lookup"><span data-stu-id="8b948-170">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="8b948-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8b948-171">lastModifiedDateTime</span></span>|<span data-ttu-id="8b948-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b948-172">DateTimeOffset</span></span>|<span data-ttu-id="8b948-173">Datum/Uhrzeit der letzten dieses PFX-Zertifikat Änderung.</span><span class="sxs-lookup"><span data-stu-id="8b948-173">Date/time when this PFX certificate was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="8b948-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b948-174">Response</span></span>
<span data-ttu-id="8b948-175">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="8b948-175">If successful, this method returns a `201 Created` response code and a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b948-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8b948-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="8b948-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8b948-177">Request</span></span>
<span data-ttu-id="8b948-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8b948-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates
Content-type: application/json
Content-length: 587

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
  "encryptedPfxPassword": "Encrypted Pfx Password value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```

### <a name="response"></a><span data-ttu-id="8b948-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="8b948-179">Response</span></span>
<span data-ttu-id="8b948-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8b948-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





