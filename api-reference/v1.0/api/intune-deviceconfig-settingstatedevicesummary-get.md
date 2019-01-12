---
title: Abrufen von „settingStateDeviceSummary“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs settingStateDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9ab2a547bbc5ef888fc3f7dbee4ddd1934ce5b95
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941870"
---
# <a name="get-settingstatedevicesummary"></a><span data-ttu-id="36514-103">Abrufen von „settingStateDeviceSummary“</span><span class="sxs-lookup"><span data-stu-id="36514-103">Get settingStateDeviceSummary</span></span>

> <span data-ttu-id="36514-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="36514-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="36514-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="36514-105">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="36514-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="36514-106">Prerequisites</span></span>
<span data-ttu-id="36514-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36514-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36514-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="36514-109">Permission type</span></span>|<span data-ttu-id="36514-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="36514-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36514-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="36514-111">Delegated (work or school account)</span></span>|<span data-ttu-id="36514-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="36514-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="36514-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="36514-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36514-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="36514-114">Not supported.</span></span>|
|<span data-ttu-id="36514-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="36514-115">Application</span></span>|<span data-ttu-id="36514-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="36514-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36514-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="36514-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="36514-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="36514-118">Optional query parameters</span></span>
<span data-ttu-id="36514-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="36514-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="36514-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="36514-120">Request headers</span></span>
|<span data-ttu-id="36514-121">Header</span><span class="sxs-lookup"><span data-stu-id="36514-121">Header</span></span>|<span data-ttu-id="36514-122">Wert</span><span class="sxs-lookup"><span data-stu-id="36514-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36514-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="36514-123">Authorization</span></span>|<span data-ttu-id="36514-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="36514-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36514-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="36514-125">Accept</span></span>|<span data-ttu-id="36514-126">application/json</span><span class="sxs-lookup"><span data-stu-id="36514-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36514-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="36514-127">Request body</span></span>
<span data-ttu-id="36514-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="36514-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36514-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="36514-129">Response</span></span>
<span data-ttu-id="36514-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="36514-130">If successful, this method returns a `200 OK` response code and [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36514-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="36514-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="36514-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="36514-132">Request</span></span>
<span data-ttu-id="36514-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="36514-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

### <a name="response"></a><span data-ttu-id="36514-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="36514-134">Response</span></span>
<span data-ttu-id="36514-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="36514-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "value": {
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
}
```



