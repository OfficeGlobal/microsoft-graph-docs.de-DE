---
title: EnterpriseCodeSigningCertificate aktualisieren
description: Aktualisieren Sie die Eigenschaften eines EnterpriseCodeSigningCertificate-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7541f75a12dc39dcf80dfcc0df06aef5d2c551a7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406577"
---
# <a name="update-enterprisecodesigningcertificate"></a><span data-ttu-id="89f01-103">EnterpriseCodeSigningCertificate aktualisieren</span><span class="sxs-lookup"><span data-stu-id="89f01-103">Update enterpriseCodeSigningCertificate</span></span>

> <span data-ttu-id="89f01-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="89f01-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="89f01-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="89f01-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="89f01-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="89f01-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89f01-107">Aktualisieren Sie die Eigenschaften eines [EnterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="89f01-107">Update the properties of a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89f01-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="89f01-108">Prerequisites</span></span>
<span data-ttu-id="89f01-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="89f01-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="89f01-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="89f01-111">Permission type</span></span>|<span data-ttu-id="89f01-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="89f01-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89f01-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="89f01-113">Delegated (work or school account)</span></span>|<span data-ttu-id="89f01-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89f01-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="89f01-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="89f01-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89f01-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="89f01-116">Not supported.</span></span>|
|<span data-ttu-id="89f01-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="89f01-117">Application</span></span>|<span data-ttu-id="89f01-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="89f01-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89f01-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="89f01-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="89f01-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="89f01-120">Request headers</span></span>
|<span data-ttu-id="89f01-121">Header</span><span class="sxs-lookup"><span data-stu-id="89f01-121">Header</span></span>|<span data-ttu-id="89f01-122">Wert</span><span class="sxs-lookup"><span data-stu-id="89f01-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89f01-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="89f01-123">Authorization</span></span>|<span data-ttu-id="89f01-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="89f01-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89f01-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="89f01-125">Accept</span></span>|<span data-ttu-id="89f01-126">application/json</span><span class="sxs-lookup"><span data-stu-id="89f01-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89f01-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="89f01-127">Request body</span></span>
<span data-ttu-id="89f01-128">Geben Sie im Textkörper Anforderung für das Objekt [EnterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="89f01-128">In the request body, supply a JSON representation for the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

<span data-ttu-id="89f01-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [EnterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="89f01-129">The following table shows the properties that are required when you create the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md).</span></span>

|<span data-ttu-id="89f01-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="89f01-130">Property</span></span>|<span data-ttu-id="89f01-131">Typ</span><span class="sxs-lookup"><span data-stu-id="89f01-131">Type</span></span>|<span data-ttu-id="89f01-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="89f01-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89f01-133">id</span><span class="sxs-lookup"><span data-stu-id="89f01-133">id</span></span>|<span data-ttu-id="89f01-134">String</span><span class="sxs-lookup"><span data-stu-id="89f01-134">String</span></span>|<span data-ttu-id="89f01-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="89f01-135">The key of the entity.</span></span>|
|<span data-ttu-id="89f01-136">content</span><span class="sxs-lookup"><span data-stu-id="89f01-136">content</span></span>|<span data-ttu-id="89f01-137">Binär</span><span class="sxs-lookup"><span data-stu-id="89f01-137">Binary</span></span>|<span data-ttu-id="89f01-138">Die Enterprise-Code für Windows-Signaturzertifikat im Format Rohdaten.</span><span class="sxs-lookup"><span data-stu-id="89f01-138">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="89f01-139">status</span><span class="sxs-lookup"><span data-stu-id="89f01-139">status</span></span>|[<span data-ttu-id="89f01-140">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="89f01-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="89f01-141">Status der bereitgestellt oder nicht bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="89f01-141">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="89f01-142">Mögliche Werte sind: `notProvisioned` und `provisioned`.</span><span class="sxs-lookup"><span data-stu-id="89f01-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="89f01-143">subjectName</span><span class="sxs-lookup"><span data-stu-id="89f01-143">subjectName</span></span>|<span data-ttu-id="89f01-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="89f01-144">String</span></span>|<span data-ttu-id="89f01-145">Der Antragstellername für das Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="89f01-145">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="89f01-146">subject</span><span class="sxs-lookup"><span data-stu-id="89f01-146">subject</span></span>|<span data-ttu-id="89f01-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="89f01-147">String</span></span>|<span data-ttu-id="89f01-148">Der Wert der Betreff für das Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="89f01-148">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="89f01-149">issuerName</span><span class="sxs-lookup"><span data-stu-id="89f01-149">issuerName</span></span>|<span data-ttu-id="89f01-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="89f01-150">String</span></span>|<span data-ttu-id="89f01-151">Der Name der Aussteller für das Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="89f01-151">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="89f01-152">Aussteller</span><span class="sxs-lookup"><span data-stu-id="89f01-152">issuer</span></span>|<span data-ttu-id="89f01-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="89f01-153">String</span></span>|<span data-ttu-id="89f01-154">Der Wert der Aussteller für das Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="89f01-154">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="89f01-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="89f01-155">expirationDateTime</span></span>|<span data-ttu-id="89f01-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89f01-156">DateTimeOffset</span></span>|<span data-ttu-id="89f01-157">Das Ablaufdatum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="89f01-157">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="89f01-158">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="89f01-158">uploadDateTime</span></span>|<span data-ttu-id="89f01-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89f01-159">DateTimeOffset</span></span>|<span data-ttu-id="89f01-160">Das Datum-Uhrzeit des Zertifikats CodeSigning, wenn diese hochgeladen wird.</span><span class="sxs-lookup"><span data-stu-id="89f01-160">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="89f01-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="89f01-161">Response</span></span>
<span data-ttu-id="89f01-162">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [EnterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="89f01-162">If successful, this method returns a `200 OK` response code and an updated [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89f01-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="89f01-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="89f01-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="89f01-164">Request</span></span>
<span data-ttu-id="89f01-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="89f01-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="89f01-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="89f01-166">Response</span></span>
<span data-ttu-id="89f01-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="89f01-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




