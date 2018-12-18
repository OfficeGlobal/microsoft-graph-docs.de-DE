---
title: Auflisten von „windowsPhone81CustomConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs windowsPhone81CustomConfiguration auf.
author: tfitzmac
ms.openlocfilehash: 0c12126afc281ee3f0fb3dec6047d5350ee66f00
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315589"
---
# <a name="list-windowsphone81customconfigurations"></a><span data-ttu-id="e6ae2-103">Auflisten von „windowsPhone81CustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="e6ae2-103">List windowsPhone81CustomConfigurations</span></span>

> <span data-ttu-id="e6ae2-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e6ae2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e6ae2-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="e6ae2-105">List properties and relationships of the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e6ae2-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e6ae2-106">Prerequisites</span></span>
<span data-ttu-id="e6ae2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6ae2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6ae2-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e6ae2-109">Permission type</span></span>|<span data-ttu-id="e6ae2-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e6ae2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6ae2-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e6ae2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e6ae2-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6ae2-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e6ae2-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e6ae2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6ae2-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e6ae2-114">Not supported.</span></span>|
|<span data-ttu-id="e6ae2-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e6ae2-115">Application</span></span>|<span data-ttu-id="e6ae2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e6ae2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6ae2-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e6ae2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e6ae2-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e6ae2-118">Request headers</span></span>
|<span data-ttu-id="e6ae2-119">Header</span><span class="sxs-lookup"><span data-stu-id="e6ae2-119">Header</span></span>|<span data-ttu-id="e6ae2-120">Wert</span><span class="sxs-lookup"><span data-stu-id="e6ae2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6ae2-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e6ae2-121">Authorization</span></span>|<span data-ttu-id="e6ae2-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e6ae2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6ae2-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e6ae2-123">Accept</span></span>|<span data-ttu-id="e6ae2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e6ae2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6ae2-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e6ae2-125">Request body</span></span>
<span data-ttu-id="e6ae2-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e6ae2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6ae2-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="e6ae2-127">Response</span></span>
<span data-ttu-id="e6ae2-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e6ae2-128">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6ae2-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e6ae2-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="e6ae2-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e6ae2-130">Request</span></span>
<span data-ttu-id="e6ae2-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e6ae2-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="e6ae2-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="e6ae2-132">Response</span></span>
<span data-ttu-id="e6ae2-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e6ae2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 678

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
      "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "omaSettings": [
        {
          "@odata.type": "microsoft.graph.omaSettingInteger",
          "displayName": "Display Name value",
          "description": "Description value",
          "omaUri": "Oma Uri value",
          "value": 5
        }
      ]
    }
  ]
}
```



