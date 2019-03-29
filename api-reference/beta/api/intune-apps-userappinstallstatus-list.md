---
title: UserAppInstallStatuses aufListen
description: AufListen von Eigenschaften und Beziehungen der userAppInstallStatus-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 84d2f7e1a4211bc717a57c5f80e774f5aa66c405
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980292"
---
# <a name="list-userappinstallstatuses"></a><span data-ttu-id="c27e7-103">UserAppInstallStatuses aufListen</span><span class="sxs-lookup"><span data-stu-id="c27e7-103">List userAppInstallStatuses</span></span>

> <span data-ttu-id="c27e7-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c27e7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c27e7-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c27e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c27e7-106">AufListen von Eigenschaften und Beziehungen der [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="c27e7-106">List properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c27e7-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c27e7-107">Prerequisites</span></span>
<span data-ttu-id="c27e7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c27e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c27e7-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c27e7-110">Permission type</span></span>|<span data-ttu-id="c27e7-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c27e7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c27e7-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c27e7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c27e7-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c27e7-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c27e7-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c27e7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c27e7-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c27e7-115">Not supported.</span></span>|
|<span data-ttu-id="c27e7-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c27e7-116">Application</span></span>|<span data-ttu-id="c27e7-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c27e7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c27e7-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c27e7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="c27e7-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c27e7-119">Request headers</span></span>
|<span data-ttu-id="c27e7-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c27e7-120">Header</span></span>|<span data-ttu-id="c27e7-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c27e7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c27e7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c27e7-122">Authorization</span></span>|<span data-ttu-id="c27e7-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c27e7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c27e7-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c27e7-124">Accept</span></span>|<span data-ttu-id="c27e7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c27e7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c27e7-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c27e7-126">Request body</span></span>
<span data-ttu-id="c27e7-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c27e7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c27e7-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="c27e7-128">Response</span></span>
<span data-ttu-id="c27e7-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c27e7-129">If successful, this method returns a `200 OK` response code and a collection of [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c27e7-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c27e7-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c27e7-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c27e7-131">Request</span></span>
<span data-ttu-id="c27e7-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c27e7-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="c27e7-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="c27e7-133">Response</span></span>
<span data-ttu-id="c27e7-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c27e7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 349

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userAppInstallStatus",
      "id": "14959a2a-9a2a-1495-2a9a-95142a9a9514",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value",
      "installedDeviceCount": 4,
      "failedDeviceCount": 1,
      "notInstalledDeviceCount": 7
    }
  ]
}
```




