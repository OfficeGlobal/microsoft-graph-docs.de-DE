---
title: Auflisten von „deviceEnrollmentLimitConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceEnrollmentLimitConfiguration auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d1816ec8358f29f8a638199346f0216ed883b7fb
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258968"
---
# <a name="list-deviceenrollmentlimitconfigurations"></a><span data-ttu-id="f1eaf-103">Auflisten von „deviceEnrollmentLimitConfiguration“</span><span class="sxs-lookup"><span data-stu-id="f1eaf-103">List deviceEnrollmentLimitConfigurations</span></span>

> <span data-ttu-id="f1eaf-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f1eaf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1eaf-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="f1eaf-105">List properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1eaf-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f1eaf-106">Prerequisites</span></span>
<span data-ttu-id="f1eaf-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f1eaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f1eaf-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f1eaf-109">Permission type</span></span>|<span data-ttu-id="f1eaf-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f1eaf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1eaf-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f1eaf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f1eaf-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1eaf-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f1eaf-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f1eaf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1eaf-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f1eaf-114">Not supported.</span></span>|
|<span data-ttu-id="f1eaf-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f1eaf-115">Application</span></span>|<span data-ttu-id="f1eaf-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f1eaf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1eaf-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1eaf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f1eaf-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f1eaf-118">Request headers</span></span>
|<span data-ttu-id="f1eaf-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f1eaf-119">Header</span></span>|<span data-ttu-id="f1eaf-120">Wert</span><span class="sxs-lookup"><span data-stu-id="f1eaf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1eaf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1eaf-121">Authorization</span></span>|<span data-ttu-id="f1eaf-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f1eaf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1eaf-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f1eaf-123">Accept</span></span>|<span data-ttu-id="f1eaf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f1eaf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1eaf-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f1eaf-125">Request body</span></span>
<span data-ttu-id="f1eaf-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f1eaf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1eaf-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1eaf-127">Response</span></span>
<span data-ttu-id="f1eaf-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f1eaf-128">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1eaf-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f1eaf-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1eaf-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1eaf-130">Request</span></span>
<span data-ttu-id="f1eaf-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f1eaf-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="f1eaf-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1eaf-132">Response</span></span>
<span data-ttu-id="f1eaf-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f1eaf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



