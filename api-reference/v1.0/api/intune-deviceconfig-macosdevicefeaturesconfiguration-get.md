---
title: Abrufen von „macOSDeviceFeaturesConfiguration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs macOSDeviceFeaturesConfiguration.
ms.openlocfilehash: 3de61b54e5847fd7ea0e6582a3a638dd418fdbe6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019157"
---
# <a name="get-macosdevicefeaturesconfiguration"></a><span data-ttu-id="1d02c-103">Abrufen von „macOSDeviceFeaturesConfiguration“</span><span class="sxs-lookup"><span data-stu-id="1d02c-103">Get macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="1d02c-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1d02c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d02c-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d02c-105">Read properties and relationships of the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1d02c-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1d02c-106">Prerequisites</span></span>
<span data-ttu-id="1d02c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d02c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d02c-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1d02c-109">Permission type</span></span>|<span data-ttu-id="1d02c-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1d02c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d02c-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1d02c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1d02c-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d02c-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1d02c-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1d02c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d02c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1d02c-114">Not supported.</span></span>|
|<span data-ttu-id="1d02c-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1d02c-115">Application</span></span>|<span data-ttu-id="1d02c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1d02c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d02c-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1d02c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1d02c-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1d02c-118">Optional query parameters</span></span>
<span data-ttu-id="1d02c-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1d02c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1d02c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1d02c-120">Request headers</span></span>
|<span data-ttu-id="1d02c-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1d02c-121">Header</span></span>|<span data-ttu-id="1d02c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="1d02c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d02c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d02c-123">Authorization</span></span>|<span data-ttu-id="1d02c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1d02c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d02c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1d02c-125">Accept</span></span>|<span data-ttu-id="1d02c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1d02c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d02c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1d02c-127">Request body</span></span>
<span data-ttu-id="1d02c-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1d02c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d02c-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="1d02c-129">Response</span></span>
<span data-ttu-id="1d02c-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1d02c-130">If successful, this method returns a `200 OK` response code and [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d02c-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1d02c-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="1d02c-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1d02c-132">Request</span></span>
<span data-ttu-id="1d02c-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1d02c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="1d02c-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="1d02c-134">Response</span></span>
<span data-ttu-id="1d02c-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1d02c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 375

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
    "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7
  }
}
```



