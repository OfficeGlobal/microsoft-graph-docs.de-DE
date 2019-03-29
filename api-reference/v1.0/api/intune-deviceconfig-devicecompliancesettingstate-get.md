---
title: deviceComplianceSettingState abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceComplianceSettingState-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1c804f03218ad7a0cb5385bb4ca73dc12d83460f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980362"
---
# <a name="get-devicecompliancesettingstate"></a><span data-ttu-id="28e14-103">deviceComplianceSettingState abrufen</span><span class="sxs-lookup"><span data-stu-id="28e14-103">Get deviceComplianceSettingState</span></span>

> <span data-ttu-id="28e14-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="28e14-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28e14-105">Lesen von Eigenschaften und Beziehungen des [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="28e14-105">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28e14-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="28e14-106">Prerequisites</span></span>
<span data-ttu-id="28e14-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28e14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28e14-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="28e14-109">Permission type</span></span>|<span data-ttu-id="28e14-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="28e14-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28e14-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="28e14-111">Delegated (work or school account)</span></span>|<span data-ttu-id="28e14-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="28e14-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="28e14-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="28e14-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28e14-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="28e14-114">Not supported.</span></span>|
|<span data-ttu-id="28e14-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="28e14-115">Application</span></span>|<span data-ttu-id="28e14-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="28e14-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28e14-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="28e14-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="28e14-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="28e14-118">Optional query parameters</span></span>
<span data-ttu-id="28e14-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="28e14-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="28e14-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="28e14-120">Request headers</span></span>
|<span data-ttu-id="28e14-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="28e14-121">Header</span></span>|<span data-ttu-id="28e14-122">Wert</span><span class="sxs-lookup"><span data-stu-id="28e14-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28e14-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="28e14-123">Authorization</span></span>|<span data-ttu-id="28e14-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="28e14-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28e14-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="28e14-125">Accept</span></span>|<span data-ttu-id="28e14-126">application/json</span><span class="sxs-lookup"><span data-stu-id="28e14-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28e14-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="28e14-127">Request body</span></span>
<span data-ttu-id="28e14-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="28e14-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28e14-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="28e14-129">Response</span></span>
<span data-ttu-id="28e14-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="28e14-130">If successful, this method returns a `200 OK` response code and [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28e14-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="28e14-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="28e14-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="28e14-132">Request</span></span>
<span data-ttu-id="28e14-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="28e14-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="28e14-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="28e14-134">Response</span></span>
<span data-ttu-id="28e14-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="28e14-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



