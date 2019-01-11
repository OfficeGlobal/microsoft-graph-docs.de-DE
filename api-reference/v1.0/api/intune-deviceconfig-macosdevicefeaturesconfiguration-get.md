---
title: Abrufen von „macOSDeviceFeaturesConfiguration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs macOSDeviceFeaturesConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: dbf7fa47d46deb20f1555f9200e0e32c1f6aa654
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816627"
---
# <a name="get-macosdevicefeaturesconfiguration"></a><span data-ttu-id="f30de-103">Abrufen von „macOSDeviceFeaturesConfiguration“</span><span class="sxs-lookup"><span data-stu-id="f30de-103">Get macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="f30de-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f30de-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f30de-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f30de-105">Read properties and relationships of the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f30de-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f30de-106">Prerequisites</span></span>
<span data-ttu-id="f30de-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f30de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f30de-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f30de-109">Permission type</span></span>|<span data-ttu-id="f30de-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f30de-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f30de-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f30de-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f30de-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f30de-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f30de-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f30de-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f30de-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f30de-114">Not supported.</span></span>|
|<span data-ttu-id="f30de-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f30de-115">Application</span></span>|<span data-ttu-id="f30de-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f30de-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f30de-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f30de-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f30de-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f30de-118">Optional query parameters</span></span>
<span data-ttu-id="f30de-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f30de-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f30de-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f30de-120">Request headers</span></span>
|<span data-ttu-id="f30de-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f30de-121">Header</span></span>|<span data-ttu-id="f30de-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f30de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f30de-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f30de-123">Authorization</span></span>|<span data-ttu-id="f30de-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f30de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f30de-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f30de-125">Accept</span></span>|<span data-ttu-id="f30de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f30de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f30de-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f30de-127">Request body</span></span>
<span data-ttu-id="f30de-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f30de-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f30de-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f30de-129">Response</span></span>
<span data-ttu-id="f30de-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f30de-130">If successful, this method returns a `200 OK` response code and [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f30de-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f30de-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f30de-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f30de-132">Request</span></span>
<span data-ttu-id="f30de-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f30de-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="f30de-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f30de-134">Response</span></span>
<span data-ttu-id="f30de-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f30de-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



