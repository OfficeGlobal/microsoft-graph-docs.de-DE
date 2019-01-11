---
title: Abrufen von „iosManagedAppRegistration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs iosManagedAppRegistration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5365d6d653ce35fd1ffedc857abcd098a0c8b5b3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821952"
---
# <a name="get-iosmanagedappregistration"></a><span data-ttu-id="b5b22-103">Abrufen von „iosManagedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="b5b22-103">Get iosManagedAppRegistration</span></span>

> <span data-ttu-id="b5b22-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b5b22-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b5b22-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b5b22-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b5b22-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b5b22-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5b22-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="b5b22-107">Read properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b5b22-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b5b22-108">Prerequisites</span></span>
<span data-ttu-id="b5b22-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5b22-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5b22-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b5b22-111">Permission type</span></span>|<span data-ttu-id="b5b22-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b5b22-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5b22-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b5b22-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b5b22-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5b22-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b5b22-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b5b22-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5b22-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b5b22-116">Not supported.</span></span>|
|<span data-ttu-id="b5b22-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b5b22-117">Application</span></span>|<span data-ttu-id="b5b22-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b5b22-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5b22-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5b22-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b5b22-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b5b22-120">Optional query parameters</span></span>
<span data-ttu-id="b5b22-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b5b22-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b5b22-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b5b22-122">Request headers</span></span>
|<span data-ttu-id="b5b22-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b5b22-123">Header</span></span>|<span data-ttu-id="b5b22-124">Wert</span><span class="sxs-lookup"><span data-stu-id="b5b22-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5b22-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5b22-125">Authorization</span></span>|<span data-ttu-id="b5b22-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5b22-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5b22-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b5b22-127">Accept</span></span>|<span data-ttu-id="b5b22-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b5b22-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5b22-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b5b22-129">Request body</span></span>
<span data-ttu-id="b5b22-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b5b22-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5b22-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5b22-131">Response</span></span>
<span data-ttu-id="b5b22-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b5b22-132">If successful, this method returns a `200 OK` response code and [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5b22-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b5b22-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="b5b22-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5b22-134">Request</span></span>
<span data-ttu-id="b5b22-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b5b22-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="b5b22-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5b22-136">Response</span></span>
<span data-ttu-id="b5b22-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b5b22-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1000

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
    "managedDeviceId": "Managed Device Id value",
    "azureADDeviceId": "Azure ADDevice Id value",
    "deviceModel": "Device Model value",
    "deviceManufacturer": "Device Manufacturer value",
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





