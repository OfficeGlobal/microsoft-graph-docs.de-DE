---
title: Auflisten von „deviceCompliancePolicySettingStateSummary“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceCompliancePolicySettingStateSummary auf.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f7f990eef1dbd7d36818ead10e57a13de54280c5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979509"
---
# <a name="list-devicecompliancepolicysettingstatesummaries"></a><span data-ttu-id="09325-103">Auflisten von „deviceCompliancePolicySettingStateSummary“</span><span class="sxs-lookup"><span data-stu-id="09325-103">List deviceCompliancePolicySettingStateSummaries</span></span>

> <span data-ttu-id="09325-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="09325-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="09325-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="09325-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="09325-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="09325-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09325-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) auf.</span><span class="sxs-lookup"><span data-stu-id="09325-107">List properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="09325-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="09325-108">Prerequisites</span></span>
<span data-ttu-id="09325-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09325-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09325-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="09325-111">Permission type</span></span>|<span data-ttu-id="09325-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="09325-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09325-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="09325-113">Delegated (work or school account)</span></span>|<span data-ttu-id="09325-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="09325-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="09325-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="09325-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09325-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="09325-116">Not supported.</span></span>|
|<span data-ttu-id="09325-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="09325-117">Application</span></span>|<span data-ttu-id="09325-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="09325-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09325-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="09325-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="09325-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="09325-120">Request headers</span></span>
|<span data-ttu-id="09325-121">Header</span><span class="sxs-lookup"><span data-stu-id="09325-121">Header</span></span>|<span data-ttu-id="09325-122">Wert</span><span class="sxs-lookup"><span data-stu-id="09325-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09325-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="09325-123">Authorization</span></span>|<span data-ttu-id="09325-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="09325-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09325-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="09325-125">Accept</span></span>|<span data-ttu-id="09325-126">application/json</span><span class="sxs-lookup"><span data-stu-id="09325-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09325-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="09325-127">Request body</span></span>
<span data-ttu-id="09325-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="09325-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09325-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="09325-129">Response</span></span>
<span data-ttu-id="09325-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="09325-130">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09325-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="09325-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="09325-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="09325-132">Request</span></span>
<span data-ttu-id="09325-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="09325-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="09325-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="09325-134">Response</span></span>
<span data-ttu-id="09325-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="09325-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 532

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
      "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "platformType": "androidForWork",
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





