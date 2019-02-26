---
title: RestrictedAppsViolation abrufen
description: Lesen von Eigenschaften und Beziehungen des restrictedAppsViolation-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 256bd07a46fc8380206e3f705566fc1ab23e01b5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147243"
---
# <a name="get-restrictedappsviolation"></a><span data-ttu-id="2a9aa-103">RestrictedAppsViolation abrufen</span><span class="sxs-lookup"><span data-stu-id="2a9aa-103">Get restrictedAppsViolation</span></span>

> <span data-ttu-id="2a9aa-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2a9aa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a9aa-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2a9aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a9aa-106">Lesen von Eigenschaften und Beziehungen des [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2a9aa-106">Read properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a9aa-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2a9aa-107">Prerequisites</span></span>
<span data-ttu-id="2a9aa-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2a9aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2a9aa-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2a9aa-110">Permission type</span></span>|<span data-ttu-id="2a9aa-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2a9aa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a9aa-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2a9aa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2a9aa-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a9aa-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2a9aa-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2a9aa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a9aa-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a9aa-115">Not supported.</span></span>|
|<span data-ttu-id="2a9aa-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2a9aa-116">Application</span></span>|<span data-ttu-id="2a9aa-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a9aa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a9aa-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a9aa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2a9aa-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="2a9aa-119">Optional query parameters</span></span>
<span data-ttu-id="2a9aa-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2a9aa-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2a9aa-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2a9aa-121">Request headers</span></span>
|<span data-ttu-id="2a9aa-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2a9aa-122">Header</span></span>|<span data-ttu-id="2a9aa-123">Wert</span><span class="sxs-lookup"><span data-stu-id="2a9aa-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a9aa-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a9aa-124">Authorization</span></span>|<span data-ttu-id="2a9aa-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2a9aa-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a9aa-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2a9aa-126">Accept</span></span>|<span data-ttu-id="2a9aa-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2a9aa-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a9aa-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2a9aa-128">Request body</span></span>
<span data-ttu-id="2a9aa-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2a9aa-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a9aa-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a9aa-130">Response</span></span>
<span data-ttu-id="2a9aa-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2a9aa-131">If successful, this method returns a `200 OK` response code and [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a9aa-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2a9aa-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a9aa-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a9aa-133">Request</span></span>
<span data-ttu-id="2a9aa-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2a9aa-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

### <a name="response"></a><span data-ttu-id="2a9aa-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a9aa-135">Response</span></span>
<span data-ttu-id="2a9aa-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2a9aa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




