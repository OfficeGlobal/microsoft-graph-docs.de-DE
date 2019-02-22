---
title: EnterpriseCodeSigningCertificates aufListen
description: AufListen von Eigenschaften und Beziehungen der enterpriseCodeSigningCertificate-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eac65068ede3c1b59b0a3baf56bfe739fb1d8d5d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162230"
---
# <a name="list-enterprisecodesigningcertificates"></a><span data-ttu-id="59e69-103">EnterpriseCodeSigningCertificates aufListen</span><span class="sxs-lookup"><span data-stu-id="59e69-103">List enterpriseCodeSigningCertificates</span></span>

> <span data-ttu-id="59e69-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="59e69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59e69-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="59e69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59e69-106">AufListen von Eigenschaften und Beziehungen der [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="59e69-106">List properties and relationships of the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59e69-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="59e69-107">Prerequisites</span></span>
<span data-ttu-id="59e69-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="59e69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="59e69-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="59e69-110">Permission type</span></span>|<span data-ttu-id="59e69-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="59e69-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59e69-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="59e69-112">Delegated (work or school account)</span></span>|<span data-ttu-id="59e69-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="59e69-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="59e69-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="59e69-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59e69-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="59e69-115">Not supported.</span></span>|
|<span data-ttu-id="59e69-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="59e69-116">Application</span></span>|<span data-ttu-id="59e69-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="59e69-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="59e69-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="59e69-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/enterpriseCodeSigningCertificates
```

## <a name="request-headers"></a><span data-ttu-id="59e69-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="59e69-119">Request headers</span></span>
|<span data-ttu-id="59e69-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="59e69-120">Header</span></span>|<span data-ttu-id="59e69-121">Wert</span><span class="sxs-lookup"><span data-stu-id="59e69-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59e69-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="59e69-122">Authorization</span></span>|<span data-ttu-id="59e69-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="59e69-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59e69-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="59e69-124">Accept</span></span>|<span data-ttu-id="59e69-125">application/json</span><span class="sxs-lookup"><span data-stu-id="59e69-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59e69-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="59e69-126">Request body</span></span>
<span data-ttu-id="59e69-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="59e69-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59e69-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="59e69-128">Response</span></span>
<span data-ttu-id="59e69-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="59e69-129">If successful, this method returns a `200 OK` response code and a collection of [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59e69-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="59e69-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="59e69-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="59e69-131">Request</span></span>
<span data-ttu-id="59e69-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="59e69-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates
```

### <a name="response"></a><span data-ttu-id="59e69-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="59e69-133">Response</span></span>
<span data-ttu-id="59e69-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="59e69-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 512

{
  "value": [
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
  ]
}
```




