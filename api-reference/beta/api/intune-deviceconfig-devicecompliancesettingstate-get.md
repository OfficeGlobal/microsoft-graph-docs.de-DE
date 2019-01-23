---
title: deviceComplianceSettingState abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceComplianceSettingState-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: acbd148b60fffa11144d457fb4dee20082cd6145
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418302"
---
# <a name="get-devicecompliancesettingstate"></a><span data-ttu-id="7afa6-103">deviceComplianceSettingState abrufen</span><span class="sxs-lookup"><span data-stu-id="7afa6-103">Get deviceComplianceSettingState</span></span>

> <span data-ttu-id="7afa6-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="7afa6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7afa6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7afa6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7afa6-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7afa6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7afa6-107">Lesen von Eigenschaften und Beziehungen des [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7afa6-107">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7afa6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7afa6-108">Prerequisites</span></span>
<span data-ttu-id="7afa6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7afa6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7afa6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7afa6-111">Permission type</span></span>|<span data-ttu-id="7afa6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7afa6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7afa6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7afa6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7afa6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7afa6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7afa6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7afa6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7afa6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7afa6-116">Not supported.</span></span>|
|<span data-ttu-id="7afa6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7afa6-117">Application</span></span>|<span data-ttu-id="7afa6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7afa6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7afa6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7afa6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7afa6-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="7afa6-120">Optional query parameters</span></span>
<span data-ttu-id="7afa6-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7afa6-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7afa6-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7afa6-122">Request headers</span></span>
|<span data-ttu-id="7afa6-123">Header</span><span class="sxs-lookup"><span data-stu-id="7afa6-123">Header</span></span>|<span data-ttu-id="7afa6-124">Wert</span><span class="sxs-lookup"><span data-stu-id="7afa6-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7afa6-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="7afa6-125">Authorization</span></span>|<span data-ttu-id="7afa6-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7afa6-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7afa6-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7afa6-127">Accept</span></span>|<span data-ttu-id="7afa6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7afa6-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7afa6-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7afa6-129">Request body</span></span>
<span data-ttu-id="7afa6-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7afa6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7afa6-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="7afa6-131">Response</span></span>
<span data-ttu-id="7afa6-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7afa6-132">If successful, this method returns a `200 OK` response code and [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7afa6-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7afa6-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="7afa6-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7afa6-134">Request</span></span>
<span data-ttu-id="7afa6-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7afa6-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="7afa6-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="7afa6-136">Response</span></span>
<span data-ttu-id="7afa6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7afa6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 645

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
    "id": "9905f955-f955-9905-55f9-059955f90599",
    "platformType": "windowsRT",
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




