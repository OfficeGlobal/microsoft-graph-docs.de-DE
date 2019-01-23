---
title: Abrufen von symantecCodeSigningCertificate
description: Lesen Sie Eigenschaften und Beziehungen des SymantecCodeSigningCertificate-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f9975639c05f7432030b229ac85b04a48f7ed149
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394950"
---
# <a name="get-symanteccodesigningcertificate"></a><span data-ttu-id="a44f8-103">Abrufen von symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="a44f8-103">Get symantecCodeSigningCertificate</span></span>

> <span data-ttu-id="a44f8-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="a44f8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a44f8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a44f8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a44f8-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a44f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a44f8-107">Lesen Sie Eigenschaften und Beziehungen des [SymantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="a44f8-107">Read properties and relationships of the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a44f8-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a44f8-108">Prerequisites</span></span>
<span data-ttu-id="a44f8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a44f8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a44f8-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a44f8-111">Permission type</span></span>|<span data-ttu-id="a44f8-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a44f8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a44f8-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a44f8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a44f8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a44f8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a44f8-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a44f8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a44f8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a44f8-116">Not supported.</span></span>|
|<span data-ttu-id="a44f8-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a44f8-117">Application</span></span>|<span data-ttu-id="a44f8-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a44f8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a44f8-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a44f8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/symantecCodeSigningCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a44f8-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a44f8-120">Optional query parameters</span></span>
<span data-ttu-id="a44f8-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a44f8-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a44f8-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a44f8-122">Request headers</span></span>
|<span data-ttu-id="a44f8-123">Header</span><span class="sxs-lookup"><span data-stu-id="a44f8-123">Header</span></span>|<span data-ttu-id="a44f8-124">Wert</span><span class="sxs-lookup"><span data-stu-id="a44f8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a44f8-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a44f8-125">Authorization</span></span>|<span data-ttu-id="a44f8-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a44f8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a44f8-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a44f8-127">Accept</span></span>|<span data-ttu-id="a44f8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a44f8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a44f8-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a44f8-129">Request body</span></span>
<span data-ttu-id="a44f8-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a44f8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a44f8-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="a44f8-131">Response</span></span>
<span data-ttu-id="a44f8-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [SymantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="a44f8-132">If successful, this method returns a `200 OK` response code and [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a44f8-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a44f8-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a44f8-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a44f8-134">Request</span></span>
<span data-ttu-id="a44f8-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a44f8-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/symantecCodeSigningCertificate
```

### <a name="response"></a><span data-ttu-id="a44f8-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="a44f8-136">Response</span></span>
<span data-ttu-id="a44f8-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a44f8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 511

{
  "value": {
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
}
```




