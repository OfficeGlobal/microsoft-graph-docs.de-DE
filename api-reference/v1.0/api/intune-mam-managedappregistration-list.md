---
title: Auflisten von „managedAppRegistration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs managedAppRegistration auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 94738c4b0aef555a536ceec2533db241007251a4
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975308"
---
# <a name="list-managedappregistrations"></a><span data-ttu-id="11e34-103">Auflisten von „managedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="11e34-103">List managedAppRegistrations</span></span>

> <span data-ttu-id="11e34-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="11e34-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11e34-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="11e34-105">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11e34-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="11e34-106">Prerequisites</span></span>
<span data-ttu-id="11e34-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11e34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11e34-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="11e34-109">Permission type</span></span>|<span data-ttu-id="11e34-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="11e34-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11e34-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="11e34-111">Delegated (work or school account)</span></span>|<span data-ttu-id="11e34-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="11e34-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="11e34-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="11e34-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11e34-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="11e34-114">Not supported.</span></span>|
|<span data-ttu-id="11e34-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="11e34-115">Application</span></span>|<span data-ttu-id="11e34-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="11e34-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11e34-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="11e34-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="11e34-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="11e34-118">Request headers</span></span>
|<span data-ttu-id="11e34-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="11e34-119">Header</span></span>|<span data-ttu-id="11e34-120">Wert</span><span class="sxs-lookup"><span data-stu-id="11e34-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11e34-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="11e34-121">Authorization</span></span>|<span data-ttu-id="11e34-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="11e34-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11e34-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="11e34-123">Accept</span></span>|<span data-ttu-id="11e34-124">application/json</span><span class="sxs-lookup"><span data-stu-id="11e34-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11e34-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="11e34-125">Request body</span></span>
<span data-ttu-id="11e34-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="11e34-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11e34-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="11e34-127">Response</span></span>
<span data-ttu-id="11e34-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="11e34-128">If successful, this method returns a `200 OK` response code and a collection of [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11e34-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="11e34-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="11e34-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="11e34-130">Request</span></span>
<span data-ttu-id="11e34-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="11e34-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="11e34-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="11e34-132">Response</span></span>
<span data-ttu-id="11e34-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="11e34-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 806

{
  "value": [
    {
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
  ]
}
```



