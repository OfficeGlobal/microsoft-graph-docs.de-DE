---
title: deviceComplianceSettingState abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceComplianceSettingState-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3756cd0b0cb235d37dd0b97bb80d80dfbd7ba8b9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940631"
---
# <a name="get-devicecompliancesettingstate"></a><span data-ttu-id="40afd-103">deviceComplianceSettingState abrufen</span><span class="sxs-lookup"><span data-stu-id="40afd-103">Get deviceComplianceSettingState</span></span>

> <span data-ttu-id="40afd-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="40afd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40afd-105">Lesen von Eigenschaften und Beziehungen des [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="40afd-105">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="40afd-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="40afd-106">Prerequisites</span></span>
<span data-ttu-id="40afd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40afd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40afd-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="40afd-109">Permission type</span></span>|<span data-ttu-id="40afd-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="40afd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40afd-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="40afd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="40afd-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="40afd-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="40afd-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="40afd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40afd-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="40afd-114">Not supported.</span></span>|
|<span data-ttu-id="40afd-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="40afd-115">Application</span></span>|<span data-ttu-id="40afd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="40afd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40afd-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="40afd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="40afd-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="40afd-118">Optional query parameters</span></span>
<span data-ttu-id="40afd-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="40afd-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="40afd-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="40afd-120">Request headers</span></span>
|<span data-ttu-id="40afd-121">Header</span><span class="sxs-lookup"><span data-stu-id="40afd-121">Header</span></span>|<span data-ttu-id="40afd-122">Wert</span><span class="sxs-lookup"><span data-stu-id="40afd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40afd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="40afd-123">Authorization</span></span>|<span data-ttu-id="40afd-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="40afd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40afd-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="40afd-125">Accept</span></span>|<span data-ttu-id="40afd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="40afd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40afd-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="40afd-127">Request body</span></span>
<span data-ttu-id="40afd-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="40afd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40afd-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="40afd-129">Response</span></span>
<span data-ttu-id="40afd-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="40afd-130">If successful, this method returns a `200 OK` response code and [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40afd-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="40afd-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="40afd-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="40afd-132">Request</span></span>
<span data-ttu-id="40afd-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="40afd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="40afd-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="40afd-134">Response</span></span>
<span data-ttu-id="40afd-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="40afd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 611

{
  "value": {
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
}
```



