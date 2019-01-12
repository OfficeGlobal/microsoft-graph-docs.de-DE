---
title: EnterpriseCodeSigningCertificate aktualisieren
description: Aktualisieren Sie die Eigenschaften eines EnterpriseCodeSigningCertificate-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5133f5dffa98834ce44849c6b18c73cc19732756
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955114"
---
# <a name="update-enterprisecodesigningcertificate"></a><span data-ttu-id="8364c-103">EnterpriseCodeSigningCertificate aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8364c-103">Update enterpriseCodeSigningCertificate</span></span>

> <span data-ttu-id="8364c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8364c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8364c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8364c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8364c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8364c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8364c-107">Aktualisieren Sie die Eigenschaften eines [EnterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="8364c-107">Update the properties of a [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8364c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8364c-108">Prerequisites</span></span>
<span data-ttu-id="8364c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8364c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8364c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8364c-111">Permission type</span></span>|<span data-ttu-id="8364c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8364c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8364c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8364c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8364c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8364c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8364c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8364c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8364c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8364c-116">Not supported.</span></span>|
|<span data-ttu-id="8364c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8364c-117">Application</span></span>|<span data-ttu-id="8364c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8364c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8364c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8364c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="8364c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8364c-120">Request headers</span></span>
|<span data-ttu-id="8364c-121">Header</span><span class="sxs-lookup"><span data-stu-id="8364c-121">Header</span></span>|<span data-ttu-id="8364c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8364c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8364c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8364c-123">Authorization</span></span>|<span data-ttu-id="8364c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8364c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8364c-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8364c-125">Accept</span></span>|<span data-ttu-id="8364c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8364c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8364c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8364c-127">Request body</span></span>
<span data-ttu-id="8364c-128">Geben Sie im Textkörper Anforderung für das Objekt [EnterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="8364c-128">In the request body, supply a JSON representation for the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

<span data-ttu-id="8364c-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [EnterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="8364c-129">The following table shows the properties that are required when you create the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md).</span></span>

|<span data-ttu-id="8364c-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8364c-130">Property</span></span>|<span data-ttu-id="8364c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="8364c-131">Type</span></span>|<span data-ttu-id="8364c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8364c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8364c-133">id</span><span class="sxs-lookup"><span data-stu-id="8364c-133">id</span></span>|<span data-ttu-id="8364c-134">String</span><span class="sxs-lookup"><span data-stu-id="8364c-134">String</span></span>|<span data-ttu-id="8364c-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8364c-135">The key of the entity.</span></span>|
|<span data-ttu-id="8364c-136">content</span><span class="sxs-lookup"><span data-stu-id="8364c-136">content</span></span>|<span data-ttu-id="8364c-137">Binär</span><span class="sxs-lookup"><span data-stu-id="8364c-137">Binary</span></span>|<span data-ttu-id="8364c-138">Die Enterprise-Code für Windows-Signaturzertifikat im Format Rohdaten.</span><span class="sxs-lookup"><span data-stu-id="8364c-138">The Windows Enterprise Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="8364c-139">status</span><span class="sxs-lookup"><span data-stu-id="8364c-139">status</span></span>|[<span data-ttu-id="8364c-140">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="8364c-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="8364c-141">Status der bereitgestellt oder nicht bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="8364c-141">The Certificate Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="8364c-142">Mögliche Werte sind: `notProvisioned` und `provisioned`.</span><span class="sxs-lookup"><span data-stu-id="8364c-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="8364c-143">subjectName</span><span class="sxs-lookup"><span data-stu-id="8364c-143">subjectName</span></span>|<span data-ttu-id="8364c-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8364c-144">String</span></span>|<span data-ttu-id="8364c-145">Der Antragstellername für das Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="8364c-145">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="8364c-146">Betreff</span><span class="sxs-lookup"><span data-stu-id="8364c-146">subject</span></span>|<span data-ttu-id="8364c-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8364c-147">String</span></span>|<span data-ttu-id="8364c-148">Der Wert der Betreff für das Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="8364c-148">The Subject Value for the cert.</span></span>|
|<span data-ttu-id="8364c-149">issuerName</span><span class="sxs-lookup"><span data-stu-id="8364c-149">issuerName</span></span>|<span data-ttu-id="8364c-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8364c-150">String</span></span>|<span data-ttu-id="8364c-151">Der Name der Aussteller für das Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="8364c-151">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="8364c-152">Aussteller</span><span class="sxs-lookup"><span data-stu-id="8364c-152">issuer</span></span>|<span data-ttu-id="8364c-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8364c-153">String</span></span>|<span data-ttu-id="8364c-154">Der Wert der Aussteller für das Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="8364c-154">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="8364c-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8364c-155">expirationDateTime</span></span>|<span data-ttu-id="8364c-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8364c-156">DateTimeOffset</span></span>|<span data-ttu-id="8364c-157">Das Ablaufdatum des Zertifikats.</span><span class="sxs-lookup"><span data-stu-id="8364c-157">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="8364c-158">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="8364c-158">uploadDateTime</span></span>|<span data-ttu-id="8364c-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8364c-159">DateTimeOffset</span></span>|<span data-ttu-id="8364c-160">Das Datum-Uhrzeit des Zertifikats CodeSigning, wenn diese hochgeladen wird.</span><span class="sxs-lookup"><span data-stu-id="8364c-160">The date time of CodeSigning Cert when it is uploaded.</span></span>|



## <a name="response"></a><span data-ttu-id="8364c-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="8364c-161">Response</span></span>
<span data-ttu-id="8364c-162">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [EnterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="8364c-162">If successful, this method returns a `200 OK` response code and an updated [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8364c-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8364c-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="8364c-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8364c-164">Request</span></span>
<span data-ttu-id="8364c-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8364c-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
Content-type: application/json
Content-length: 319

{
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

### <a name="response"></a><span data-ttu-id="8364c-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="8364c-166">Response</span></span>
<span data-ttu-id="8364c-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8364c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





