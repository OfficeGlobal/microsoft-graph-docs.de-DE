---
title: Auflisten von „iosUpdateConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs iosUpdateConfiguration auf.
author: tfitzmac
ms.openlocfilehash: 31e8cbee1f9c39633386786a66f90b74915920a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329988"
---
# <a name="list-iosupdateconfigurations"></a><span data-ttu-id="f670a-103">Auflisten von „iosUpdateConfiguration“</span><span class="sxs-lookup"><span data-stu-id="f670a-103">List iosUpdateConfigurations</span></span>

> <span data-ttu-id="f670a-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f670a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f670a-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="f670a-105">List properties and relationships of the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f670a-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f670a-106">Prerequisites</span></span>
<span data-ttu-id="f670a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f670a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f670a-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f670a-109">Permission type</span></span>|<span data-ttu-id="f670a-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f670a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f670a-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f670a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f670a-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f670a-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f670a-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f670a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f670a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f670a-114">Not supported.</span></span>|
|<span data-ttu-id="f670a-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f670a-115">Application</span></span>|<span data-ttu-id="f670a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f670a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f670a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f670a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f670a-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f670a-118">Request headers</span></span>
|<span data-ttu-id="f670a-119">Header</span><span class="sxs-lookup"><span data-stu-id="f670a-119">Header</span></span>|<span data-ttu-id="f670a-120">Wert</span><span class="sxs-lookup"><span data-stu-id="f670a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f670a-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f670a-121">Authorization</span></span>|<span data-ttu-id="f670a-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f670a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f670a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f670a-123">Accept</span></span>|<span data-ttu-id="f670a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f670a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f670a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f670a-125">Request body</span></span>
<span data-ttu-id="f670a-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f670a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f670a-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="f670a-127">Response</span></span>
<span data-ttu-id="f670a-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f670a-128">If successful, this method returns a `200 OK` response code and a collection of [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f670a-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f670a-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="f670a-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f670a-130">Request</span></span>
<span data-ttu-id="f670a-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f670a-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="f670a-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="f670a-132">Response</span></span>
<span data-ttu-id="f670a-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f670a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 582

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
      "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "activeHoursStart": "12:00:05.5020000",
      "activeHoursEnd": "11:59:00.8990000",
      "scheduledInstallDays": [
        "monday"
      ],
      "utcTimeOffsetInMinutes": 6
    }
  ]
}
```



