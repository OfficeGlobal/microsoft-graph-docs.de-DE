---
title: MobileAppInstallStatuses aufListen
description: AufListen von Eigenschaften und Beziehungen der mobileAppInstallStatus-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5153b022e6a15a4faa26fe70bb411cd2a17a4d62
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962260"
---
# <a name="list-mobileappinstallstatuses"></a><span data-ttu-id="6fbcc-103">MobileAppInstallStatuses aufListen</span><span class="sxs-lookup"><span data-stu-id="6fbcc-103">List mobileAppInstallStatuses</span></span>

> <span data-ttu-id="6fbcc-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6fbcc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6fbcc-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6fbcc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fbcc-106">AufListen von Eigenschaften und Beziehungen der [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="6fbcc-106">List properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6fbcc-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6fbcc-107">Prerequisites</span></span>
<span data-ttu-id="6fbcc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fbcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fbcc-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6fbcc-110">Permission type</span></span>|<span data-ttu-id="6fbcc-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6fbcc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6fbcc-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6fbcc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6fbcc-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6fbcc-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6fbcc-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6fbcc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fbcc-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6fbcc-115">Not supported.</span></span>|
|<span data-ttu-id="6fbcc-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6fbcc-116">Application</span></span>|<span data-ttu-id="6fbcc-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6fbcc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6fbcc-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6fbcc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="6fbcc-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6fbcc-119">Request headers</span></span>
|<span data-ttu-id="6fbcc-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6fbcc-120">Header</span></span>|<span data-ttu-id="6fbcc-121">Wert</span><span class="sxs-lookup"><span data-stu-id="6fbcc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6fbcc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fbcc-122">Authorization</span></span>|<span data-ttu-id="6fbcc-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6fbcc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6fbcc-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6fbcc-124">Accept</span></span>|<span data-ttu-id="6fbcc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6fbcc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fbcc-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6fbcc-126">Request body</span></span>
<span data-ttu-id="6fbcc-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6fbcc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fbcc-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="6fbcc-128">Response</span></span>
<span data-ttu-id="6fbcc-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6fbcc-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fbcc-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6fbcc-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6fbcc-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6fbcc-131">Request</span></span>
<span data-ttu-id="6fbcc-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6fbcc-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="6fbcc-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="6fbcc-133">Response</span></span>
<span data-ttu-id="6fbcc-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6fbcc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 687

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
      "id": "7560ee45-ee45-7560-45ee-607545ee6075",
      "deviceName": "Device Name value",
      "deviceId": "Device Id value",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "mobileAppInstallStatusValue": "failed",
      "installState": "failed",
      "installStateDetail": "seeInstallErrorCode",
      "errorCode": 9,
      "osVersion": "Os Version value",
      "osDescription": "Os Description value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value",
      "displayVersion": "Display Version value"
    }
  ]
}
```




