---
title: Abrufen von „deviceConfiguration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs deviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ee502af04c1e00edd37ade9f8f29b5b27320f940
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884294"
---
# <a name="get-deviceconfiguration"></a><span data-ttu-id="50881-103">Abrufen von „deviceConfiguration“</span><span class="sxs-lookup"><span data-stu-id="50881-103">Get deviceConfiguration</span></span>

> <span data-ttu-id="50881-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="50881-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="50881-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="50881-105">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="50881-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="50881-106">Prerequisites</span></span>
<span data-ttu-id="50881-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50881-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50881-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="50881-109">Permission type</span></span>|<span data-ttu-id="50881-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="50881-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50881-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="50881-111">Delegated (work or school account)</span></span>|<span data-ttu-id="50881-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="50881-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="50881-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="50881-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50881-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50881-114">Not supported.</span></span>|
|<span data-ttu-id="50881-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="50881-115">Application</span></span>|<span data-ttu-id="50881-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50881-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50881-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="50881-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="50881-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="50881-118">Optional query parameters</span></span>
<span data-ttu-id="50881-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="50881-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="50881-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="50881-120">Request headers</span></span>
|<span data-ttu-id="50881-121">Header</span><span class="sxs-lookup"><span data-stu-id="50881-121">Header</span></span>|<span data-ttu-id="50881-122">Wert</span><span class="sxs-lookup"><span data-stu-id="50881-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50881-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="50881-123">Authorization</span></span>|<span data-ttu-id="50881-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="50881-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50881-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="50881-125">Accept</span></span>|<span data-ttu-id="50881-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50881-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50881-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="50881-127">Request body</span></span>
<span data-ttu-id="50881-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="50881-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50881-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="50881-129">Response</span></span>
<span data-ttu-id="50881-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="50881-130">If successful, this method returns a `200 OK` response code and [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50881-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="50881-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="50881-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="50881-132">Request</span></span>
<span data-ttu-id="50881-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="50881-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="50881-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="50881-134">Response</span></span>
<span data-ttu-id="50881-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="50881-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 362

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfiguration",
    "id": "34977265-7265-3497-6572-973465729734",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7
  }
}
```



