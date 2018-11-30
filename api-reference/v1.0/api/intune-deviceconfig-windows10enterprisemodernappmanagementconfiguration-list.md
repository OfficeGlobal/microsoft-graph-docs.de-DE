---
title: Auflisten von „windows10EnterpriseModernAppManagementConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs windows10EnterpriseModernAppManagementConfiguration auf.
ms.openlocfilehash: 0b6e2e155d9d5dbc0c1bfa3cfc95153580873f40
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018032"
---
# <a name="list-windows10enterprisemodernappmanagementconfigurations"></a><span data-ttu-id="22a37-103">Auflisten von „windows10EnterpriseModernAppManagementConfiguration“</span><span class="sxs-lookup"><span data-stu-id="22a37-103">List windows10EnterpriseModernAppManagementConfigurations</span></span>

> <span data-ttu-id="22a37-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="22a37-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22a37-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="22a37-105">List properties and relationships of the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="22a37-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="22a37-106">Prerequisites</span></span>
<span data-ttu-id="22a37-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22a37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22a37-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="22a37-109">Permission type</span></span>|<span data-ttu-id="22a37-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="22a37-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22a37-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="22a37-111">Delegated (work or school account)</span></span>|<span data-ttu-id="22a37-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="22a37-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="22a37-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="22a37-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22a37-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="22a37-114">Not supported.</span></span>|
|<span data-ttu-id="22a37-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="22a37-115">Application</span></span>|<span data-ttu-id="22a37-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="22a37-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22a37-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="22a37-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="22a37-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="22a37-118">Request headers</span></span>
|<span data-ttu-id="22a37-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="22a37-119">Header</span></span>|<span data-ttu-id="22a37-120">Wert</span><span class="sxs-lookup"><span data-stu-id="22a37-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22a37-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="22a37-121">Authorization</span></span>|<span data-ttu-id="22a37-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="22a37-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22a37-123">Accept</span><span class="sxs-lookup"><span data-stu-id="22a37-123">Accept</span></span>|<span data-ttu-id="22a37-124">application/json</span><span class="sxs-lookup"><span data-stu-id="22a37-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22a37-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="22a37-125">Request body</span></span>
<span data-ttu-id="22a37-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="22a37-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22a37-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="22a37-127">Response</span></span>
<span data-ttu-id="22a37-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="22a37-128">If successful, this method returns a `200 OK` response code and a collection of [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22a37-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="22a37-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="22a37-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="22a37-130">Request</span></span>
<span data-ttu-id="22a37-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="22a37-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="22a37-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="22a37-132">Response</span></span>
<span data-ttu-id="22a37-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="22a37-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 459

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
      "id": "d6577687-7687-d657-8776-57d6877657d6",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "uninstallBuiltInApps": true
    }
  ]
}
```



