---
title: EnterpriseCodeSigningCertificate aktualisieren
description: Aktualisieren der Eigenschaften eines enterpriseCodeSigningCertificate-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3820c47b4aa87ecbeed4b5c6e5a5520e5126e3a1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957521"
---
# <a name="update-enterprisecodesigningcertificate"></a><span data-ttu-id="bd9f6-103">EnterpriseCodeSigningCertificate aktualisieren</span><span class="sxs-lookup"><span data-stu-id="bd9f6-103">Update enterpriseCodeSigningCertificate</span></span>

> <span data-ttu-id="bd9f6-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bd9f6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd9f6-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="bd9f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd9f6-106">Aktualisieren der Eigenschaften eines [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="bd9f6-106">Update the properties of a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd9f6-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bd9f6-107">Prerequisites</span></span>
<span data-ttu-id="bd9f6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd9f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd9f6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bd9f6-110">Permission type</span></span>|<span data-ttu-id="bd9f6-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bd9f6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd9f6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bd9f6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bd9f6-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd9f6-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bd9f6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bd9f6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd9f6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bd9f6-115">Not supported.</span></span>|
|<span data-ttu-id="bd9f6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bd9f6-116">Application</span></span>|<span data-ttu-id="bd9f6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bd9f6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd9f6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd9f6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="bd9f6-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bd9f6-119">Request headers</span></span>
|<span data-ttu-id="bd9f6-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bd9f6-120">Header</span></span>|<span data-ttu-id="bd9f6-121">Wert</span><span class="sxs-lookup"><span data-stu-id="bd9f6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd9f6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd9f6-122">Authorization</span></span>|<span data-ttu-id="bd9f6-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bd9f6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd9f6-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bd9f6-124">Accept</span></span>|<span data-ttu-id="bd9f6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bd9f6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd9f6-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bd9f6-126">Request body</span></span>
<span data-ttu-id="bd9f6-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="bd9f6-127">In the request body, supply a JSON representation for the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

<span data-ttu-id="bd9f6-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="bd9f6-128">The following table shows the properties that are required when you create the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md).</span></span>

|<span data-ttu-id="bd9f6-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bd9f6-129">Property</span></span>|<span data-ttu-id="bd9f6-130">Typ</span><span class="sxs-lookup"><span data-stu-id="bd9f6-130">Type</span></span>|<span data-ttu-id="bd9f6-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bd9f6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd9f6-132">id</span><span class="sxs-lookup"><span data-stu-id="bd9f6-132">id</span></span>|<span data-ttu-id="bd9f6-133">String</span><span class="sxs-lookup"><span data-stu-id="bd9f6-133">String</span></span>|<span data-ttu-id="bd9f6-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="bd9f6-134">The key of the entity.</span></span>|
|<span data-ttu-id="bd9f6-135">content</span><span class="sxs-lookup"><span data-stu-id="bd9f6-135">content</span></span>|<span data-ttu-id="bd9f6-136">Binär</span><span class="sxs-lookup"><span data-stu-id="bd9f6-136">Binary</span></span>|<span data-ttu-id="bd9f6-137">Das Windows Enterprise-Code SignierungsZertifikat im RAW-Datenformat.</span><span class="sxs-lookup"><span data-stu-id="bd9f6-137">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="bd9f6-138">status</span><span class="sxs-lookup"><span data-stu-id="bd9f6-138">status</span></span>|[<span data-ttu-id="bd9f6-139">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="bd9f6-139">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="bd9f6-140">Der Zertifikat Status, der für die Einrichtung oder nicht-Einrichtung vorgesehen ist.</span><span class="sxs-lookup"><span data-stu-id="bd9f6-140">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="bd9f6-141">Mögliche Werte sind: `notProvisioned` und `provisioned`.</span><span class="sxs-lookup"><span data-stu-id="bd9f6-141">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="bd9f6-142">subjectName</span><span class="sxs-lookup"><span data-stu-id="bd9f6-142">subjectName</span></span>|<span data-ttu-id="bd9f6-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bd9f6-143">String</span></span>|<span data-ttu-id="bd9f6-144">Der AntragsTeller Name für das Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="bd9f6-144">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="bd9f6-145">subject</span><span class="sxs-lookup"><span data-stu-id="bd9f6-145">subject</span></span>|<span data-ttu-id="bd9f6-146">String</span><span class="sxs-lookup"><span data-stu-id="bd9f6-146">String</span></span>|<span data-ttu-id="bd9f6-147">Der Subject-Wert für das Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="bd9f6-147">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="bd9f6-148">issuerName</span><span class="sxs-lookup"><span data-stu-id="bd9f6-148">issuerName</span></span>|<span data-ttu-id="bd9f6-149">String</span><span class="sxs-lookup"><span data-stu-id="bd9f6-149">String</span></span>|<span data-ttu-id="bd9f6-150">Der Aussteller Name für das Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="bd9f6-150">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="bd9f6-151">Aussteller</span><span class="sxs-lookup"><span data-stu-id="bd9f6-151">issuer</span></span>|<span data-ttu-id="bd9f6-152">String</span><span class="sxs-lookup"><span data-stu-id="bd9f6-152">String</span></span>|<span data-ttu-id="bd9f6-153">Der Aussteller Wert für das Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="bd9f6-153">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="bd9f6-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bd9f6-154">expirationDateTime</span></span>|<span data-ttu-id="bd9f6-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd9f6-155">DateTimeOffset</span></span>|<span data-ttu-id="bd9f6-156">Das Ablaufdatum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="bd9f6-156">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="bd9f6-157">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="bd9f6-157">uploadDateTime</span></span>|<span data-ttu-id="bd9f6-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd9f6-158">DateTimeOffset</span></span>|<span data-ttu-id="bd9f6-159">Die Datum-Uhrzeit der mitGestaltung von CERT beim Hochladen.</span><span class="sxs-lookup"><span data-stu-id="bd9f6-159">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="bd9f6-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd9f6-160">Response</span></span>
<span data-ttu-id="bd9f6-161">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bd9f6-161">If successful, this method returns a `200 OK` response code and an updated [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd9f6-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bd9f6-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd9f6-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd9f6-163">Request</span></span>
<span data-ttu-id="bd9f6-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bd9f6-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
Content-type: application/json
Content-length: 390

{
  "@odata.type": "#microsoft.graph.enterpriseCodeSigningCertificate",
  "content": "Y29udGVudA==",
  "status": "provisioned",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
}
```

### <a name="response"></a><span data-ttu-id="bd9f6-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd9f6-165">Response</span></span>
<span data-ttu-id="bd9f6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bd9f6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 439

{
  "@odata.type": "#microsoft.graph.enterpriseCodeSigningCertificate",
  "id": "b20d3703-3703-b20d-0337-0db203370db2",
  "content": "Y29udGVudA==",
  "status": "provisioned",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
}
```




