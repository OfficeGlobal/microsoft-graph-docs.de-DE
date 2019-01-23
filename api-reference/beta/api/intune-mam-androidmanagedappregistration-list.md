---
title: Auflisten von „androidManagedAppRegistration“
description: Auflisten von Eigenschaften und Beziehungen der androidManagedAppRegistration-Objekte.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8fb7abfba70411569e8ad0295fcb9b1adc47430b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411253"
---
# <a name="list-androidmanagedappregistrations"></a><span data-ttu-id="63e85-103">Auflisten von „androidManagedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="63e85-103">List androidManagedAppRegistrations</span></span>

> <span data-ttu-id="63e85-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="63e85-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="63e85-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="63e85-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63e85-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="63e85-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63e85-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="63e85-107">List properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63e85-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="63e85-108">Prerequisites</span></span>
<span data-ttu-id="63e85-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="63e85-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="63e85-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="63e85-111">Permission type</span></span>|<span data-ttu-id="63e85-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="63e85-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63e85-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="63e85-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63e85-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="63e85-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="63e85-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="63e85-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63e85-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="63e85-116">Not supported.</span></span>|
|<span data-ttu-id="63e85-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="63e85-117">Application</span></span>|<span data-ttu-id="63e85-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="63e85-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63e85-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="63e85-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="63e85-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="63e85-120">Request headers</span></span>
|<span data-ttu-id="63e85-121">Header</span><span class="sxs-lookup"><span data-stu-id="63e85-121">Header</span></span>|<span data-ttu-id="63e85-122">Wert</span><span class="sxs-lookup"><span data-stu-id="63e85-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63e85-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="63e85-123">Authorization</span></span>|<span data-ttu-id="63e85-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="63e85-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63e85-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="63e85-125">Accept</span></span>|<span data-ttu-id="63e85-126">application/json</span><span class="sxs-lookup"><span data-stu-id="63e85-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63e85-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="63e85-127">Request body</span></span>
<span data-ttu-id="63e85-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="63e85-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63e85-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="63e85-129">Response</span></span>
<span data-ttu-id="63e85-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="63e85-130">If successful, this method returns a `200 OK` response code and a collection of [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63e85-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="63e85-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="63e85-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="63e85-132">Request</span></span>
<span data-ttu-id="63e85-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="63e85-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="63e85-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="63e85-134">Response</span></span>
<span data-ttu-id="63e85-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="63e85-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1116

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
      "version": "Version value",
      "patchVersion": "Patch Version value"
    }
  ]
}
```




