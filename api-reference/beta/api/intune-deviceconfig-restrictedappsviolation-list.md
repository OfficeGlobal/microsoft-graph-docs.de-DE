---
title: RestrictedAppsViolations aufListen
description: AufListen von Eigenschaften und Beziehungen der restrictedAppsViolation-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3a66a87f30c815c45d9d8f39b44bd8409eb57705
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172107"
---
# <a name="list-restrictedappsviolations"></a><span data-ttu-id="a9498-103">RestrictedAppsViolations aufListen</span><span class="sxs-lookup"><span data-stu-id="a9498-103">List restrictedAppsViolations</span></span>

> <span data-ttu-id="a9498-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a9498-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9498-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a9498-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9498-106">AufListen von Eigenschaften und Beziehungen der [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="a9498-106">List properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9498-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a9498-107">Prerequisites</span></span>
<span data-ttu-id="a9498-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a9498-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a9498-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a9498-110">Permission type</span></span>|<span data-ttu-id="a9498-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a9498-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9498-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a9498-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a9498-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9498-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a9498-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a9498-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9498-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a9498-115">Not supported.</span></span>|
|<span data-ttu-id="a9498-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a9498-116">Application</span></span>|<span data-ttu-id="a9498-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a9498-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9498-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a9498-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a><span data-ttu-id="a9498-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a9498-119">Request headers</span></span>
|<span data-ttu-id="a9498-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a9498-120">Header</span></span>|<span data-ttu-id="a9498-121">Wert</span><span class="sxs-lookup"><span data-stu-id="a9498-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9498-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9498-122">Authorization</span></span>|<span data-ttu-id="a9498-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a9498-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9498-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a9498-124">Accept</span></span>|<span data-ttu-id="a9498-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a9498-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9498-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a9498-126">Request body</span></span>
<span data-ttu-id="a9498-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a9498-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9498-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="a9498-128">Response</span></span>
<span data-ttu-id="a9498-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a9498-129">If successful, this method returns a `200 OK` response code and a collection of [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9498-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a9498-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9498-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a9498-131">Request</span></span>
<span data-ttu-id="a9498-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a9498-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations
```

### <a name="response"></a><span data-ttu-id="a9498-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="a9498-133">Response</span></span>
<span data-ttu-id="a9498-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a9498-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 710

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.restrictedAppsViolation",
      "id": "53f99903-9903-53f9-0399-f9530399f953",
      "userId": "User Id value",
      "userName": "User Name value",
      "managedDeviceId": "Managed Device Id value",
      "deviceName": "Device Name value",
      "deviceConfigurationId": "Device Configuration Id value",
      "deviceConfigurationName": "Device Configuration Name value",
      "platformType": "androidForWork",
      "restrictedAppsState": "notApprovedApps",
      "restrictedApps": [
        {
          "@odata.type": "microsoft.graph.managedDeviceReportedApp",
          "appId": "App Id value"
        }
      ]
    }
  ]
}
```




