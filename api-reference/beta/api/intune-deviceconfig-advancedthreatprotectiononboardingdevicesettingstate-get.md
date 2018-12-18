---
title: Abrufen von advancedThreatProtectionOnboardingDeviceSettingState
description: Lesen Sie Eigenschaften und Beziehungen des AdvancedThreatProtectionOnboardingDeviceSettingState-Objekts.
author: tfitzmac
ms.openlocfilehash: 368cc4ab180fa55930887c68640c6c29ad62fab3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303430"
---
# <a name="get-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="6ecb6-103">Abrufen von advancedThreatProtectionOnboardingDeviceSettingState</span><span class="sxs-lookup"><span data-stu-id="6ecb6-103">Get advancedThreatProtectionOnboardingDeviceSettingState</span></span>

> <span data-ttu-id="6ecb6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ecb6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6ecb6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ecb6-107">Lesen Sie Eigenschaften und Beziehungen des [AdvancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-107">Read properties and relationships of the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6ecb6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6ecb6-108">Prerequisites</span></span>
<span data-ttu-id="6ecb6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ecb6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ecb6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6ecb6-111">Permission type</span></span>|<span data-ttu-id="6ecb6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6ecb6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ecb6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6ecb6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6ecb6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ecb6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6ecb6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6ecb6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ecb6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6ecb6-116">Not supported.</span></span>|
|<span data-ttu-id="6ecb6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6ecb6-117">Application</span></span>|<span data-ttu-id="6ecb6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6ecb6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ecb6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6ecb6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6ecb6-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6ecb6-120">Optional query parameters</span></span>
<span data-ttu-id="6ecb6-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6ecb6-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6ecb6-122">Request headers</span></span>
|<span data-ttu-id="6ecb6-123">Header</span><span class="sxs-lookup"><span data-stu-id="6ecb6-123">Header</span></span>|<span data-ttu-id="6ecb6-124">Wert</span><span class="sxs-lookup"><span data-stu-id="6ecb6-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ecb6-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="6ecb6-125">Authorization</span></span>|<span data-ttu-id="6ecb6-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6ecb6-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ecb6-127">Accept</span><span class="sxs-lookup"><span data-stu-id="6ecb6-127">Accept</span></span>|<span data-ttu-id="6ecb6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6ecb6-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ecb6-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6ecb6-129">Request body</span></span>
<span data-ttu-id="6ecb6-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ecb6-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="6ecb6-131">Response</span></span>
<span data-ttu-id="6ecb6-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [AdvancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-132">If successful, this method returns a `200 OK` response code and [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ecb6-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6ecb6-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="6ecb6-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6ecb6-134">Request</span></span>
<span data-ttu-id="6ecb6-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="6ecb6-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="6ecb6-136">Response</span></span>
<span data-ttu-id="6ecb6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6ecb6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 669

{
  "value": {
    "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingDeviceSettingState",
    "id": "63593fc6-3fc6-6359-c63f-5963c63f5963",
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





