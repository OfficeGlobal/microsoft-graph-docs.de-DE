---
title: Auflisten von „deviceEnrollmentConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceEnrollmentConfiguration auf.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8f5649cbe7b46c69e0e9408c7d724088ada27ac6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864617"
---
# <a name="list-deviceenrollmentconfigurations"></a><span data-ttu-id="a9c24-103">Auflisten von „deviceEnrollmentConfiguration“</span><span class="sxs-lookup"><span data-stu-id="a9c24-103">List deviceEnrollmentConfigurations</span></span>

> <span data-ttu-id="a9c24-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a9c24-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a9c24-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="a9c24-105">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a9c24-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a9c24-106">Prerequisites</span></span>
<span data-ttu-id="a9c24-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9c24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9c24-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a9c24-109">Permission type</span></span>|<span data-ttu-id="a9c24-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a9c24-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9c24-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a9c24-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a9c24-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9c24-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a9c24-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a9c24-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9c24-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a9c24-114">Not supported.</span></span>|
|<span data-ttu-id="a9c24-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a9c24-115">Application</span></span>|<span data-ttu-id="a9c24-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a9c24-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9c24-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a9c24-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a9c24-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a9c24-118">Request headers</span></span>
|<span data-ttu-id="a9c24-119">Header</span><span class="sxs-lookup"><span data-stu-id="a9c24-119">Header</span></span>|<span data-ttu-id="a9c24-120">Wert</span><span class="sxs-lookup"><span data-stu-id="a9c24-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9c24-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9c24-121">Authorization</span></span>|<span data-ttu-id="a9c24-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a9c24-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9c24-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a9c24-123">Accept</span></span>|<span data-ttu-id="a9c24-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a9c24-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9c24-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a9c24-125">Request body</span></span>
<span data-ttu-id="a9c24-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a9c24-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9c24-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="a9c24-127">Response</span></span>
<span data-ttu-id="a9c24-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a9c24-128">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9c24-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a9c24-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="a9c24-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a9c24-130">Request</span></span>
<span data-ttu-id="a9c24-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a9c24-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="a9c24-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="a9c24-132">Response</span></span>
<span data-ttu-id="a9c24-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a9c24-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 422

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
      "id": "df13d8b9-d8b9-df13-b9d8-13dfb9d813df",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7
    }
  ]
}
```



