---
title: Auflisten von „settingStateDeviceSummary“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs settingStateDeviceSummary auf.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0bdf1622396f58c3451029b2164d5d6273035d9b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839123"
---
# <a name="list-settingstatedevicesummaries"></a><span data-ttu-id="9c1a4-103">Auflisten von „settingStateDeviceSummary“</span><span class="sxs-lookup"><span data-stu-id="9c1a4-103">List settingStateDeviceSummaries</span></span>

> <span data-ttu-id="9c1a4-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9c1a4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c1a4-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) auf.</span><span class="sxs-lookup"><span data-stu-id="9c1a4-105">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9c1a4-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9c1a4-106">Prerequisites</span></span>
<span data-ttu-id="9c1a4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c1a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c1a4-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9c1a4-109">Permission type</span></span>|<span data-ttu-id="9c1a4-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9c1a4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c1a4-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9c1a4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9c1a4-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c1a4-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9c1a4-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9c1a4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c1a4-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9c1a4-114">Not supported.</span></span>|
|<span data-ttu-id="9c1a4-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9c1a4-115">Application</span></span>|<span data-ttu-id="9c1a4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9c1a4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c1a4-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9c1a4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="9c1a4-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9c1a4-118">Request headers</span></span>
|<span data-ttu-id="9c1a4-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9c1a4-119">Header</span></span>|<span data-ttu-id="9c1a4-120">Wert</span><span class="sxs-lookup"><span data-stu-id="9c1a4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c1a4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c1a4-121">Authorization</span></span>|<span data-ttu-id="9c1a4-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9c1a4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c1a4-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9c1a4-123">Accept</span></span>|<span data-ttu-id="9c1a4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9c1a4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c1a4-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9c1a4-125">Request body</span></span>
<span data-ttu-id="9c1a4-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9c1a4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c1a4-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="9c1a4-127">Response</span></span>
<span data-ttu-id="9c1a4-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9c1a4-128">If successful, this method returns a `200 OK` response code and a collection of [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c1a4-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9c1a4-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="9c1a4-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9c1a4-130">Request</span></span>
<span data-ttu-id="9c1a4-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9c1a4-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="9c1a4-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="9c1a4-132">Response</span></span>
<span data-ttu-id="9c1a4-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9c1a4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 486

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
      "id": "3e2d4526-4526-3e2d-2645-2d3e26452d3e",
      "settingName": "Setting Name value",
      "instancePath": "Instance Path value",
      "unknownDeviceCount": 2,
      "notApplicableDeviceCount": 8,
      "compliantDeviceCount": 4,
      "remediatedDeviceCount": 5,
      "nonCompliantDeviceCount": 7,
      "errorDeviceCount": 0,
      "conflictDeviceCount": 3
    }
  ]
}
```



