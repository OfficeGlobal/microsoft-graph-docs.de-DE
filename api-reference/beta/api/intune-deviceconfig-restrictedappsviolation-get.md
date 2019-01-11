---
title: Abrufen von restrictedAppsViolation
description: Lesen Sie Eigenschaften und Beziehungen des RestrictedAppsViolation-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 69daff20c843d1be47ff2f97e7a4190acc7a8a51
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891889"
---
# <a name="get-restrictedappsviolation"></a><span data-ttu-id="f73c9-103">Abrufen von restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="f73c9-103">Get restrictedAppsViolation</span></span>

> <span data-ttu-id="f73c9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f73c9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f73c9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f73c9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f73c9-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f73c9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f73c9-107">Lesen Sie Eigenschaften und Beziehungen des [RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f73c9-107">Read properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f73c9-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f73c9-108">Prerequisites</span></span>
<span data-ttu-id="f73c9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f73c9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f73c9-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f73c9-111">Permission type</span></span>|<span data-ttu-id="f73c9-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f73c9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f73c9-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f73c9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f73c9-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f73c9-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f73c9-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f73c9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f73c9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f73c9-116">Not supported.</span></span>|
|<span data-ttu-id="f73c9-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f73c9-117">Application</span></span>|<span data-ttu-id="f73c9-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f73c9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f73c9-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f73c9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f73c9-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f73c9-120">Optional query parameters</span></span>
<span data-ttu-id="f73c9-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f73c9-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f73c9-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f73c9-122">Request headers</span></span>
|<span data-ttu-id="f73c9-123">Header</span><span class="sxs-lookup"><span data-stu-id="f73c9-123">Header</span></span>|<span data-ttu-id="f73c9-124">Wert</span><span class="sxs-lookup"><span data-stu-id="f73c9-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f73c9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f73c9-125">Authorization</span></span>|<span data-ttu-id="f73c9-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f73c9-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f73c9-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f73c9-127">Accept</span></span>|<span data-ttu-id="f73c9-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f73c9-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f73c9-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f73c9-129">Request body</span></span>
<span data-ttu-id="f73c9-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f73c9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f73c9-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="f73c9-131">Response</span></span>
<span data-ttu-id="f73c9-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f73c9-132">If successful, this method returns a `200 OK` response code and [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f73c9-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f73c9-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="f73c9-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f73c9-134">Request</span></span>
<span data-ttu-id="f73c9-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f73c9-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

### <a name="response"></a><span data-ttu-id="f73c9-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="f73c9-136">Response</span></span>
<span data-ttu-id="f73c9-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f73c9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 664

{
  "value": {
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
}
```





