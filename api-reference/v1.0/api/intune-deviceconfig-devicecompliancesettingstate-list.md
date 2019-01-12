---
title: Auflisten von „deviceComplianceSettingState“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceComplianceSettingState auf.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 41db2fb82a492d061f0dfdbbf1bfe5782f7fad02
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971718"
---
# <a name="list-devicecompliancesettingstates"></a><span data-ttu-id="6d3d8-103">Auflisten von „deviceComplianceSettingState“</span><span class="sxs-lookup"><span data-stu-id="6d3d8-103">List deviceComplianceSettingStates</span></span>

> <span data-ttu-id="6d3d8-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6d3d8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6d3d8-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) auf.</span><span class="sxs-lookup"><span data-stu-id="6d3d8-105">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6d3d8-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6d3d8-106">Prerequisites</span></span>
<span data-ttu-id="6d3d8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d3d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d3d8-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6d3d8-109">Permission type</span></span>|<span data-ttu-id="6d3d8-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6d3d8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d3d8-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6d3d8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6d3d8-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6d3d8-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6d3d8-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6d3d8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d3d8-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6d3d8-114">Not supported.</span></span>|
|<span data-ttu-id="6d3d8-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6d3d8-115">Application</span></span>|<span data-ttu-id="6d3d8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6d3d8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d3d8-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6d3d8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="6d3d8-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6d3d8-118">Request headers</span></span>
|<span data-ttu-id="6d3d8-119">Header</span><span class="sxs-lookup"><span data-stu-id="6d3d8-119">Header</span></span>|<span data-ttu-id="6d3d8-120">Wert</span><span class="sxs-lookup"><span data-stu-id="6d3d8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d3d8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d3d8-121">Authorization</span></span>|<span data-ttu-id="6d3d8-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6d3d8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d3d8-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6d3d8-123">Accept</span></span>|<span data-ttu-id="6d3d8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6d3d8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d3d8-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6d3d8-125">Request body</span></span>
<span data-ttu-id="6d3d8-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6d3d8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d3d8-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="6d3d8-127">Response</span></span>
<span data-ttu-id="6d3d8-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6d3d8-128">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d3d8-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6d3d8-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="6d3d8-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6d3d8-130">Request</span></span>
<span data-ttu-id="6d3d8-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6d3d8-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

### <a name="response"></a><span data-ttu-id="6d3d8-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="6d3d8-132">Response</span></span>
<span data-ttu-id="6d3d8-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6d3d8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 651

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
      "id": "9905f955-f955-9905-55f9-059955f90599",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "deviceId": "Device Id value",
      "deviceName": "Device Name value",
      "userId": "User Id value",
      "userEmail": "User Email value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value",
      "deviceModel": "Device Model value",
      "state": "notApplicable",
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
    }
  ]
}
```



