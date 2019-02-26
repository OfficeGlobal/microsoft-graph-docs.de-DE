---
title: iosCertificateProfile abrufen
description: Lesen von Eigenschaften und Beziehungen des iosCertificateProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4336672393415becc0d4b4ff46a05b5bef9f0fa9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174510"
---
# <a name="get-ioscertificateprofile"></a><span data-ttu-id="a72e8-103">iosCertificateProfile abrufen</span><span class="sxs-lookup"><span data-stu-id="a72e8-103">Get iosCertificateProfile</span></span>

> <span data-ttu-id="a72e8-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a72e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a72e8-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a72e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a72e8-106">Lesen von Eigenschaften und Beziehungen des [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a72e8-106">Read properties and relationships of the [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a72e8-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a72e8-107">Prerequisites</span></span>
<span data-ttu-id="a72e8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a72e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a72e8-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a72e8-110">Permission type</span></span>|<span data-ttu-id="a72e8-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a72e8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a72e8-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a72e8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a72e8-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a72e8-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a72e8-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a72e8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a72e8-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a72e8-115">Not supported.</span></span>|
|<span data-ttu-id="a72e8-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a72e8-116">Application</span></span>|<span data-ttu-id="a72e8-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a72e8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a72e8-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a72e8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/smimeSigningCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/smimeEncryptionCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a72e8-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a72e8-119">Optional query parameters</span></span>
<span data-ttu-id="a72e8-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a72e8-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a72e8-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a72e8-121">Request headers</span></span>
|<span data-ttu-id="a72e8-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a72e8-122">Header</span></span>|<span data-ttu-id="a72e8-123">Wert</span><span class="sxs-lookup"><span data-stu-id="a72e8-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a72e8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a72e8-124">Authorization</span></span>|<span data-ttu-id="a72e8-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a72e8-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a72e8-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a72e8-126">Accept</span></span>|<span data-ttu-id="a72e8-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a72e8-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a72e8-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a72e8-128">Request body</span></span>
<span data-ttu-id="a72e8-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a72e8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a72e8-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="a72e8-130">Response</span></span>
<span data-ttu-id="a72e8-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a72e8-131">If successful, this method returns a `200 OK` response code and [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a72e8-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a72e8-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a72e8-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a72e8-133">Request</span></span>
<span data-ttu-id="a72e8-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a72e8-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/smimeSigningCertificate
```

### <a name="response"></a><span data-ttu-id="a72e8-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="a72e8-135">Response</span></span>
<span data-ttu-id="a72e8-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a72e8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 464

{
  "value": {
    "@odata.type": "#microsoft.graph.iosCertificateProfile",
    "id": "0ea4f39a-f39a-0ea4-9af3-a40e9af3a40e",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7
  }
}
```




