---
title: SymantecCodeSigningCertificate aktualisieren
description: Aktualisieren der Eigenschaften eines symantecCodeSigningCertificate-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 56c665a75d594d2f1ad0e28c3800348f0fbde9c3
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957528"
---
# <a name="update-symanteccodesigningcertificate"></a><span data-ttu-id="340a4-103">SymantecCodeSigningCertificate aktualisieren</span><span class="sxs-lookup"><span data-stu-id="340a4-103">Update symantecCodeSigningCertificate</span></span>

> <span data-ttu-id="340a4-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="340a4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="340a4-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="340a4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="340a4-106">Aktualisieren der Eigenschaften eines [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="340a4-106">Update the properties of a [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="340a4-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="340a4-107">Prerequisites</span></span>
<span data-ttu-id="340a4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="340a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="340a4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="340a4-110">Permission type</span></span>|<span data-ttu-id="340a4-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="340a4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="340a4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="340a4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="340a4-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="340a4-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="340a4-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="340a4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="340a4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="340a4-115">Not supported.</span></span>|
|<span data-ttu-id="340a4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="340a4-116">Application</span></span>|<span data-ttu-id="340a4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="340a4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="340a4-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="340a4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/symantecCodeSigningCertificate
```

## <a name="request-headers"></a><span data-ttu-id="340a4-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="340a4-119">Request headers</span></span>
|<span data-ttu-id="340a4-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="340a4-120">Header</span></span>|<span data-ttu-id="340a4-121">Wert</span><span class="sxs-lookup"><span data-stu-id="340a4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="340a4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="340a4-122">Authorization</span></span>|<span data-ttu-id="340a4-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="340a4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="340a4-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="340a4-124">Accept</span></span>|<span data-ttu-id="340a4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="340a4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="340a4-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="340a4-126">Request body</span></span>
<span data-ttu-id="340a4-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="340a4-127">In the request body, supply a JSON representation for the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

<span data-ttu-id="340a4-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="340a4-128">The following table shows the properties that are required when you create the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md).</span></span>

|<span data-ttu-id="340a4-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="340a4-129">Property</span></span>|<span data-ttu-id="340a4-130">Typ</span><span class="sxs-lookup"><span data-stu-id="340a4-130">Type</span></span>|<span data-ttu-id="340a4-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="340a4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="340a4-132">id</span><span class="sxs-lookup"><span data-stu-id="340a4-132">id</span></span>|<span data-ttu-id="340a4-133">String</span><span class="sxs-lookup"><span data-stu-id="340a4-133">String</span></span>|<span data-ttu-id="340a4-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="340a4-134">The key of the entity.</span></span>|
|<span data-ttu-id="340a4-135">content</span><span class="sxs-lookup"><span data-stu-id="340a4-135">content</span></span>|<span data-ttu-id="340a4-136">Binär</span><span class="sxs-lookup"><span data-stu-id="340a4-136">Binary</span></span>|<span data-ttu-id="340a4-137">Das Windows Symantec Code Signing Certificate im RAW-Datenformat.</span><span class="sxs-lookup"><span data-stu-id="340a4-137">The Windows Symantec Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="340a4-138">status</span><span class="sxs-lookup"><span data-stu-id="340a4-138">status</span></span>|[<span data-ttu-id="340a4-139">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="340a4-139">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="340a4-140">Der CERT-Status, der für die Einrichtung oder nicht-Einrichtung vorgesehen ist.</span><span class="sxs-lookup"><span data-stu-id="340a4-140">The Cert Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="340a4-141">Mögliche Werte sind: `notProvisioned` und `provisioned`.</span><span class="sxs-lookup"><span data-stu-id="340a4-141">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="340a4-142">password</span><span class="sxs-lookup"><span data-stu-id="340a4-142">password</span></span>|<span data-ttu-id="340a4-143">String</span><span class="sxs-lookup"><span data-stu-id="340a4-143">String</span></span>|<span data-ttu-id="340a4-144">Das für die PFX-Datei erforderliche Kennwort.</span><span class="sxs-lookup"><span data-stu-id="340a4-144">The Password required for .pfx file.</span></span>|
|<span data-ttu-id="340a4-145">subjectName</span><span class="sxs-lookup"><span data-stu-id="340a4-145">subjectName</span></span>|<span data-ttu-id="340a4-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="340a4-146">String</span></span>|<span data-ttu-id="340a4-147">Der AntragsTeller Name für das Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="340a4-147">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="340a4-148">subject</span><span class="sxs-lookup"><span data-stu-id="340a4-148">subject</span></span>|<span data-ttu-id="340a4-149">String</span><span class="sxs-lookup"><span data-stu-id="340a4-149">String</span></span>|<span data-ttu-id="340a4-150">Der Subject-Wert für das Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="340a4-150">The Subject value for the cert.</span></span>|
|<span data-ttu-id="340a4-151">issuerName</span><span class="sxs-lookup"><span data-stu-id="340a4-151">issuerName</span></span>|<span data-ttu-id="340a4-152">String</span><span class="sxs-lookup"><span data-stu-id="340a4-152">String</span></span>|<span data-ttu-id="340a4-153">Der Aussteller Name für das Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="340a4-153">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="340a4-154">Aussteller</span><span class="sxs-lookup"><span data-stu-id="340a4-154">issuer</span></span>|<span data-ttu-id="340a4-155">String</span><span class="sxs-lookup"><span data-stu-id="340a4-155">String</span></span>|<span data-ttu-id="340a4-156">Der Aussteller Wert für das Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="340a4-156">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="340a4-157">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="340a4-157">expirationDateTime</span></span>|<span data-ttu-id="340a4-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="340a4-158">DateTimeOffset</span></span>|<span data-ttu-id="340a4-159">Das Ablaufdatum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="340a4-159">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="340a4-160">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="340a4-160">uploadDateTime</span></span>|<span data-ttu-id="340a4-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="340a4-161">DateTimeOffset</span></span>|<span data-ttu-id="340a4-162">Der Typ des deSign Zertifikats als Symantec cert.</span><span class="sxs-lookup"><span data-stu-id="340a4-162">The Type of the CodeSigning Cert as Symantec Cert.</span></span>|



## <a name="response"></a><span data-ttu-id="340a4-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="340a4-163">Response</span></span>
<span data-ttu-id="340a4-164">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="340a4-164">If successful, this method returns a `200 OK` response code and an updated [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="340a4-165">Beispiel</span><span class="sxs-lookup"><span data-stu-id="340a4-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="340a4-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="340a4-166">Request</span></span>
<span data-ttu-id="340a4-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="340a4-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/symantecCodeSigningCertificate
Content-type: application/json
Content-length: 421

{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
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

### <a name="response"></a><span data-ttu-id="340a4-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="340a4-168">Response</span></span>
<span data-ttu-id="340a4-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="340a4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




