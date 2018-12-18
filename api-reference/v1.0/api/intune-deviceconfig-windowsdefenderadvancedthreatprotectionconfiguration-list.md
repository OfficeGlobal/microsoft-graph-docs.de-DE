---
title: Auflisten von „windowsDefenderAdvancedThreatProtectionConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs windowsDefenderAdvancedThreatProtectionConfiguration auf.
author: tfitzmac
ms.openlocfilehash: 8a1214cfe215e8db9e0c8e1c209987e045b45940
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316996"
---
# <a name="list-windowsdefenderadvancedthreatprotectionconfigurations"></a><span data-ttu-id="5ace8-103">Auflisten von „windowsDefenderAdvancedThreatProtectionConfiguration“</span><span class="sxs-lookup"><span data-stu-id="5ace8-103">List windowsDefenderAdvancedThreatProtectionConfigurations</span></span>

> <span data-ttu-id="5ace8-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5ace8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5ace8-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="5ace8-105">List properties and relationships of the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5ace8-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5ace8-106">Prerequisites</span></span>
<span data-ttu-id="5ace8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ace8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ace8-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5ace8-109">Permission type</span></span>|<span data-ttu-id="5ace8-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5ace8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ace8-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5ace8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5ace8-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ace8-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5ace8-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5ace8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ace8-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5ace8-114">Not supported.</span></span>|
|<span data-ttu-id="5ace8-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5ace8-115">Application</span></span>|<span data-ttu-id="5ace8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5ace8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ace8-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5ace8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5ace8-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5ace8-118">Request headers</span></span>
|<span data-ttu-id="5ace8-119">Header</span><span class="sxs-lookup"><span data-stu-id="5ace8-119">Header</span></span>|<span data-ttu-id="5ace8-120">Wert</span><span class="sxs-lookup"><span data-stu-id="5ace8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ace8-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="5ace8-121">Authorization</span></span>|<span data-ttu-id="5ace8-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5ace8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ace8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5ace8-123">Accept</span></span>|<span data-ttu-id="5ace8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5ace8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ace8-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5ace8-125">Request body</span></span>
<span data-ttu-id="5ace8-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5ace8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ace8-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="5ace8-127">Response</span></span>
<span data-ttu-id="5ace8-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5ace8-128">If successful, this method returns a `200 OK` response code and a collection of [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ace8-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5ace8-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="5ace8-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5ace8-130">Request</span></span>
<span data-ttu-id="5ace8-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5ace8-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="5ace8-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="5ace8-132">Response</span></span>
<span data-ttu-id="5ace8-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5ace8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 508

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
      "id": "294373aa-73aa-2943-aa73-4329aa734329",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "allowSampleSharing": true,
      "enableExpeditedTelemetryReporting": true
    }
  ]
}
```



