---
title: Auflisten von „androidManagedAppRegistration“
description: Auflisten von Eigenschaften und Beziehungen der androidManagedAppRegistration-Objekte.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 21ad01c12e21f3aa1722bb921a2a59e7b8b82ebb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827006"
---
# <a name="list-androidmanagedappregistrations"></a><span data-ttu-id="69102-103">Auflisten von „androidManagedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="69102-103">List androidManagedAppRegistrations</span></span>

> <span data-ttu-id="69102-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="69102-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69102-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="69102-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="69102-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="69102-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69102-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="69102-107">List properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="69102-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="69102-108">Prerequisites</span></span>
<span data-ttu-id="69102-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69102-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69102-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="69102-111">Permission type</span></span>|<span data-ttu-id="69102-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="69102-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69102-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="69102-113">Delegated (work or school account)</span></span>|<span data-ttu-id="69102-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="69102-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="69102-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="69102-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69102-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="69102-116">Not supported.</span></span>|
|<span data-ttu-id="69102-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="69102-117">Application</span></span>|<span data-ttu-id="69102-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="69102-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69102-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="69102-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="69102-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="69102-120">Request headers</span></span>
|<span data-ttu-id="69102-121">Header</span><span class="sxs-lookup"><span data-stu-id="69102-121">Header</span></span>|<span data-ttu-id="69102-122">Wert</span><span class="sxs-lookup"><span data-stu-id="69102-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69102-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="69102-123">Authorization</span></span>|<span data-ttu-id="69102-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="69102-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69102-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="69102-125">Accept</span></span>|<span data-ttu-id="69102-126">application/json</span><span class="sxs-lookup"><span data-stu-id="69102-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69102-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="69102-127">Request body</span></span>
<span data-ttu-id="69102-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="69102-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69102-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="69102-129">Response</span></span>
<span data-ttu-id="69102-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="69102-130">If successful, this method returns a `200 OK` response code and a collection of [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69102-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="69102-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="69102-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="69102-132">Request</span></span>
<span data-ttu-id="69102-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="69102-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="69102-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="69102-134">Response</span></span>
<span data-ttu-id="69102-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="69102-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





