---
title: deviceEnrollmentLimitConfiguration abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceEnrollmentLimitConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b55b90f3eaf754a8835775212747228e352096a9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144219"
---
# <a name="get-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="2f93b-103">deviceEnrollmentLimitConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="2f93b-103">Get deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="2f93b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2f93b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f93b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2f93b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f93b-106">Lesen von Eigenschaften und Beziehungen des [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2f93b-106">Read properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f93b-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2f93b-107">Prerequisites</span></span>
<span data-ttu-id="2f93b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2f93b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2f93b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2f93b-110">Permission type</span></span>|<span data-ttu-id="2f93b-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2f93b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f93b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2f93b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2f93b-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f93b-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2f93b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2f93b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f93b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f93b-115">Not supported.</span></span>|
|<span data-ttu-id="2f93b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2f93b-116">Application</span></span>|<span data-ttu-id="2f93b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f93b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f93b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f93b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2f93b-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="2f93b-119">Optional query parameters</span></span>
<span data-ttu-id="2f93b-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2f93b-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f93b-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2f93b-121">Request headers</span></span>
|<span data-ttu-id="2f93b-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2f93b-122">Header</span></span>|<span data-ttu-id="2f93b-123">Wert</span><span class="sxs-lookup"><span data-stu-id="2f93b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f93b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f93b-124">Authorization</span></span>|<span data-ttu-id="2f93b-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2f93b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f93b-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2f93b-126">Accept</span></span>|<span data-ttu-id="2f93b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2f93b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f93b-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2f93b-128">Request body</span></span>
<span data-ttu-id="2f93b-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2f93b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f93b-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f93b-130">Response</span></span>
<span data-ttu-id="2f93b-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2f93b-131">If successful, this method returns a `200 OK` response code and [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f93b-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f93b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f93b-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f93b-133">Request</span></span>
<span data-ttu-id="2f93b-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2f93b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="2f93b-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f93b-135">Response</span></span>
<span data-ttu-id="2f93b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2f93b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 414

{
  "value": {
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
}
```




