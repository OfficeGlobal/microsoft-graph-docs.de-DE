---
title: Abrufen von „macOSCustomConfiguration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs macOSCustomConfiguration.
author: tfitzmac
ms.openlocfilehash: 7f805f06bbd669b3ef82e2c487f9c7906f0065d1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348391"
---
# <a name="get-macoscustomconfiguration"></a><span data-ttu-id="9889f-103">Abrufen von „macOSCustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="9889f-103">Get macOSCustomConfiguration</span></span>

> <span data-ttu-id="9889f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9889f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9889f-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9889f-105">Read properties and relationships of the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9889f-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9889f-106">Prerequisites</span></span>
<span data-ttu-id="9889f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9889f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9889f-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9889f-109">Permission type</span></span>|<span data-ttu-id="9889f-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9889f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9889f-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9889f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9889f-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9889f-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9889f-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9889f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9889f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9889f-114">Not supported.</span></span>|
|<span data-ttu-id="9889f-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9889f-115">Application</span></span>|<span data-ttu-id="9889f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9889f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9889f-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9889f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9889f-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9889f-118">Optional query parameters</span></span>
<span data-ttu-id="9889f-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9889f-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9889f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9889f-120">Request headers</span></span>
|<span data-ttu-id="9889f-121">Header</span><span class="sxs-lookup"><span data-stu-id="9889f-121">Header</span></span>|<span data-ttu-id="9889f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="9889f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9889f-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9889f-123">Authorization</span></span>|<span data-ttu-id="9889f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9889f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9889f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9889f-125">Accept</span></span>|<span data-ttu-id="9889f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9889f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9889f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9889f-127">Request body</span></span>
<span data-ttu-id="9889f-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9889f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9889f-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="9889f-129">Response</span></span>
<span data-ttu-id="9889f-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9889f-130">If successful, this method returns a `200 OK` response code and [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9889f-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9889f-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="9889f-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9889f-132">Request</span></span>
<span data-ttu-id="9889f-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9889f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="9889f-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="9889f-134">Response</span></span>
<span data-ttu-id="9889f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9889f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 492

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
    "id": "a253835d-835d-a253-5d83-53a25d8353a2",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "payloadName": "Payload Name value",
    "payloadFileName": "Payload File Name value",
    "payload": "cGF5bG9hZA=="
  }
}
```



