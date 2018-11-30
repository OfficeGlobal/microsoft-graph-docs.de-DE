---
title: Abrufen von „managedAppRegistration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedAppRegistration.
ms.openlocfilehash: 4d852e187b7cf7f778969ff216eda836c7a8db63
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066084"
---
# <a name="get-managedappregistration"></a><span data-ttu-id="1ec30-103">Abrufen von „managedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="1ec30-103">Get managedAppRegistration</span></span>

> <span data-ttu-id="1ec30-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1ec30-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1ec30-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1ec30-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1ec30-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1ec30-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ec30-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="1ec30-107">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1ec30-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1ec30-108">Prerequisites</span></span>
<span data-ttu-id="1ec30-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ec30-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ec30-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1ec30-111">Permission type</span></span>|<span data-ttu-id="1ec30-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1ec30-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ec30-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1ec30-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1ec30-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ec30-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1ec30-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1ec30-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ec30-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1ec30-116">Not supported.</span></span>|
|<span data-ttu-id="1ec30-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1ec30-117">Application</span></span>|<span data-ttu-id="1ec30-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1ec30-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ec30-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1ec30-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1ec30-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1ec30-120">Optional query parameters</span></span>
<span data-ttu-id="1ec30-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1ec30-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1ec30-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1ec30-122">Request headers</span></span>
|<span data-ttu-id="1ec30-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1ec30-123">Header</span></span>|<span data-ttu-id="1ec30-124">Wert</span><span class="sxs-lookup"><span data-stu-id="1ec30-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ec30-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ec30-125">Authorization</span></span>|<span data-ttu-id="1ec30-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1ec30-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ec30-127">Accept</span><span class="sxs-lookup"><span data-stu-id="1ec30-127">Accept</span></span>|<span data-ttu-id="1ec30-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1ec30-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ec30-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1ec30-129">Request body</span></span>
<span data-ttu-id="1ec30-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1ec30-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ec30-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="1ec30-131">Response</span></span>
<span data-ttu-id="1ec30-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1ec30-132">If successful, this method returns a `200 OK` response code and [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ec30-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1ec30-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="1ec30-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1ec30-134">Request</span></span>
<span data-ttu-id="1ec30-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1ec30-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="1ec30-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="1ec30-136">Response</span></span>
<span data-ttu-id="1ec30-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1ec30-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 956

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppRegistration",
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
      "@odata.type": "microsoft.graph.mobileAppIdentifier"
    },
    "id": "5496aa60-aa60-5496-60aa-965460aa9654",
    "version": "Version value"
  }
}
```





