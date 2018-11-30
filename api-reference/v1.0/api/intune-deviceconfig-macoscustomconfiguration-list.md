---
title: Auflisten von „macOSCustomConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs macOSCustomConfiguration auf.
ms.openlocfilehash: 7200906df6beeddbf544c7e697dc84213063d9ba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018367"
---
# <a name="list-macoscustomconfigurations"></a><span data-ttu-id="c1247-103">Auflisten von „macOSCustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="c1247-103">List macOSCustomConfigurations</span></span>

> <span data-ttu-id="c1247-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c1247-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1247-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="c1247-105">List properties and relationships of the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c1247-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c1247-106">Prerequisites</span></span>
<span data-ttu-id="c1247-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1247-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1247-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c1247-109">Permission type</span></span>|<span data-ttu-id="c1247-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c1247-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1247-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c1247-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c1247-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1247-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c1247-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c1247-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1247-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1247-114">Not supported.</span></span>|
|<span data-ttu-id="c1247-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c1247-115">Application</span></span>|<span data-ttu-id="c1247-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1247-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1247-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1247-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c1247-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c1247-118">Request headers</span></span>
|<span data-ttu-id="c1247-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c1247-119">Header</span></span>|<span data-ttu-id="c1247-120">Wert</span><span class="sxs-lookup"><span data-stu-id="c1247-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1247-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1247-121">Authorization</span></span>|<span data-ttu-id="c1247-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c1247-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1247-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c1247-123">Accept</span></span>|<span data-ttu-id="c1247-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c1247-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1247-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c1247-125">Request body</span></span>
<span data-ttu-id="c1247-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c1247-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1247-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1247-127">Response</span></span>
<span data-ttu-id="c1247-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c1247-128">If successful, this method returns a `200 OK` response code and a collection of [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1247-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c1247-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="c1247-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1247-130">Request</span></span>
<span data-ttu-id="c1247-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c1247-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="c1247-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1247-132">Response</span></span>
<span data-ttu-id="c1247-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c1247-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 526

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
      "id": "a253835d-835d-a253-5d83-53a25d8353a2",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "payloadName": "Payload Name value",
      "payloadFileName": "Payload File Name value",
      "payload": "cGF5bG9hZA=="
    }
  ]
}
```



