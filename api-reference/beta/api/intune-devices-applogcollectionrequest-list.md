---
title: Liste appLogCollectionRequests
description: Listeneigenschaften und Beziehungen der AppLogCollectionRequest-Objekte.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f5cab95b3a7c4315e1d895e8dcc73c1f0cfc0278
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430163"
---
# <a name="list-applogcollectionrequests"></a><span data-ttu-id="985a4-103">Liste appLogCollectionRequests</span><span class="sxs-lookup"><span data-stu-id="985a4-103">List appLogCollectionRequests</span></span>

> <span data-ttu-id="985a4-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="985a4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="985a4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="985a4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="985a4-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="985a4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="985a4-107">Listeneigenschaften und Beziehungen der [AppLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="985a4-107">List properties and relationships of the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="985a4-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="985a4-108">Prerequisites</span></span>
<span data-ttu-id="985a4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="985a4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="985a4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="985a4-111">Permission type</span></span>|<span data-ttu-id="985a4-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="985a4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="985a4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="985a4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="985a4-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="985a4-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="985a4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="985a4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="985a4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="985a4-116">Not supported.</span></span>|
|<span data-ttu-id="985a4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="985a4-117">Application</span></span>|<span data-ttu-id="985a4-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="985a4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="985a4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="985a4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
```

## <a name="request-headers"></a><span data-ttu-id="985a4-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="985a4-120">Request headers</span></span>
|<span data-ttu-id="985a4-121">Header</span><span class="sxs-lookup"><span data-stu-id="985a4-121">Header</span></span>|<span data-ttu-id="985a4-122">Wert</span><span class="sxs-lookup"><span data-stu-id="985a4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="985a4-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="985a4-123">Authorization</span></span>|<span data-ttu-id="985a4-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="985a4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="985a4-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="985a4-125">Accept</span></span>|<span data-ttu-id="985a4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="985a4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="985a4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="985a4-127">Request body</span></span>
<span data-ttu-id="985a4-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="985a4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="985a4-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="985a4-129">Response</span></span>
<span data-ttu-id="985a4-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [AppLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="985a4-130">If successful, this method returns a `200 OK` response code and a collection of [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="985a4-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="985a4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="985a4-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="985a4-132">Request</span></span>
<span data-ttu-id="985a4-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="985a4-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
```

### <a name="response"></a><span data-ttu-id="985a4-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="985a4-134">Response</span></span>
<span data-ttu-id="985a4-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="985a4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 371

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.appLogCollectionRequest",
      "id": "cca685ff-85ff-cca6-ff85-a6ccff85a6cc",
      "status": "completed",
      "errorMessage": "Error Message value",
      "customLogFolders": [
        "Custom Log Folders value"
      ],
      "completedDateTime": "2016-12-31T23:58:52.3534526-08:00"
    }
  ]
}
```




