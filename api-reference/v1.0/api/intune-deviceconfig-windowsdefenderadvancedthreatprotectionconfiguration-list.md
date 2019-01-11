---
title: Auflisten von „windowsDefenderAdvancedThreatProtectionConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs windowsDefenderAdvancedThreatProtectionConfiguration auf.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d8a9b6461431281db63b93017748d6b7b2c6bd27
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826411"
---
# <a name="list-windowsdefenderadvancedthreatprotectionconfigurations"></a><span data-ttu-id="31ba4-103">Auflisten von „windowsDefenderAdvancedThreatProtectionConfiguration“</span><span class="sxs-lookup"><span data-stu-id="31ba4-103">List windowsDefenderAdvancedThreatProtectionConfigurations</span></span>

> <span data-ttu-id="31ba4-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="31ba4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31ba4-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="31ba4-105">List properties and relationships of the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="31ba4-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="31ba4-106">Prerequisites</span></span>
<span data-ttu-id="31ba4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31ba4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31ba4-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="31ba4-109">Permission type</span></span>|<span data-ttu-id="31ba4-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="31ba4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31ba4-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="31ba4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="31ba4-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="31ba4-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="31ba4-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="31ba4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31ba4-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="31ba4-114">Not supported.</span></span>|
|<span data-ttu-id="31ba4-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="31ba4-115">Application</span></span>|<span data-ttu-id="31ba4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="31ba4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31ba4-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="31ba4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="31ba4-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="31ba4-118">Request headers</span></span>
|<span data-ttu-id="31ba4-119">Header</span><span class="sxs-lookup"><span data-stu-id="31ba4-119">Header</span></span>|<span data-ttu-id="31ba4-120">Wert</span><span class="sxs-lookup"><span data-stu-id="31ba4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31ba4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="31ba4-121">Authorization</span></span>|<span data-ttu-id="31ba4-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="31ba4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31ba4-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="31ba4-123">Accept</span></span>|<span data-ttu-id="31ba4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="31ba4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31ba4-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="31ba4-125">Request body</span></span>
<span data-ttu-id="31ba4-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="31ba4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31ba4-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="31ba4-127">Response</span></span>
<span data-ttu-id="31ba4-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="31ba4-128">If successful, this method returns a `200 OK` response code and a collection of [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31ba4-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="31ba4-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="31ba4-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="31ba4-130">Request</span></span>
<span data-ttu-id="31ba4-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="31ba4-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="31ba4-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="31ba4-132">Response</span></span>
<span data-ttu-id="31ba4-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="31ba4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



