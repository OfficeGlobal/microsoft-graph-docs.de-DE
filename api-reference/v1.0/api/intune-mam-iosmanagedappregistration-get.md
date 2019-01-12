---
title: Abrufen von „iosManagedAppRegistration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs iosManagedAppRegistration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d2c9c9144be60b0832c8f0f42198f4060265886f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958523"
---
# <a name="get-iosmanagedappregistration"></a><span data-ttu-id="891d8-103">Abrufen von „iosManagedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="891d8-103">Get iosManagedAppRegistration</span></span>

> <span data-ttu-id="891d8-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="891d8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="891d8-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="891d8-105">Read properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="891d8-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="891d8-106">Prerequisites</span></span>
<span data-ttu-id="891d8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="891d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="891d8-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="891d8-109">Permission type</span></span>|<span data-ttu-id="891d8-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="891d8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="891d8-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="891d8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="891d8-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="891d8-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="891d8-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="891d8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="891d8-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="891d8-114">Not supported.</span></span>|
|<span data-ttu-id="891d8-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="891d8-115">Application</span></span>|<span data-ttu-id="891d8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="891d8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="891d8-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="891d8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="891d8-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="891d8-118">Optional query parameters</span></span>
<span data-ttu-id="891d8-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="891d8-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="891d8-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="891d8-120">Request headers</span></span>
|<span data-ttu-id="891d8-121">Header</span><span class="sxs-lookup"><span data-stu-id="891d8-121">Header</span></span>|<span data-ttu-id="891d8-122">Wert</span><span class="sxs-lookup"><span data-stu-id="891d8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="891d8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="891d8-123">Authorization</span></span>|<span data-ttu-id="891d8-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="891d8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="891d8-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="891d8-125">Accept</span></span>|<span data-ttu-id="891d8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="891d8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="891d8-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="891d8-127">Request body</span></span>
<span data-ttu-id="891d8-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="891d8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="891d8-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="891d8-129">Response</span></span>
<span data-ttu-id="891d8-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="891d8-130">If successful, this method returns a `200 OK` response code and [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="891d8-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="891d8-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="891d8-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="891d8-132">Request</span></span>
<span data-ttu-id="891d8-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="891d8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="891d8-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="891d8-134">Response</span></span>
<span data-ttu-id="891d8-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="891d8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 800

{
  "value": {
    "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "applicationVersion": "Application Version value",
    "managementSdkVersion": "Management Sdk Version value",
    "platformVersion": "Platform Version value",
    "deviceType": "Device Type value",
    "deviceTag": "Device Tag value",
    "deviceName": "Device Name value",
    "flaggedReasons": [
      "rootedDevice"
    ],
    "userId": "User Id value",
    "appIdentifier": {
      "@odata.type": "microsoft.graph.iosMobileAppIdentifier",
      "bundleId": "Bundle Id value"
    },
    "id": "47632c19-2c19-4763-192c-6347192c6347",
    "version": "Version value"
  }
}
```



