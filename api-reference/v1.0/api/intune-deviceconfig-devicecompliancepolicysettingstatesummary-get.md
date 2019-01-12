---
title: deviceCompliancePolicySettingStateSummary abrufen
description: Lesen von Eigenschaften und Beziehungen der deviceCompliancePolicySettingStateSummary-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bbff377d832a569cbfa22feb3d28fdc0bf975857
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974210"
---
# <a name="get-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="f98f4-103">deviceCompliancePolicySettingStateSummary abrufen</span><span class="sxs-lookup"><span data-stu-id="f98f4-103">Get deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="f98f4-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f98f4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f98f4-105">Lesen von Eigenschaften und Beziehungen der [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="f98f4-105">Read properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f98f4-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f98f4-106">Prerequisites</span></span>
<span data-ttu-id="f98f4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f98f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f98f4-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f98f4-109">Permission type</span></span>|<span data-ttu-id="f98f4-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f98f4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f98f4-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f98f4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f98f4-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f98f4-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f98f4-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f98f4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f98f4-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f98f4-114">Not supported.</span></span>|
|<span data-ttu-id="f98f4-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f98f4-115">Application</span></span>|<span data-ttu-id="f98f4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f98f4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f98f4-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f98f4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f98f4-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f98f4-118">Optional query parameters</span></span>
<span data-ttu-id="f98f4-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f98f4-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f98f4-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f98f4-120">Request headers</span></span>
|<span data-ttu-id="f98f4-121">Header</span><span class="sxs-lookup"><span data-stu-id="f98f4-121">Header</span></span>|<span data-ttu-id="f98f4-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f98f4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f98f4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f98f4-123">Authorization</span></span>|<span data-ttu-id="f98f4-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f98f4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f98f4-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f98f4-125">Accept</span></span>|<span data-ttu-id="f98f4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f98f4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f98f4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f98f4-127">Request body</span></span>
<span data-ttu-id="f98f4-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f98f4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f98f4-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f98f4-129">Response</span></span>
<span data-ttu-id="f98f4-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f98f4-130">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f98f4-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f98f4-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f98f4-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f98f4-132">Request</span></span>
<span data-ttu-id="f98f4-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f98f4-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="f98f4-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f98f4-134">Response</span></span>
<span data-ttu-id="f98f4-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f98f4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 483

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
    "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
    "setting": "Setting value",
    "settingName": "Setting Name value",
    "platformType": "iOS",
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



