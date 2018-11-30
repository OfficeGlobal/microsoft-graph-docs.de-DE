---
title: Auflisten von „windows10CustomConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs windows10CustomConfiguration auf.
ms.openlocfilehash: 34a59b3fb2f0c83568ea79b16c5c913ef5e9a742
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019375"
---
# <a name="list-windows10customconfigurations"></a><span data-ttu-id="2cb4f-103">Auflisten von „windows10CustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="2cb4f-103">List windows10CustomConfigurations</span></span>

> <span data-ttu-id="2cb4f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2cb4f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2cb4f-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="2cb4f-105">List properties and relationships of the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2cb4f-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2cb4f-106">Prerequisites</span></span>
<span data-ttu-id="2cb4f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cb4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cb4f-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2cb4f-109">Permission type</span></span>|<span data-ttu-id="2cb4f-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2cb4f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2cb4f-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2cb4f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2cb4f-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2cb4f-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2cb4f-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2cb4f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2cb4f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2cb4f-114">Not supported.</span></span>|
|<span data-ttu-id="2cb4f-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2cb4f-115">Application</span></span>|<span data-ttu-id="2cb4f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2cb4f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2cb4f-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2cb4f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2cb4f-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2cb4f-118">Request headers</span></span>
|<span data-ttu-id="2cb4f-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2cb4f-119">Header</span></span>|<span data-ttu-id="2cb4f-120">Wert</span><span class="sxs-lookup"><span data-stu-id="2cb4f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2cb4f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2cb4f-121">Authorization</span></span>|<span data-ttu-id="2cb4f-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2cb4f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2cb4f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2cb4f-123">Accept</span></span>|<span data-ttu-id="2cb4f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2cb4f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cb4f-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2cb4f-125">Request body</span></span>
<span data-ttu-id="2cb4f-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2cb4f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2cb4f-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="2cb4f-127">Response</span></span>
<span data-ttu-id="2cb4f-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2cb4f-128">If successful, this method returns a `200 OK` response code and a collection of [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2cb4f-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2cb4f-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="2cb4f-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2cb4f-130">Request</span></span>
<span data-ttu-id="2cb4f-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2cb4f-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="2cb4f-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="2cb4f-132">Response</span></span>
<span data-ttu-id="2cb4f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2cb4f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 673

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
      "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
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



