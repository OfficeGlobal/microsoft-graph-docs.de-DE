---
title: Auflisten von „iosManagedAppRegistration“
description: Listet die Eigenschaften und Beziehungen von Objekten des Typs iosManagedAppRegistration auf.
ms.openlocfilehash: 6827b2c846fd2695aa9e9a6c60c80b61851745c7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017645"
---
# <a name="list-iosmanagedappregistrations"></a><span data-ttu-id="35bd5-103">Auflisten von „iosManagedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="35bd5-103">List iosManagedAppRegistrations</span></span>

> <span data-ttu-id="35bd5-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="35bd5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="35bd5-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="35bd5-105">List properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="35bd5-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="35bd5-106">Prerequisites</span></span>
<span data-ttu-id="35bd5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35bd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35bd5-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="35bd5-109">Permission type</span></span>|<span data-ttu-id="35bd5-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="35bd5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35bd5-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="35bd5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="35bd5-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="35bd5-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="35bd5-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="35bd5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35bd5-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="35bd5-114">Not supported.</span></span>|
|<span data-ttu-id="35bd5-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="35bd5-115">Application</span></span>|<span data-ttu-id="35bd5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="35bd5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35bd5-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="35bd5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="35bd5-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="35bd5-118">Request headers</span></span>
|<span data-ttu-id="35bd5-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="35bd5-119">Header</span></span>|<span data-ttu-id="35bd5-120">Wert</span><span class="sxs-lookup"><span data-stu-id="35bd5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35bd5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="35bd5-121">Authorization</span></span>|<span data-ttu-id="35bd5-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="35bd5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35bd5-123">Accept</span><span class="sxs-lookup"><span data-stu-id="35bd5-123">Accept</span></span>|<span data-ttu-id="35bd5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="35bd5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35bd5-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="35bd5-125">Request body</span></span>
<span data-ttu-id="35bd5-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="35bd5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35bd5-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="35bd5-127">Response</span></span>
<span data-ttu-id="35bd5-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="35bd5-128">If successful, this method returns a `200 OK` response code and a collection of [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35bd5-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="35bd5-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="35bd5-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="35bd5-130">Request</span></span>
<span data-ttu-id="35bd5-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="35bd5-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="35bd5-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="35bd5-132">Response</span></span>
<span data-ttu-id="35bd5-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="35bd5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 852

{
  "value": [
    {
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
  ]
}
```



