---
title: Abrufen von windowsProtectionState
description: Lesen Sie Eigenschaften und Beziehungen des WindowsProtectionState-Objekts.
ms.openlocfilehash: 064b47a9595838d0e77a5378b6238e9f6fd227b6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060944"
---
# <a name="get-windowsprotectionstate"></a><span data-ttu-id="0da52-103">Abrufen von windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="0da52-103">Get windowsProtectionState</span></span>

> <span data-ttu-id="0da52-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0da52-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0da52-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0da52-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0da52-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0da52-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0da52-107">Lesen Sie Eigenschaften und Beziehungen des [WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0da52-107">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0da52-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0da52-108">Prerequisites</span></span>
<span data-ttu-id="0da52-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0da52-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0da52-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0da52-111">Permission type</span></span>|<span data-ttu-id="0da52-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0da52-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0da52-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0da52-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0da52-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0da52-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="0da52-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0da52-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0da52-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0da52-116">Not supported.</span></span>|
|<span data-ttu-id="0da52-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0da52-117">Application</span></span>|<span data-ttu-id="0da52-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0da52-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0da52-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0da52-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0da52-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0da52-120">Optional query parameters</span></span>
<span data-ttu-id="0da52-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0da52-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0da52-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0da52-122">Request headers</span></span>
|<span data-ttu-id="0da52-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0da52-123">Header</span></span>|<span data-ttu-id="0da52-124">Wert</span><span class="sxs-lookup"><span data-stu-id="0da52-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0da52-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0da52-125">Authorization</span></span>|<span data-ttu-id="0da52-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0da52-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0da52-127">Accept</span><span class="sxs-lookup"><span data-stu-id="0da52-127">Accept</span></span>|<span data-ttu-id="0da52-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0da52-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0da52-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0da52-129">Request body</span></span>
<span data-ttu-id="0da52-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0da52-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0da52-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="0da52-131">Response</span></span>
<span data-ttu-id="0da52-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0da52-132">If successful, this method returns a `200 OK` response code and [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0da52-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0da52-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="0da52-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0da52-134">Request</span></span>
<span data-ttu-id="0da52-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0da52-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
```

### <a name="response"></a><span data-ttu-id="0da52-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="0da52-136">Response</span></span>
<span data-ttu-id="0da52-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0da52-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 971

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsProtectionState",
    "id": "1ac6ea5a-ea5a-1ac6-5aea-c61a5aeac61a",
    "malwareProtectionEnabled": true,
    "deviceState": "fullScanPending",
    "realTimeProtectionEnabled": true,
    "networkInspectionSystemEnabled": true,
    "quickScanOverdue": true,
    "fullScanOverdue": true,
    "signatureUpdateOverdue": true,
    "rebootRequired": true,
    "fullScanRequired": true,
    "engineVersion": "Engine Version value",
    "signatureVersion": "Signature Version value",
    "antiMalwareVersion": "Anti Malware Version value",
    "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
    "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
    "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
    "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
  }
}
```





