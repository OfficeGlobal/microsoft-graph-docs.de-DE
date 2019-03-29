---
title: EnterpriseCodeSigningCertificate abrufen
description: Lesen von Eigenschaften und Beziehungen des enterpriseCodeSigningCertificate-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ed7779156aa18f86403a4e4e892da2e618d6e5ec
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974349"
---
# <a name="get-enterprisecodesigningcertificate"></a><span data-ttu-id="e3300-103">EnterpriseCodeSigningCertificate abrufen</span><span class="sxs-lookup"><span data-stu-id="e3300-103">Get enterpriseCodeSigningCertificate</span></span>

> <span data-ttu-id="e3300-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e3300-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3300-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e3300-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3300-106">Lesen von Eigenschaften und Beziehungen des [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="e3300-106">Read properties and relationships of the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3300-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e3300-107">Prerequisites</span></span>
<span data-ttu-id="e3300-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3300-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3300-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e3300-110">Permission type</span></span>|<span data-ttu-id="e3300-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e3300-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3300-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e3300-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e3300-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3300-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e3300-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e3300-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3300-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3300-115">Not supported.</span></span>|
|<span data-ttu-id="e3300-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e3300-116">Application</span></span>|<span data-ttu-id="e3300-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3300-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3300-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3300-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e3300-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e3300-119">Optional query parameters</span></span>
<span data-ttu-id="e3300-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e3300-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3300-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e3300-121">Request headers</span></span>
|<span data-ttu-id="e3300-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e3300-122">Header</span></span>|<span data-ttu-id="e3300-123">Wert</span><span class="sxs-lookup"><span data-stu-id="e3300-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3300-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3300-124">Authorization</span></span>|<span data-ttu-id="e3300-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e3300-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3300-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e3300-126">Accept</span></span>|<span data-ttu-id="e3300-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e3300-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3300-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e3300-128">Request body</span></span>
<span data-ttu-id="e3300-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e3300-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3300-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3300-130">Response</span></span>
<span data-ttu-id="e3300-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e3300-131">If successful, this method returns a `200 OK` response code and [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3300-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e3300-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3300-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3300-133">Request</span></span>
<span data-ttu-id="e3300-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e3300-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
```

### <a name="response"></a><span data-ttu-id="e3300-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3300-135">Response</span></span>
<span data-ttu-id="e3300-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e3300-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 478

{
  "value": {
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
}
```




