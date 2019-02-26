---
title: createDownloadUrl-Aktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1ed7e111dc99e3db3f44accdbaaee9b205e8c5ae
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164120"
---
# <a name="createdownloadurl-action"></a><span data-ttu-id="daf7e-103">createDownloadUrl-Aktion</span><span class="sxs-lookup"><span data-stu-id="daf7e-103">createDownloadUrl action</span></span>

> <span data-ttu-id="daf7e-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="daf7e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="daf7e-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="daf7e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="daf7e-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="daf7e-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="daf7e-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="daf7e-107">Prerequisites</span></span>
<span data-ttu-id="daf7e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="daf7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="daf7e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="daf7e-110">Permission type</span></span>|<span data-ttu-id="daf7e-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="daf7e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="daf7e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="daf7e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="daf7e-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="daf7e-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="daf7e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="daf7e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="daf7e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="daf7e-115">Not supported.</span></span>|
|<span data-ttu-id="daf7e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="daf7e-116">Application</span></span>|<span data-ttu-id="daf7e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="daf7e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="daf7e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="daf7e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}/createDownloadUrl
```

## <a name="request-headers"></a><span data-ttu-id="daf7e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="daf7e-119">Request headers</span></span>
|<span data-ttu-id="daf7e-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="daf7e-120">Header</span></span>|<span data-ttu-id="daf7e-121">Wert</span><span class="sxs-lookup"><span data-stu-id="daf7e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="daf7e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="daf7e-122">Authorization</span></span>|<span data-ttu-id="daf7e-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="daf7e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="daf7e-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="daf7e-124">Accept</span></span>|<span data-ttu-id="daf7e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="daf7e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="daf7e-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="daf7e-126">Request body</span></span>
<span data-ttu-id="daf7e-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="daf7e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="daf7e-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="daf7e-128">Response</span></span>
<span data-ttu-id="daf7e-129">Bei erfolgreicher Ausführung gibt die Aktion den `200 OK` Antwortcode und eine [appLogCollectionDownloadDetails](../resources/intune-devices-applogcollectiondownloaddetails.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="daf7e-129">If successful, this action returns a `200 OK` response code and a [appLogCollectionDownloadDetails](../resources/intune-devices-applogcollectiondownloaddetails.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="daf7e-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="daf7e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="daf7e-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="daf7e-131">Request</span></span>
<span data-ttu-id="daf7e-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="daf7e-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}/createDownloadUrl
```

### <a name="response"></a><span data-ttu-id="daf7e-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="daf7e-133">Response</span></span>
<span data-ttu-id="daf7e-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="daf7e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 239

{
  "value": {
    "@odata.type": "microsoft.graph.appLogCollectionDownloadDetails",
    "downloadUrl": "https://example.com/downloadUrl/",
    "decryptionKey": "Decryption Key value",
    "appLogDecryptionAlgorithm": "aes256"
  }
}
```




