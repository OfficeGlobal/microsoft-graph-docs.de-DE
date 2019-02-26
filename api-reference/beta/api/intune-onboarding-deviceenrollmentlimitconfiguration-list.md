---
title: Auflisten von „deviceEnrollmentLimitConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceEnrollmentLimitConfiguration auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 84ab33a8b53af21625ae73a894884fd7d4e3d6d2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165681"
---
# <a name="list-deviceenrollmentlimitconfigurations"></a><span data-ttu-id="8fef1-103">Auflisten von „deviceEnrollmentLimitConfiguration“</span><span class="sxs-lookup"><span data-stu-id="8fef1-103">List deviceEnrollmentLimitConfigurations</span></span>

> <span data-ttu-id="8fef1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8fef1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8fef1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8fef1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fef1-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="8fef1-106">List properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8fef1-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8fef1-107">Prerequisites</span></span>
<span data-ttu-id="8fef1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8fef1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8fef1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8fef1-110">Permission type</span></span>|<span data-ttu-id="8fef1-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8fef1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8fef1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8fef1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8fef1-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8fef1-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="8fef1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8fef1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8fef1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8fef1-115">Not supported.</span></span>|
|<span data-ttu-id="8fef1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8fef1-116">Application</span></span>|<span data-ttu-id="8fef1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8fef1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8fef1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8fef1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8fef1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8fef1-119">Request headers</span></span>
|<span data-ttu-id="8fef1-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8fef1-120">Header</span></span>|<span data-ttu-id="8fef1-121">Wert</span><span class="sxs-lookup"><span data-stu-id="8fef1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8fef1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8fef1-122">Authorization</span></span>|<span data-ttu-id="8fef1-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8fef1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8fef1-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8fef1-124">Accept</span></span>|<span data-ttu-id="8fef1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8fef1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fef1-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8fef1-126">Request body</span></span>
<span data-ttu-id="8fef1-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8fef1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8fef1-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="8fef1-128">Response</span></span>
<span data-ttu-id="8fef1-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8fef1-129">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fef1-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8fef1-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8fef1-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8fef1-131">Request</span></span>
<span data-ttu-id="8fef1-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8fef1-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="8fef1-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="8fef1-133">Response</span></span>
<span data-ttu-id="8fef1-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8fef1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 446

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
      "id": "4f8c4e4c-4e4c-4f8c-4c4e-8c4f4c4e8c4f",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7,
      "limit": 5
    }
  ]
}
```




