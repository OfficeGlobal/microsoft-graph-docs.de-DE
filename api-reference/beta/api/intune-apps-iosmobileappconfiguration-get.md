---
title: iosMobileAppConfiguration abrufen
description: Lesen von Eigenschaften und Beziehungen des iosMobileAppConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 79af23548c16e0d7797ce831aa2812066d3743cd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980356"
---
# <a name="get-iosmobileappconfiguration"></a><span data-ttu-id="3332c-103">iosMobileAppConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="3332c-103">Get iosMobileAppConfiguration</span></span>

> <span data-ttu-id="3332c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3332c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3332c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3332c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3332c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3332c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3332c-107">Lesen von Eigenschaften und Beziehungen des [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3332c-107">Read properties and relationships of the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3332c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3332c-108">Prerequisites</span></span>
<span data-ttu-id="3332c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3332c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3332c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3332c-111">Permission type</span></span>|<span data-ttu-id="3332c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3332c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3332c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3332c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3332c-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3332c-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3332c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3332c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3332c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3332c-116">Not supported.</span></span>|
|<span data-ttu-id="3332c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3332c-117">Application</span></span>|<span data-ttu-id="3332c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3332c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3332c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3332c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3332c-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3332c-120">Optional query parameters</span></span>
<span data-ttu-id="3332c-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3332c-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3332c-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3332c-122">Request headers</span></span>
|<span data-ttu-id="3332c-123">Header</span><span class="sxs-lookup"><span data-stu-id="3332c-123">Header</span></span>|<span data-ttu-id="3332c-124">Wert</span><span class="sxs-lookup"><span data-stu-id="3332c-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3332c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3332c-125">Authorization</span></span>|<span data-ttu-id="3332c-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3332c-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3332c-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3332c-127">Accept</span></span>|<span data-ttu-id="3332c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3332c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3332c-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3332c-129">Request body</span></span>
<span data-ttu-id="3332c-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3332c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3332c-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="3332c-131">Response</span></span>
<span data-ttu-id="3332c-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3332c-132">If successful, this method returns a `200 OK` response code and [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3332c-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3332c-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="3332c-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3332c-134">Request</span></span>
<span data-ttu-id="3332c-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3332c-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="3332c-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="3332c-136">Response</span></span>
<span data-ttu-id="3332c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3332c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 831

{
  "value": {
    "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
    "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
    "targetedMobileApps": [
      "Targeted Mobile Apps value"
    ],
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
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





