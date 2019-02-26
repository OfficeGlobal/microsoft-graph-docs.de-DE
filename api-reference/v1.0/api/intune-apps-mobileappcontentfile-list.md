---
title: Auflisten von „mobileAppContentFile“
description: Diese Methode listet die Eigenschaften von Objekten des Typs mobileAppContentFile auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1e01fc28975f5f72cd51ec64fe79857112d6f79f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261278"
---
# <a name="list-mobileappcontentfiles"></a><span data-ttu-id="a2371-103">Auflisten von „mobileAppContentFile“</span><span class="sxs-lookup"><span data-stu-id="a2371-103">List mobileAppContentFiles</span></span>

> <span data-ttu-id="a2371-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a2371-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2371-105">Diese Methode listet die Eigenschaften von Objekten des Typs [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) auf.</span><span class="sxs-lookup"><span data-stu-id="a2371-105">List properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2371-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a2371-106">Prerequisites</span></span>
<span data-ttu-id="a2371-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a2371-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a2371-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a2371-109">Permission type</span></span>|<span data-ttu-id="a2371-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a2371-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2371-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a2371-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a2371-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2371-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a2371-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a2371-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2371-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a2371-114">Not supported.</span></span>|
|<span data-ttu-id="a2371-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a2371-115">Application</span></span>|<span data-ttu-id="a2371-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a2371-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2371-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2371-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="a2371-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a2371-118">Request headers</span></span>
|<span data-ttu-id="a2371-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a2371-119">Header</span></span>|<span data-ttu-id="a2371-120">Wert</span><span class="sxs-lookup"><span data-stu-id="a2371-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2371-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2371-121">Authorization</span></span>|<span data-ttu-id="a2371-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a2371-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2371-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a2371-123">Accept</span></span>|<span data-ttu-id="a2371-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a2371-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2371-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a2371-125">Request body</span></span>
<span data-ttu-id="a2371-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a2371-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2371-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="a2371-127">Response</span></span>
<span data-ttu-id="a2371-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a2371-128">If successful, this method returns a `200 OK` response code and a collection of [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2371-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a2371-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2371-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2371-130">Request</span></span>
<span data-ttu-id="a2371-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a2371-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

### <a name="response"></a><span data-ttu-id="a2371-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="a2371-132">Response</span></span>
<span data-ttu-id="a2371-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a2371-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 527

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppContentFile",
      "azureStorageUri": "Azure Storage Uri value",
      "isCommitted": true,
      "id": "eab2e29b-e29b-eab2-9be2-b2ea9be2b2ea",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "name": "Name value",
      "size": 4,
      "sizeEncrypted": 13,
      "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
      "manifest": "bWFuaWZlc3Q=",
      "uploadState": "transientError"
    }
  ]
}
```



