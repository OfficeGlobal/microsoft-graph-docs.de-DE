---
title: SymantecCodeSigningCertificate aktualisieren
description: Aktualisieren Sie die Eigenschaften eines SymantecCodeSigningCertificate-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f0a938fcb207ee242115eb89cd45da0b1c092a6f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968785"
---
# <a name="update-symanteccodesigningcertificate"></a><span data-ttu-id="e4106-103">SymantecCodeSigningCertificate aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e4106-103">Update symantecCodeSigningCertificate</span></span>

> <span data-ttu-id="e4106-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e4106-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4106-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e4106-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e4106-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e4106-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4106-107">Aktualisieren Sie die Eigenschaften eines [SymantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="e4106-107">Update the properties of a [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e4106-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e4106-108">Prerequisites</span></span>
<span data-ttu-id="e4106-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4106-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4106-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e4106-111">Permission type</span></span>|<span data-ttu-id="e4106-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e4106-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4106-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e4106-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e4106-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4106-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e4106-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e4106-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4106-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e4106-116">Not supported.</span></span>|
|<span data-ttu-id="e4106-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e4106-117">Application</span></span>|<span data-ttu-id="e4106-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e4106-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4106-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4106-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/symantecCodeSigningCertificate
```

## <a name="request-headers"></a><span data-ttu-id="e4106-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e4106-120">Request headers</span></span>
|<span data-ttu-id="e4106-121">Header</span><span class="sxs-lookup"><span data-stu-id="e4106-121">Header</span></span>|<span data-ttu-id="e4106-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e4106-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4106-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4106-123">Authorization</span></span>|<span data-ttu-id="e4106-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e4106-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4106-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e4106-125">Accept</span></span>|<span data-ttu-id="e4106-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e4106-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4106-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e4106-127">Request body</span></span>
<span data-ttu-id="e4106-128">Geben Sie im Textkörper Anforderung für das Objekt [SymantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="e4106-128">In the request body, supply a JSON representation for the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

<span data-ttu-id="e4106-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [SymantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="e4106-129">The following table shows the properties that are required when you create the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md).</span></span>

|<span data-ttu-id="e4106-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e4106-130">Property</span></span>|<span data-ttu-id="e4106-131">Typ</span><span class="sxs-lookup"><span data-stu-id="e4106-131">Type</span></span>|<span data-ttu-id="e4106-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e4106-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4106-133">id</span><span class="sxs-lookup"><span data-stu-id="e4106-133">id</span></span>|<span data-ttu-id="e4106-134">String</span><span class="sxs-lookup"><span data-stu-id="e4106-134">String</span></span>|<span data-ttu-id="e4106-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e4106-135">The key of the entity.</span></span>|
|<span data-ttu-id="e4106-136">content</span><span class="sxs-lookup"><span data-stu-id="e4106-136">content</span></span>|<span data-ttu-id="e4106-137">Binär</span><span class="sxs-lookup"><span data-stu-id="e4106-137">Binary</span></span>|<span data-ttu-id="e4106-138">Das Windows Symantec Codesignierung-Zertifikat im Format Rohdaten.</span><span class="sxs-lookup"><span data-stu-id="e4106-138">The Windows Symantec Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="e4106-139">status</span><span class="sxs-lookup"><span data-stu-id="e4106-139">status</span></span>|[<span data-ttu-id="e4106-140">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="e4106-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="e4106-141">Der Status Cert bereitgestellt oder nicht bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="e4106-141">The Cert Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="e4106-142">Mögliche Werte sind: `notProvisioned` und `provisioned`.</span><span class="sxs-lookup"><span data-stu-id="e4106-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="e4106-143">password</span><span class="sxs-lookup"><span data-stu-id="e4106-143">password</span></span>|<span data-ttu-id="e4106-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e4106-144">String</span></span>|<span data-ttu-id="e4106-145">Das Kennwort für die PFX-Datei.</span><span class="sxs-lookup"><span data-stu-id="e4106-145">The Password required for .pfx file.</span></span>|
|<span data-ttu-id="e4106-146">subjectName</span><span class="sxs-lookup"><span data-stu-id="e4106-146">subjectName</span></span>|<span data-ttu-id="e4106-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e4106-147">String</span></span>|<span data-ttu-id="e4106-148">Der Antragstellername für das Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="e4106-148">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="e4106-149">Betreff</span><span class="sxs-lookup"><span data-stu-id="e4106-149">subject</span></span>|<span data-ttu-id="e4106-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e4106-150">String</span></span>|<span data-ttu-id="e4106-151">Der Wert der Betreff für das Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="e4106-151">The Subject value for the cert.</span></span>|
|<span data-ttu-id="e4106-152">issuerName</span><span class="sxs-lookup"><span data-stu-id="e4106-152">issuerName</span></span>|<span data-ttu-id="e4106-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e4106-153">String</span></span>|<span data-ttu-id="e4106-154">Der Name der Aussteller für das Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="e4106-154">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="e4106-155">Aussteller</span><span class="sxs-lookup"><span data-stu-id="e4106-155">issuer</span></span>|<span data-ttu-id="e4106-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e4106-156">String</span></span>|<span data-ttu-id="e4106-157">Der Wert der Aussteller für das Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="e4106-157">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="e4106-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e4106-158">expirationDateTime</span></span>|<span data-ttu-id="e4106-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4106-159">DateTimeOffset</span></span>|<span data-ttu-id="e4106-160">Das Ablaufdatum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="e4106-160">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="e4106-161">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="e4106-161">uploadDateTime</span></span>|<span data-ttu-id="e4106-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4106-162">DateTimeOffset</span></span>|<span data-ttu-id="e4106-163">Der Typ des der Cert CodeSigning als Symantec Cert.</span><span class="sxs-lookup"><span data-stu-id="e4106-163">The Type of the CodeSigning Cert as Symantec Cert.</span></span>|



## <a name="response"></a><span data-ttu-id="e4106-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4106-164">Response</span></span>
<span data-ttu-id="e4106-165">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [SymantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="e4106-165">If successful, this method returns a `200 OK` response code and an updated [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4106-166">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e4106-166">Example</span></span>
### <a name="request"></a><span data-ttu-id="e4106-167">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4106-167">Request</span></span>
<span data-ttu-id="e4106-168">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e4106-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e4106-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4106-169">Response</span></span>
<span data-ttu-id="e4106-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e4106-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





