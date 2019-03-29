---
title: Auflisten von „deviceEnrollmentConfiguration“
description: Auflisten von Eigenschaften und Beziehungen der deviceEnrollmentConfiguration-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9acffd3d342391722207898340cd7ee005a51fb5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978010"
---
# <a name="list-deviceenrollmentconfigurations"></a><span data-ttu-id="272d8-103">Auflisten von „deviceEnrollmentConfiguration“</span><span class="sxs-lookup"><span data-stu-id="272d8-103">List deviceEnrollmentConfigurations</span></span>

> <span data-ttu-id="272d8-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="272d8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="272d8-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="272d8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="272d8-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="272d8-106">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="272d8-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="272d8-107">Prerequisites</span></span>
<span data-ttu-id="272d8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="272d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="272d8-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="272d8-110">Permission type</span></span>|<span data-ttu-id="272d8-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="272d8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="272d8-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="272d8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="272d8-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="272d8-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="272d8-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="272d8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="272d8-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="272d8-115">Not supported.</span></span>|
|<span data-ttu-id="272d8-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="272d8-116">Application</span></span>|<span data-ttu-id="272d8-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="272d8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="272d8-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="272d8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="272d8-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="272d8-119">Request headers</span></span>
|<span data-ttu-id="272d8-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="272d8-120">Header</span></span>|<span data-ttu-id="272d8-121">Wert</span><span class="sxs-lookup"><span data-stu-id="272d8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="272d8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="272d8-122">Authorization</span></span>|<span data-ttu-id="272d8-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="272d8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="272d8-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="272d8-124">Accept</span></span>|<span data-ttu-id="272d8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="272d8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="272d8-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="272d8-126">Request body</span></span>
<span data-ttu-id="272d8-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="272d8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="272d8-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="272d8-128">Response</span></span>
<span data-ttu-id="272d8-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="272d8-129">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="272d8-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="272d8-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="272d8-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="272d8-131">Request</span></span>
<span data-ttu-id="272d8-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="272d8-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="272d8-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="272d8-133">Response</span></span>
<span data-ttu-id="272d8-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="272d8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




