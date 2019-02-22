---
title: UserPFXCertificate erstellen
description: Erstellen eines neuen userPFXCertificate-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bf704664785eb1d61aacea3b72dcaed7a02bd24d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158709"
---
# <a name="create-userpfxcertificate"></a><span data-ttu-id="ac1f8-103">UserPFXCertificate erstellen</span><span class="sxs-lookup"><span data-stu-id="ac1f8-103">Create userPFXCertificate</span></span>

> <span data-ttu-id="ac1f8-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ac1f8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac1f8-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ac1f8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac1f8-106">Erstellen eines neuen [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ac1f8-106">Create a new [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ac1f8-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ac1f8-107">Prerequisites</span></span>
<span data-ttu-id="ac1f8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ac1f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ac1f8-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ac1f8-110">Permission type</span></span>|<span data-ttu-id="ac1f8-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ac1f8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac1f8-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ac1f8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ac1f8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac1f8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ac1f8-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ac1f8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac1f8-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ac1f8-115">Not supported.</span></span>|
|<span data-ttu-id="ac1f8-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ac1f8-116">Application</span></span>|<span data-ttu-id="ac1f8-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ac1f8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac1f8-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ac1f8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userPfxCertificates
```

## <a name="request-headers"></a><span data-ttu-id="ac1f8-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ac1f8-119">Request headers</span></span>
|<span data-ttu-id="ac1f8-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ac1f8-120">Header</span></span>|<span data-ttu-id="ac1f8-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ac1f8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac1f8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac1f8-122">Authorization</span></span>|<span data-ttu-id="ac1f8-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ac1f8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac1f8-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ac1f8-124">Accept</span></span>|<span data-ttu-id="ac1f8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ac1f8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac1f8-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ac1f8-126">Request body</span></span>
<span data-ttu-id="ac1f8-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das userPFXCertificate-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="ac1f8-127">In the request body, supply a JSON representation for the userPFXCertificate object.</span></span>

<span data-ttu-id="ac1f8-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der userPFXCertificate erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="ac1f8-128">The following table shows the properties that are required when you create the userPFXCertificate.</span></span>

|<span data-ttu-id="ac1f8-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ac1f8-129">Property</span></span>|<span data-ttu-id="ac1f8-130">Typ</span><span class="sxs-lookup"><span data-stu-id="ac1f8-130">Type</span></span>|<span data-ttu-id="ac1f8-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ac1f8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac1f8-132">id</span><span class="sxs-lookup"><span data-stu-id="ac1f8-132">id</span></span>|<span data-ttu-id="ac1f8-133">string</span><span class="sxs-lookup"><span data-stu-id="ac1f8-133">String</span></span>|<span data-ttu-id="ac1f8-134">Eindeutiger Bezeichner für das PFX-Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="ac1f8-134">Unique identifier for the PFX certificate.</span></span>|
|<span data-ttu-id="ac1f8-135">Fingerabdruck</span><span class="sxs-lookup"><span data-stu-id="ac1f8-135">thumbprint</span></span>|<span data-ttu-id="ac1f8-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ac1f8-136">String</span></span>|<span data-ttu-id="ac1f8-137">SHA-1 Fingerabdruck des PFX-Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="ac1f8-137">SHA-1 thumbprint of the PFX certificate.</span></span>|
|<span data-ttu-id="ac1f8-138">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="ac1f8-138">intendedPurpose</span></span>|[<span data-ttu-id="ac1f8-139">userPfxIntendedPurpose</span><span class="sxs-lookup"><span data-stu-id="ac1f8-139">userPfxIntendedPurpose</span></span>](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|<span data-ttu-id="ac1f8-140">Zweck des Zertifikats aus der Sicht der Bereitstellung.</span><span class="sxs-lookup"><span data-stu-id="ac1f8-140">Certificate's intended purpose from the point-of-view of deployment.</span></span> <span data-ttu-id="ac1f8-141">Mögliche Werte: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="ac1f8-141">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|
|<span data-ttu-id="ac1f8-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ac1f8-142">userPrincipalName</span></span>|<span data-ttu-id="ac1f8-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ac1f8-143">String</span></span>|<span data-ttu-id="ac1f8-144">Benutzerprinzipal Name des PFX-Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="ac1f8-144">User Principal Name of the PFX certificate.</span></span>|
|<span data-ttu-id="ac1f8-145">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ac1f8-145">startDateTime</span></span>|<span data-ttu-id="ac1f8-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac1f8-146">DateTimeOffset</span></span>|<span data-ttu-id="ac1f8-147">Gültigkeitsdatum/-Uhrzeit des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="ac1f8-147">Certificate's validity start date/time.</span></span>|
|<span data-ttu-id="ac1f8-148">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ac1f8-148">expirationDateTime</span></span>|<span data-ttu-id="ac1f8-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac1f8-149">DateTimeOffset</span></span>|<span data-ttu-id="ac1f8-150">Gültigkeitsablauf Datum/-Uhrzeit des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="ac1f8-150">Certificate's validity expiration date/time.</span></span>|
|<span data-ttu-id="ac1f8-151">providerName</span><span class="sxs-lookup"><span data-stu-id="ac1f8-151">providerName</span></span>|<span data-ttu-id="ac1f8-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ac1f8-152">String</span></span>|<span data-ttu-id="ac1f8-153">Crypto-Anbieter, der zum Verschlüsseln dieses BLOBs verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="ac1f8-153">Crypto provider used to encrypt this blob.</span></span>|
|<span data-ttu-id="ac1f8-154">keyName</span><span class="sxs-lookup"><span data-stu-id="ac1f8-154">keyName</span></span>|<span data-ttu-id="ac1f8-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ac1f8-155">String</span></span>|<span data-ttu-id="ac1f8-156">Der Name des Schlüssels (innerhalb des Anbieters), der zum Verschlüsseln des BLOBs verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="ac1f8-156">Name of the key (within the provider) used to encrypt the blob.</span></span>|
|<span data-ttu-id="ac1f8-157">paddingScheme</span><span class="sxs-lookup"><span data-stu-id="ac1f8-157">paddingScheme</span></span>|[<span data-ttu-id="ac1f8-158">userPfxPaddingScheme</span><span class="sxs-lookup"><span data-stu-id="ac1f8-158">userPfxPaddingScheme</span></span>](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|<span data-ttu-id="ac1f8-159">Vom Anbieter während der Verschlüsselung/Entschlüsselung verwendetes Padding-Schema.</span><span class="sxs-lookup"><span data-stu-id="ac1f8-159">Padding scheme used by the provider during encryption/decryption.</span></span> <span data-ttu-id="ac1f8-160">Mögliche Werte sind: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384` und `oaepSha512`.</span><span class="sxs-lookup"><span data-stu-id="ac1f8-160">Possible values are: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.</span></span>|
|<span data-ttu-id="ac1f8-161">encryptedPfxBlob</span><span class="sxs-lookup"><span data-stu-id="ac1f8-161">encryptedPfxBlob</span></span>|<span data-ttu-id="ac1f8-162">Binär</span><span class="sxs-lookup"><span data-stu-id="ac1f8-162">Binary</span></span>|<span data-ttu-id="ac1f8-163">Verschlüsselter PFX-BLOB.</span><span class="sxs-lookup"><span data-stu-id="ac1f8-163">Encrypted PFX blob.</span></span>|
|<span data-ttu-id="ac1f8-164">encryptedPfxPassword</span><span class="sxs-lookup"><span data-stu-id="ac1f8-164">encryptedPfxPassword</span></span>|<span data-ttu-id="ac1f8-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ac1f8-165">String</span></span>|<span data-ttu-id="ac1f8-166">Kennwort für verSchlüsselte PFX.</span><span class="sxs-lookup"><span data-stu-id="ac1f8-166">Encrypted PFX password.</span></span>|
|<span data-ttu-id="ac1f8-167">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ac1f8-167">createdDateTime</span></span>|<span data-ttu-id="ac1f8-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac1f8-168">DateTimeOffset</span></span>|<span data-ttu-id="ac1f8-169">Datum/Uhrzeit des Imports dieses PFX-Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="ac1f8-169">Date/time when this PFX certificate was imported.</span></span>|
|<span data-ttu-id="ac1f8-170">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ac1f8-170">lastModifiedDateTime</span></span>|<span data-ttu-id="ac1f8-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac1f8-171">DateTimeOffset</span></span>|<span data-ttu-id="ac1f8-172">Datum/Uhrzeit der letzten Änderung dieses PFX-Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="ac1f8-172">Date/time when this PFX certificate was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="ac1f8-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="ac1f8-173">Response</span></span>
<span data-ttu-id="ac1f8-174">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ac1f8-174">If successful, this method returns a `201 Created` response code and a [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac1f8-175">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ac1f8-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac1f8-176">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ac1f8-176">Request</span></span>
<span data-ttu-id="ac1f8-177">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ac1f8-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ac1f8-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="ac1f8-178">Response</span></span>
<span data-ttu-id="ac1f8-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ac1f8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




