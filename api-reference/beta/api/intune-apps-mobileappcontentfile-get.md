---
title: mobileAppContentFile abrufen
description: Lesen von Eigenschaften und Beziehungen des mobileAppContentFile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9c6e08c38f49e8db7217d81434c900bc9734c979
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145654"
---
# <a name="get-mobileappcontentfile"></a><span data-ttu-id="a70cd-103">mobileAppContentFile abrufen</span><span class="sxs-lookup"><span data-stu-id="a70cd-103">Get mobileAppContentFile</span></span>

> <span data-ttu-id="a70cd-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a70cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a70cd-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a70cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a70cd-106">Lesen von Eigenschaften und Beziehungen des [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a70cd-106">Read properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a70cd-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a70cd-107">Prerequisites</span></span>
<span data-ttu-id="a70cd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a70cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a70cd-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a70cd-110">Permission type</span></span>|<span data-ttu-id="a70cd-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a70cd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a70cd-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a70cd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a70cd-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a70cd-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a70cd-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a70cd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a70cd-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a70cd-115">Not supported.</span></span>|
|<span data-ttu-id="a70cd-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a70cd-116">Application</span></span>|<span data-ttu-id="a70cd-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a70cd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a70cd-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a70cd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a70cd-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a70cd-119">Optional query parameters</span></span>
<span data-ttu-id="a70cd-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a70cd-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a70cd-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a70cd-121">Request headers</span></span>
|<span data-ttu-id="a70cd-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a70cd-122">Header</span></span>|<span data-ttu-id="a70cd-123">Wert</span><span class="sxs-lookup"><span data-stu-id="a70cd-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a70cd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a70cd-124">Authorization</span></span>|<span data-ttu-id="a70cd-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a70cd-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a70cd-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a70cd-126">Accept</span></span>|<span data-ttu-id="a70cd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a70cd-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a70cd-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a70cd-128">Request body</span></span>
<span data-ttu-id="a70cd-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a70cd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a70cd-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="a70cd-130">Response</span></span>
<span data-ttu-id="a70cd-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a70cd-131">If successful, this method returns a `200 OK` response code and [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a70cd-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a70cd-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a70cd-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a70cd-133">Request</span></span>
<span data-ttu-id="a70cd-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a70cd-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

### <a name="response"></a><span data-ttu-id="a70cd-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="a70cd-135">Response</span></span>
<span data-ttu-id="a70cd-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a70cd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 548

{
  "value": {
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
    "uploadState": "transientError",
    "isFrameworkFile": true,
    "isDependency": true
  }
}
```




