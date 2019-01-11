---
title: SymantecCodeSigningCertificate aktualisieren
description: Aktualisieren Sie die Eigenschaften eines SymantecCodeSigningCertificate-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7d95627e9a2c678097be0c3cb818a03906e8a06f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824738"
---
# <a name="update-symanteccodesigningcertificate"></a><span data-ttu-id="fa856-103">SymantecCodeSigningCertificate aktualisieren</span><span class="sxs-lookup"><span data-stu-id="fa856-103">Update symantecCodeSigningCertificate</span></span>

> <span data-ttu-id="fa856-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fa856-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa856-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fa856-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fa856-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fa856-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa856-107">Aktualisieren Sie die Eigenschaften eines [SymantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="fa856-107">Update the properties of a [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fa856-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fa856-108">Prerequisites</span></span>
<span data-ttu-id="fa856-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa856-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa856-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fa856-111">Permission type</span></span>|<span data-ttu-id="fa856-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fa856-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa856-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fa856-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fa856-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa856-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fa856-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fa856-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa856-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa856-116">Not supported.</span></span>|
|<span data-ttu-id="fa856-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fa856-117">Application</span></span>|<span data-ttu-id="fa856-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa856-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa856-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa856-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/symantecCodeSigningCertificate
```

## <a name="request-headers"></a><span data-ttu-id="fa856-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fa856-120">Request headers</span></span>
|<span data-ttu-id="fa856-121">Header</span><span class="sxs-lookup"><span data-stu-id="fa856-121">Header</span></span>|<span data-ttu-id="fa856-122">Wert</span><span class="sxs-lookup"><span data-stu-id="fa856-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa856-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa856-123">Authorization</span></span>|<span data-ttu-id="fa856-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fa856-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa856-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fa856-125">Accept</span></span>|<span data-ttu-id="fa856-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fa856-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa856-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fa856-127">Request body</span></span>
<span data-ttu-id="fa856-128">Geben Sie im Textkörper Anforderung für das Objekt [SymantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="fa856-128">In the request body, supply a JSON representation for the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

<span data-ttu-id="fa856-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [SymantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="fa856-129">The following table shows the properties that are required when you create the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md).</span></span>

|<span data-ttu-id="fa856-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fa856-130">Property</span></span>|<span data-ttu-id="fa856-131">Typ</span><span class="sxs-lookup"><span data-stu-id="fa856-131">Type</span></span>|<span data-ttu-id="fa856-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa856-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa856-133">id</span><span class="sxs-lookup"><span data-stu-id="fa856-133">id</span></span>|<span data-ttu-id="fa856-134">String</span><span class="sxs-lookup"><span data-stu-id="fa856-134">String</span></span>|<span data-ttu-id="fa856-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="fa856-135">The key of the entity.</span></span>|
|<span data-ttu-id="fa856-136">content</span><span class="sxs-lookup"><span data-stu-id="fa856-136">content</span></span>|<span data-ttu-id="fa856-137">Binär</span><span class="sxs-lookup"><span data-stu-id="fa856-137">Binary</span></span>|<span data-ttu-id="fa856-138">Das Windows Symantec Codesignierung-Zertifikat im Format Rohdaten.</span><span class="sxs-lookup"><span data-stu-id="fa856-138">The Windows Symantec Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="fa856-139">status</span><span class="sxs-lookup"><span data-stu-id="fa856-139">status</span></span>|[<span data-ttu-id="fa856-140">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="fa856-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="fa856-141">Der Status Cert bereitgestellt oder nicht bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="fa856-141">The Cert Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="fa856-142">Mögliche Werte sind: `notProvisioned` und `provisioned`.</span><span class="sxs-lookup"><span data-stu-id="fa856-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="fa856-143">password</span><span class="sxs-lookup"><span data-stu-id="fa856-143">password</span></span>|<span data-ttu-id="fa856-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa856-144">String</span></span>|<span data-ttu-id="fa856-145">Das Kennwort für die PFX-Datei.</span><span class="sxs-lookup"><span data-stu-id="fa856-145">The Password required for .pfx file.</span></span>|
|<span data-ttu-id="fa856-146">subjectName</span><span class="sxs-lookup"><span data-stu-id="fa856-146">subjectName</span></span>|<span data-ttu-id="fa856-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa856-147">String</span></span>|<span data-ttu-id="fa856-148">Der Antragstellername für das Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="fa856-148">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="fa856-149">Betreff</span><span class="sxs-lookup"><span data-stu-id="fa856-149">subject</span></span>|<span data-ttu-id="fa856-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa856-150">String</span></span>|<span data-ttu-id="fa856-151">Der Wert der Betreff für das Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="fa856-151">The Subject value for the cert.</span></span>|
|<span data-ttu-id="fa856-152">issuerName</span><span class="sxs-lookup"><span data-stu-id="fa856-152">issuerName</span></span>|<span data-ttu-id="fa856-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa856-153">String</span></span>|<span data-ttu-id="fa856-154">Der Name der Aussteller für das Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="fa856-154">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="fa856-155">Aussteller</span><span class="sxs-lookup"><span data-stu-id="fa856-155">issuer</span></span>|<span data-ttu-id="fa856-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa856-156">String</span></span>|<span data-ttu-id="fa856-157">Der Wert der Aussteller für das Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="fa856-157">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="fa856-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="fa856-158">expirationDateTime</span></span>|<span data-ttu-id="fa856-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa856-159">DateTimeOffset</span></span>|<span data-ttu-id="fa856-160">Das Ablaufdatum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="fa856-160">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="fa856-161">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="fa856-161">uploadDateTime</span></span>|<span data-ttu-id="fa856-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa856-162">DateTimeOffset</span></span>|<span data-ttu-id="fa856-163">Der Typ des der Cert CodeSigning als Symantec Cert.</span><span class="sxs-lookup"><span data-stu-id="fa856-163">The Type of the CodeSigning Cert as Symantec Cert.</span></span>|



## <a name="response"></a><span data-ttu-id="fa856-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa856-164">Response</span></span>
<span data-ttu-id="fa856-165">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [SymantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="fa856-165">If successful, this method returns a `200 OK` response code and an updated [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa856-166">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fa856-166">Example</span></span>
### <a name="request"></a><span data-ttu-id="fa856-167">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa856-167">Request</span></span>
<span data-ttu-id="fa856-168">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fa856-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/symantecCodeSigningCertificate
Content-type: application/json
Content-length: 352

{
  "content": "Y29udGVudA==",
  "status": "provisioned",
  "password": "Password value",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
}
```

### <a name="response"></a><span data-ttu-id="fa856-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa856-169">Response</span></span>
<span data-ttu-id="fa856-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fa856-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 470

{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "id": "00ffe83e-e83e-00ff-3ee8-ff003ee8ff00",
  "content": "Y29udGVudA==",
  "status": "provisioned",
  "password": "Password value",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
}
```





