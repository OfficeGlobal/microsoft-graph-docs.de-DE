---
title: Auflisten von „deviceEnrollmentLimitConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceEnrollmentLimitConfiguration auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: afd0c6f4a62ead8c609b764b955ded40d868d214
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30987538"
---
# <a name="list-deviceenrollmentlimitconfigurations"></a><span data-ttu-id="2cfe9-103">Auflisten von „deviceEnrollmentLimitConfiguration“</span><span class="sxs-lookup"><span data-stu-id="2cfe9-103">List deviceEnrollmentLimitConfigurations</span></span>

> <span data-ttu-id="2cfe9-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2cfe9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2cfe9-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2cfe9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cfe9-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="2cfe9-106">List properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2cfe9-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2cfe9-107">Prerequisites</span></span>
<span data-ttu-id="2cfe9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cfe9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cfe9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2cfe9-110">Permission type</span></span>|<span data-ttu-id="2cfe9-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2cfe9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2cfe9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2cfe9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2cfe9-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2cfe9-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2cfe9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2cfe9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2cfe9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2cfe9-115">Not supported.</span></span>|
|<span data-ttu-id="2cfe9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2cfe9-116">Application</span></span>|<span data-ttu-id="2cfe9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2cfe9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2cfe9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2cfe9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2cfe9-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2cfe9-119">Request headers</span></span>
|<span data-ttu-id="2cfe9-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2cfe9-120">Header</span></span>|<span data-ttu-id="2cfe9-121">Wert</span><span class="sxs-lookup"><span data-stu-id="2cfe9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2cfe9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2cfe9-122">Authorization</span></span>|<span data-ttu-id="2cfe9-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2cfe9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2cfe9-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2cfe9-124">Accept</span></span>|<span data-ttu-id="2cfe9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2cfe9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cfe9-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2cfe9-126">Request body</span></span>
<span data-ttu-id="2cfe9-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2cfe9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2cfe9-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="2cfe9-128">Response</span></span>
<span data-ttu-id="2cfe9-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2cfe9-129">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2cfe9-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2cfe9-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2cfe9-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2cfe9-131">Request</span></span>
<span data-ttu-id="2cfe9-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2cfe9-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="2cfe9-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="2cfe9-133">Response</span></span>
<span data-ttu-id="2cfe9-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2cfe9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




