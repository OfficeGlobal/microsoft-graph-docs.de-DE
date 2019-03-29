---
title: Abrufen von „deviceEnrollmentPlatformRestrictionsConfiguration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs deviceEnrollmentPlatformRestrictionsConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d2d123b37e1e0eab84c3ad3517d32c6da8245e1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970737"
---
# <a name="get-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="91ac2-103">Abrufen von „deviceEnrollmentPlatformRestrictionsConfiguration“</span><span class="sxs-lookup"><span data-stu-id="91ac2-103">Get deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="91ac2-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="91ac2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91ac2-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="91ac2-105">Read properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91ac2-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="91ac2-106">Prerequisites</span></span>
<span data-ttu-id="91ac2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91ac2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91ac2-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="91ac2-109">Permission type</span></span>|<span data-ttu-id="91ac2-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="91ac2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91ac2-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="91ac2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="91ac2-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="91ac2-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="91ac2-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="91ac2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91ac2-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="91ac2-114">Not supported.</span></span>|
|<span data-ttu-id="91ac2-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="91ac2-115">Application</span></span>|<span data-ttu-id="91ac2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="91ac2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="91ac2-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="91ac2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="91ac2-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="91ac2-118">Optional query parameters</span></span>
<span data-ttu-id="91ac2-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="91ac2-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="91ac2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="91ac2-120">Request headers</span></span>
|<span data-ttu-id="91ac2-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="91ac2-121">Header</span></span>|<span data-ttu-id="91ac2-122">Wert</span><span class="sxs-lookup"><span data-stu-id="91ac2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91ac2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="91ac2-123">Authorization</span></span>|<span data-ttu-id="91ac2-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="91ac2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91ac2-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="91ac2-125">Accept</span></span>|<span data-ttu-id="91ac2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="91ac2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91ac2-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="91ac2-127">Request body</span></span>
<span data-ttu-id="91ac2-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="91ac2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91ac2-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="91ac2-129">Response</span></span>
<span data-ttu-id="91ac2-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="91ac2-130">If successful, this method returns a `200 OK` response code and [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91ac2-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="91ac2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="91ac2-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="91ac2-132">Request</span></span>
<span data-ttu-id="91ac2-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="91ac2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="91ac2-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="91ac2-134">Response</span></span>
<span data-ttu-id="91ac2-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="91ac2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1927

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
    "id": "3acb2d75-2d75-3acb-752d-cb3a752dcb3a",
    "displayName": "Display Name value",
    "description": "Description value",
    "priority": 8,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "version": 7,
    "iosRestriction": {
      "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
      "platformBlocked": true,
      "personalDeviceEnrollmentBlocked": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value"
    },
    "windowsRestriction": {
      "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
      "platformBlocked": true,
      "personalDeviceEnrollmentBlocked": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value"
    },
    "windowsMobileRestriction": {
      "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
      "platformBlocked": true,
      "personalDeviceEnrollmentBlocked": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value"
    },
    "androidRestriction": {
      "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
      "platformBlocked": true,
      "personalDeviceEnrollmentBlocked": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value"
    },
    "macOSRestriction": {
      "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
      "platformBlocked": true,
      "personalDeviceEnrollmentBlocked": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value"
    }
  }
}
```



