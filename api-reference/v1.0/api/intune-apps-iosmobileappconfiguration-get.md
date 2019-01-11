---
title: iosMobileAppConfiguration abrufen
description: Lesen von Eigenschaften und Beziehungen des iosMobileAppConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a694364197ae3e660b7caa829eecb478ee449774
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872401"
---
# <a name="get-iosmobileappconfiguration"></a><span data-ttu-id="cbf81-103">iosMobileAppConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="cbf81-103">Get iosMobileAppConfiguration</span></span>

> <span data-ttu-id="cbf81-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cbf81-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cbf81-105">Lesen von Eigenschaften und Beziehungen des [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="cbf81-105">Read properties and relationships of the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cbf81-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cbf81-106">Prerequisites</span></span>
<span data-ttu-id="cbf81-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbf81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbf81-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cbf81-109">Permission type</span></span>|<span data-ttu-id="cbf81-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cbf81-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbf81-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cbf81-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cbf81-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cbf81-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="cbf81-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cbf81-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbf81-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cbf81-114">Not supported.</span></span>|
|<span data-ttu-id="cbf81-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cbf81-115">Application</span></span>|<span data-ttu-id="cbf81-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cbf81-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbf81-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cbf81-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cbf81-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cbf81-118">Optional query parameters</span></span>
<span data-ttu-id="cbf81-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cbf81-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cbf81-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cbf81-120">Request headers</span></span>
|<span data-ttu-id="cbf81-121">Header</span><span class="sxs-lookup"><span data-stu-id="cbf81-121">Header</span></span>|<span data-ttu-id="cbf81-122">Wert</span><span class="sxs-lookup"><span data-stu-id="cbf81-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbf81-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbf81-123">Authorization</span></span>|<span data-ttu-id="cbf81-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cbf81-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbf81-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="cbf81-125">Accept</span></span>|<span data-ttu-id="cbf81-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cbf81-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbf81-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cbf81-127">Request body</span></span>
<span data-ttu-id="cbf81-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cbf81-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cbf81-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="cbf81-129">Response</span></span>
<span data-ttu-id="cbf81-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="cbf81-130">If successful, this method returns a `200 OK` response code and [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbf81-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cbf81-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="cbf81-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cbf81-132">Request</span></span>
<span data-ttu-id="cbf81-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cbf81-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="cbf81-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="cbf81-134">Response</span></span>
<span data-ttu-id="cbf81-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cbf81-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 763

{
  "value": {
    "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
    "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
    "targetedMobileApps": [
      "Targeted Mobile Apps value"
    ],
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
    "settings": [
      {
        "@odata.type": "microsoft.graph.appConfigurationSettingItem",
        "appConfigKey": "App Config Key value",
        "appConfigKeyType": "integerType",
        "appConfigKeyValue": "App Config Key Value value"
      }
    ]
  }
}
```



