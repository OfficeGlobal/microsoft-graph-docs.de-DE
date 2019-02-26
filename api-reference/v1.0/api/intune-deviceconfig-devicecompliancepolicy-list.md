---
title: Auflisten von „deviceCompliancePolicy“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceCompliancePolicy auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e7382448112a3a7ef3bbc69b6e4f134bc9961242
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262909"
---
# <a name="list-devicecompliancepolicies"></a><span data-ttu-id="4d5c3-103">Auflisten von „deviceCompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="4d5c3-103">List deviceCompliancePolicies</span></span>

> <span data-ttu-id="4d5c3-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4d5c3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d5c3-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) auf.</span><span class="sxs-lookup"><span data-stu-id="4d5c3-105">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d5c3-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4d5c3-106">Prerequisites</span></span>
<span data-ttu-id="4d5c3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4d5c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4d5c3-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4d5c3-109">Permission type</span></span>|<span data-ttu-id="4d5c3-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4d5c3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d5c3-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4d5c3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4d5c3-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d5c3-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4d5c3-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4d5c3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d5c3-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d5c3-114">Not supported.</span></span>|
|<span data-ttu-id="4d5c3-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4d5c3-115">Application</span></span>|<span data-ttu-id="4d5c3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d5c3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d5c3-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d5c3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="4d5c3-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4d5c3-118">Request headers</span></span>
|<span data-ttu-id="4d5c3-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4d5c3-119">Header</span></span>|<span data-ttu-id="4d5c3-120">Wert</span><span class="sxs-lookup"><span data-stu-id="4d5c3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d5c3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d5c3-121">Authorization</span></span>|<span data-ttu-id="4d5c3-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4d5c3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d5c3-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4d5c3-123">Accept</span></span>|<span data-ttu-id="4d5c3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4d5c3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d5c3-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4d5c3-125">Request body</span></span>
<span data-ttu-id="4d5c3-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4d5c3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d5c3-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d5c3-127">Response</span></span>
<span data-ttu-id="4d5c3-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4d5c3-128">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d5c3-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4d5c3-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d5c3-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d5c3-130">Request</span></span>
<span data-ttu-id="4d5c3-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4d5c3-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="4d5c3-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d5c3-132">Response</span></span>
<span data-ttu-id="4d5c3-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4d5c3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 393

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
      "id": "4214b716-b716-4214-16b7-144216b71442",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```



