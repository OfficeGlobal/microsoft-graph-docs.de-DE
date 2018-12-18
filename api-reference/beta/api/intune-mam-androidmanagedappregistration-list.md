---
title: Auflisten von „androidManagedAppRegistration“
description: Auflisten von Eigenschaften und Beziehungen der androidManagedAppRegistration-Objekte.
author: tfitzmac
ms.openlocfilehash: b3e3839ac84133c8213582429e9826cf1af2d249
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337394"
---
# <a name="list-androidmanagedappregistrations"></a><span data-ttu-id="0a0ac-103">Auflisten von „androidManagedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="0a0ac-103">List androidManagedAppRegistrations</span></span>

> <span data-ttu-id="0a0ac-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0a0ac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a0ac-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0a0ac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a0ac-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0a0ac-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a0ac-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="0a0ac-107">List properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0a0ac-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0a0ac-108">Prerequisites</span></span>
<span data-ttu-id="0a0ac-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a0ac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a0ac-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0a0ac-111">Permission type</span></span>|<span data-ttu-id="0a0ac-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0a0ac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a0ac-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0a0ac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0a0ac-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a0ac-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0a0ac-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0a0ac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a0ac-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0a0ac-116">Not supported.</span></span>|
|<span data-ttu-id="0a0ac-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0a0ac-117">Application</span></span>|<span data-ttu-id="0a0ac-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0a0ac-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a0ac-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0a0ac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="0a0ac-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0a0ac-120">Request headers</span></span>
|<span data-ttu-id="0a0ac-121">Header</span><span class="sxs-lookup"><span data-stu-id="0a0ac-121">Header</span></span>|<span data-ttu-id="0a0ac-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0a0ac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a0ac-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0a0ac-123">Authorization</span></span>|<span data-ttu-id="0a0ac-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a0ac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a0ac-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0a0ac-125">Accept</span></span>|<span data-ttu-id="0a0ac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0a0ac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a0ac-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0a0ac-127">Request body</span></span>
<span data-ttu-id="0a0ac-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0a0ac-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a0ac-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="0a0ac-129">Response</span></span>
<span data-ttu-id="0a0ac-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0a0ac-130">If successful, this method returns a `200 OK` response code and a collection of [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a0ac-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0a0ac-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="0a0ac-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0a0ac-132">Request</span></span>
<span data-ttu-id="0a0ac-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0a0ac-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="0a0ac-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="0a0ac-134">Response</span></span>
<span data-ttu-id="0a0ac-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0a0ac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1070

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "applicationVersion": "Application Version value",
      "managementSdkVersion": "Management Sdk Version value",
      "platformVersion": "Platform Version value",
      "deviceType": "Device Type value",
      "deviceTag": "Device Tag value",
      "deviceName": "Device Name value",
      "managedDeviceId": "Managed Device Id value",
      "azureADDeviceId": "Azure ADDevice Id value",
      "deviceModel": "Device Model value",
      "deviceManufacturer": "Device Manufacturer value",
      "flaggedReasons": [
        "rootedDevice"
      ],
      "userId": "User Id value",
      "appIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "Package Id value"
      },
      "id": "0e064997-4997-0e06-9749-060e9749060e",
      "version": "Version value"
    }
  ]
}
```





