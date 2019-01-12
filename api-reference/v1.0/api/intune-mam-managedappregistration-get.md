---
title: Abrufen von „managedAppRegistration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedAppRegistration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b044a9d2a491763d8a25f3c80538dde873094e53
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983072"
---
# <a name="get-managedappregistration"></a><span data-ttu-id="76508-103">Abrufen von „managedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="76508-103">Get managedAppRegistration</span></span>

> <span data-ttu-id="76508-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="76508-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="76508-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="76508-105">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="76508-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="76508-106">Prerequisites</span></span>
<span data-ttu-id="76508-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76508-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76508-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="76508-109">Permission type</span></span>|<span data-ttu-id="76508-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="76508-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76508-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="76508-111">Delegated (work or school account)</span></span>|<span data-ttu-id="76508-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="76508-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="76508-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="76508-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76508-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="76508-114">Not supported.</span></span>|
|<span data-ttu-id="76508-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="76508-115">Application</span></span>|<span data-ttu-id="76508-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="76508-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="76508-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="76508-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="76508-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="76508-118">Optional query parameters</span></span>
<span data-ttu-id="76508-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="76508-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="76508-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="76508-120">Request headers</span></span>
|<span data-ttu-id="76508-121">Header</span><span class="sxs-lookup"><span data-stu-id="76508-121">Header</span></span>|<span data-ttu-id="76508-122">Wert</span><span class="sxs-lookup"><span data-stu-id="76508-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76508-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="76508-123">Authorization</span></span>|<span data-ttu-id="76508-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="76508-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76508-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="76508-125">Accept</span></span>|<span data-ttu-id="76508-126">application/json</span><span class="sxs-lookup"><span data-stu-id="76508-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76508-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="76508-127">Request body</span></span>
<span data-ttu-id="76508-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="76508-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76508-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="76508-129">Response</span></span>
<span data-ttu-id="76508-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="76508-130">If successful, this method returns a `200 OK` response code and [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76508-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="76508-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="76508-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="76508-132">Request</span></span>
<span data-ttu-id="76508-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="76508-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="76508-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="76508-134">Response</span></span>
<span data-ttu-id="76508-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="76508-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 756

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



