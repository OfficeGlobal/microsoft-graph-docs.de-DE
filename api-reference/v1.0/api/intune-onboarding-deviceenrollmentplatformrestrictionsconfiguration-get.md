---
title: Abrufen von „deviceEnrollmentPlatformRestrictionsConfiguration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs deviceEnrollmentPlatformRestrictionsConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a468a38edc5dfd45b5e0c2cc10b42f7d09130f3a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845115"
---
# <a name="get-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="e2859-103">Abrufen von „deviceEnrollmentPlatformRestrictionsConfiguration“</span><span class="sxs-lookup"><span data-stu-id="e2859-103">Get deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="e2859-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e2859-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2859-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2859-105">Read properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e2859-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e2859-106">Prerequisites</span></span>
<span data-ttu-id="e2859-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2859-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2859-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e2859-109">Permission type</span></span>|<span data-ttu-id="e2859-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e2859-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2859-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e2859-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e2859-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2859-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e2859-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e2859-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2859-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e2859-114">Not supported.</span></span>|
|<span data-ttu-id="e2859-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e2859-115">Application</span></span>|<span data-ttu-id="e2859-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e2859-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2859-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e2859-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e2859-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e2859-118">Optional query parameters</span></span>
<span data-ttu-id="e2859-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e2859-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e2859-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e2859-120">Request headers</span></span>
|<span data-ttu-id="e2859-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e2859-121">Header</span></span>|<span data-ttu-id="e2859-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e2859-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2859-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2859-123">Authorization</span></span>|<span data-ttu-id="e2859-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e2859-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2859-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e2859-125">Accept</span></span>|<span data-ttu-id="e2859-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e2859-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2859-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e2859-127">Request body</span></span>
<span data-ttu-id="e2859-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e2859-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2859-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e2859-129">Response</span></span>
<span data-ttu-id="e2859-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e2859-130">If successful, this method returns a `200 OK` response code and [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2859-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e2859-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e2859-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e2859-132">Request</span></span>
<span data-ttu-id="e2859-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e2859-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e2859-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="e2859-134">Response</span></span>
<span data-ttu-id="e2859-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e2859-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



