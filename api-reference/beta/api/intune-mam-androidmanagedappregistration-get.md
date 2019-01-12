---
title: Abrufen von „androidManagedAppRegistration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs androidManagedAppRegistration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f88bf1531d137bc7c22443f60237c1ae8519e765
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924335"
---
# <a name="get-androidmanagedappregistration"></a><span data-ttu-id="4c97d-103">Abrufen von „androidManagedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="4c97d-103">Get androidManagedAppRegistration</span></span>

> <span data-ttu-id="4c97d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4c97d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c97d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4c97d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4c97d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4c97d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c97d-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="4c97d-107">Read properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4c97d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4c97d-108">Prerequisites</span></span>
<span data-ttu-id="4c97d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c97d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c97d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4c97d-111">Permission type</span></span>|<span data-ttu-id="4c97d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4c97d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c97d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4c97d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4c97d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c97d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4c97d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4c97d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c97d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4c97d-116">Not supported.</span></span>|
|<span data-ttu-id="4c97d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4c97d-117">Application</span></span>|<span data-ttu-id="4c97d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4c97d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c97d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4c97d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4c97d-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4c97d-120">Optional query parameters</span></span>
<span data-ttu-id="4c97d-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4c97d-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4c97d-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4c97d-122">Request headers</span></span>
|<span data-ttu-id="4c97d-123">Header</span><span class="sxs-lookup"><span data-stu-id="4c97d-123">Header</span></span>|<span data-ttu-id="4c97d-124">Wert</span><span class="sxs-lookup"><span data-stu-id="4c97d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c97d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c97d-125">Authorization</span></span>|<span data-ttu-id="4c97d-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4c97d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c97d-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4c97d-127">Accept</span></span>|<span data-ttu-id="4c97d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4c97d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c97d-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4c97d-129">Request body</span></span>
<span data-ttu-id="4c97d-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4c97d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c97d-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="4c97d-131">Response</span></span>
<span data-ttu-id="4c97d-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4c97d-132">If successful, this method returns a `200 OK` response code and [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c97d-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4c97d-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="4c97d-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4c97d-134">Request</span></span>
<span data-ttu-id="4c97d-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4c97d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="4c97d-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="4c97d-136">Response</span></span>
<span data-ttu-id="4c97d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4c97d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1010

{
  "value": {
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
}
```





