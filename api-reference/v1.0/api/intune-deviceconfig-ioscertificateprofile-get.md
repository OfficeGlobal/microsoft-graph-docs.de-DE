---
title: iosCertificateProfile abrufen
description: Lesen von Eigenschaften und Beziehungen des iosCertificateProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f4cf567d8dbc9d7961536b676a1e8388a355337
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30985718"
---
# <a name="get-ioscertificateprofile"></a><span data-ttu-id="81fe8-103">iosCertificateProfile abrufen</span><span class="sxs-lookup"><span data-stu-id="81fe8-103">Get iosCertificateProfile</span></span>

> <span data-ttu-id="81fe8-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="81fe8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81fe8-105">Lesen von Eigenschaften und Beziehungen des [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="81fe8-105">Read properties and relationships of the [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81fe8-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="81fe8-106">Prerequisites</span></span>
<span data-ttu-id="81fe8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81fe8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81fe8-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="81fe8-109">Permission type</span></span>|<span data-ttu-id="81fe8-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="81fe8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81fe8-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="81fe8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="81fe8-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="81fe8-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="81fe8-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="81fe8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81fe8-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="81fe8-114">Not supported.</span></span>|
|<span data-ttu-id="81fe8-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="81fe8-115">Application</span></span>|<span data-ttu-id="81fe8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="81fe8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81fe8-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="81fe8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="81fe8-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="81fe8-118">Optional query parameters</span></span>
<span data-ttu-id="81fe8-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="81fe8-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="81fe8-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="81fe8-120">Request headers</span></span>
|<span data-ttu-id="81fe8-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="81fe8-121">Header</span></span>|<span data-ttu-id="81fe8-122">Wert</span><span class="sxs-lookup"><span data-stu-id="81fe8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81fe8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="81fe8-123">Authorization</span></span>|<span data-ttu-id="81fe8-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="81fe8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81fe8-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="81fe8-125">Accept</span></span>|<span data-ttu-id="81fe8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="81fe8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81fe8-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="81fe8-127">Request body</span></span>
<span data-ttu-id="81fe8-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="81fe8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81fe8-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="81fe8-129">Response</span></span>
<span data-ttu-id="81fe8-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="81fe8-130">If successful, this method returns a `200 OK` response code and [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81fe8-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="81fe8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="81fe8-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="81fe8-132">Request</span></span>
<span data-ttu-id="81fe8-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="81fe8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="81fe8-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="81fe8-134">Response</span></span>
<span data-ttu-id="81fe8-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="81fe8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 364

{
  "value": {
    "@odata.type": "#microsoft.graph.iosCertificateProfile",
    "id": "0ea4f39a-f39a-0ea4-9af3-a40e9af3a40e",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7
  }
}
```



