---
title: UserAppInstallStatuses aufListen
description: AufListen von Eigenschaften und Beziehungen der userAppInstallStatus-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a89090b81480e99b3c9b5ac0a7ade589971caa11
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143834"
---
# <a name="list-userappinstallstatuses"></a><span data-ttu-id="53523-103">UserAppInstallStatuses aufListen</span><span class="sxs-lookup"><span data-stu-id="53523-103">List userAppInstallStatuses</span></span>

> <span data-ttu-id="53523-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="53523-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53523-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="53523-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53523-106">AufListen von Eigenschaften und Beziehungen der [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="53523-106">List properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53523-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="53523-107">Prerequisites</span></span>
<span data-ttu-id="53523-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="53523-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="53523-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="53523-110">Permission type</span></span>|<span data-ttu-id="53523-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="53523-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53523-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="53523-112">Delegated (work or school account)</span></span>|<span data-ttu-id="53523-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="53523-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="53523-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="53523-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53523-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53523-115">Not supported.</span></span>|
|<span data-ttu-id="53523-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="53523-116">Application</span></span>|<span data-ttu-id="53523-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53523-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53523-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="53523-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="53523-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="53523-119">Request headers</span></span>
|<span data-ttu-id="53523-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="53523-120">Header</span></span>|<span data-ttu-id="53523-121">Wert</span><span class="sxs-lookup"><span data-stu-id="53523-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53523-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="53523-122">Authorization</span></span>|<span data-ttu-id="53523-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="53523-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53523-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="53523-124">Accept</span></span>|<span data-ttu-id="53523-125">application/json</span><span class="sxs-lookup"><span data-stu-id="53523-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53523-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="53523-126">Request body</span></span>
<span data-ttu-id="53523-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="53523-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53523-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="53523-128">Response</span></span>
<span data-ttu-id="53523-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="53523-129">If successful, this method returns a `200 OK` response code and a collection of [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53523-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="53523-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="53523-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="53523-131">Request</span></span>
<span data-ttu-id="53523-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="53523-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="53523-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="53523-133">Response</span></span>
<span data-ttu-id="53523-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="53523-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




