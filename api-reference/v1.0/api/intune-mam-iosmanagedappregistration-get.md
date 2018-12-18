---
title: Abrufen von „iosManagedAppRegistration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs iosManagedAppRegistration.
author: tfitzmac
ms.openlocfilehash: 0199362bdc92db6ed45f44a28b135327b1cb9a94
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351632"
---
# <a name="get-iosmanagedappregistration"></a><span data-ttu-id="c70f3-103">Abrufen von „iosManagedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="c70f3-103">Get iosManagedAppRegistration</span></span>

> <span data-ttu-id="c70f3-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c70f3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c70f3-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="c70f3-105">Read properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c70f3-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c70f3-106">Prerequisites</span></span>
<span data-ttu-id="c70f3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c70f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c70f3-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c70f3-109">Permission type</span></span>|<span data-ttu-id="c70f3-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c70f3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c70f3-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c70f3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c70f3-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c70f3-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c70f3-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c70f3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c70f3-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c70f3-114">Not supported.</span></span>|
|<span data-ttu-id="c70f3-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c70f3-115">Application</span></span>|<span data-ttu-id="c70f3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c70f3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c70f3-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c70f3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c70f3-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c70f3-118">Optional query parameters</span></span>
<span data-ttu-id="c70f3-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c70f3-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c70f3-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c70f3-120">Request headers</span></span>
|<span data-ttu-id="c70f3-121">Header</span><span class="sxs-lookup"><span data-stu-id="c70f3-121">Header</span></span>|<span data-ttu-id="c70f3-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c70f3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c70f3-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c70f3-123">Authorization</span></span>|<span data-ttu-id="c70f3-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c70f3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c70f3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c70f3-125">Accept</span></span>|<span data-ttu-id="c70f3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c70f3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c70f3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c70f3-127">Request body</span></span>
<span data-ttu-id="c70f3-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c70f3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c70f3-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="c70f3-129">Response</span></span>
<span data-ttu-id="c70f3-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c70f3-130">If successful, this method returns a `200 OK` response code and [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c70f3-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c70f3-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c70f3-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c70f3-132">Request</span></span>
<span data-ttu-id="c70f3-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c70f3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="c70f3-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c70f3-134">Response</span></span>
<span data-ttu-id="c70f3-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c70f3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



