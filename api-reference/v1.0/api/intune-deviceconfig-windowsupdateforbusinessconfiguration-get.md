---
title: Abrufen von „windowsUpdateForBusinessConfiguration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs windowsUpdateForBusinessConfiguration.
author: tfitzmac
ms.openlocfilehash: b0ddb0e650fb860d005268f26102de79e01026bb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344206"
---
# <a name="get-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="28aae-103">Abrufen von „windowsUpdateForBusinessConfiguration“</span><span class="sxs-lookup"><span data-stu-id="28aae-103">Get windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="28aae-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="28aae-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="28aae-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="28aae-105">Read properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="28aae-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="28aae-106">Prerequisites</span></span>
<span data-ttu-id="28aae-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28aae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28aae-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="28aae-109">Permission type</span></span>|<span data-ttu-id="28aae-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="28aae-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28aae-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="28aae-111">Delegated (work or school account)</span></span>|<span data-ttu-id="28aae-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="28aae-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="28aae-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="28aae-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28aae-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="28aae-114">Not supported.</span></span>|
|<span data-ttu-id="28aae-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="28aae-115">Application</span></span>|<span data-ttu-id="28aae-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="28aae-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28aae-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="28aae-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="28aae-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="28aae-118">Optional query parameters</span></span>
<span data-ttu-id="28aae-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="28aae-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="28aae-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="28aae-120">Request headers</span></span>
|<span data-ttu-id="28aae-121">Header</span><span class="sxs-lookup"><span data-stu-id="28aae-121">Header</span></span>|<span data-ttu-id="28aae-122">Wert</span><span class="sxs-lookup"><span data-stu-id="28aae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28aae-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="28aae-123">Authorization</span></span>|<span data-ttu-id="28aae-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="28aae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28aae-125">Accept</span><span class="sxs-lookup"><span data-stu-id="28aae-125">Accept</span></span>|<span data-ttu-id="28aae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="28aae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28aae-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="28aae-127">Request body</span></span>
<span data-ttu-id="28aae-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="28aae-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28aae-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="28aae-129">Response</span></span>
<span data-ttu-id="28aae-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="28aae-130">If successful, this method returns a `200 OK` response code and [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28aae-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="28aae-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="28aae-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="28aae-132">Request</span></span>
<span data-ttu-id="28aae-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="28aae-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="28aae-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="28aae-134">Response</span></span>
<span data-ttu-id="28aae-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="28aae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1149

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
    "id": "4928dd6a-dd6a-4928-6add-28496add2849",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "deliveryOptimizationMode": "httpOnly",
    "prereleaseFeatures": "settingsOnly",
    "automaticUpdateMode": "notifyDownload",
    "microsoftUpdateServiceAllowed": true,
    "driversExcluded": true,
    "installationSchedule": {
      "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
      "scheduledInstallDay": "everyday",
      "scheduledInstallTime": "11:59:31.3170000"
    },
    "qualityUpdatesDeferralPeriodInDays": 2,
    "featureUpdatesDeferralPeriodInDays": 2,
    "qualityUpdatesPaused": true,
    "featureUpdatesPaused": true,
    "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
    "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
    "businessReadyUpdatesOnly": "all"
  }
}
```



