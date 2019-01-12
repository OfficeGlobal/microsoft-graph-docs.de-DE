---
title: Liste restrictedAppsViolations
description: Listeneigenschaften und Beziehungen der RestrictedAppsViolation-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ecd78f2300461198b31fb94117005995d12892bb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950375"
---
# <a name="list-restrictedappsviolations"></a><span data-ttu-id="80018-103">Liste restrictedAppsViolations</span><span class="sxs-lookup"><span data-stu-id="80018-103">List restrictedAppsViolations</span></span>

> <span data-ttu-id="80018-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="80018-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80018-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="80018-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="80018-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="80018-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80018-107">Listeneigenschaften und Beziehungen der [RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="80018-107">List properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="80018-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="80018-108">Prerequisites</span></span>
<span data-ttu-id="80018-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80018-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80018-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="80018-111">Permission type</span></span>|<span data-ttu-id="80018-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="80018-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80018-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="80018-113">Delegated (work or school account)</span></span>|<span data-ttu-id="80018-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="80018-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="80018-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="80018-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80018-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="80018-116">Not supported.</span></span>|
|<span data-ttu-id="80018-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="80018-117">Application</span></span>|<span data-ttu-id="80018-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="80018-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80018-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="80018-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a><span data-ttu-id="80018-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="80018-120">Request headers</span></span>
|<span data-ttu-id="80018-121">Header</span><span class="sxs-lookup"><span data-stu-id="80018-121">Header</span></span>|<span data-ttu-id="80018-122">Wert</span><span class="sxs-lookup"><span data-stu-id="80018-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80018-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="80018-123">Authorization</span></span>|<span data-ttu-id="80018-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="80018-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80018-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="80018-125">Accept</span></span>|<span data-ttu-id="80018-126">application/json</span><span class="sxs-lookup"><span data-stu-id="80018-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80018-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="80018-127">Request body</span></span>
<span data-ttu-id="80018-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="80018-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80018-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="80018-129">Response</span></span>
<span data-ttu-id="80018-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="80018-130">If successful, this method returns a `200 OK` response code and a collection of [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80018-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="80018-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="80018-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="80018-132">Request</span></span>
<span data-ttu-id="80018-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="80018-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations
```

### <a name="response"></a><span data-ttu-id="80018-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="80018-134">Response</span></span>
<span data-ttu-id="80018-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="80018-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





