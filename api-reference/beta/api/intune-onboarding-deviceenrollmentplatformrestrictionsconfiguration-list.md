---
title: Auflisten von „deviceEnrollmentPlatformRestrictionsConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceEnrollmentPlatformRestrictionsConfiguration auf.
ms.openlocfilehash: fc16125add898cfad3142d24830d26804035afc5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066126"
---
# <a name="list-deviceenrollmentplatformrestrictionsconfigurations"></a><span data-ttu-id="8313a-103">Auflisten von „deviceEnrollmentPlatformRestrictionsConfiguration“</span><span class="sxs-lookup"><span data-stu-id="8313a-103">List deviceEnrollmentPlatformRestrictionsConfigurations</span></span>

> <span data-ttu-id="8313a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8313a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8313a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8313a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8313a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8313a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8313a-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="8313a-107">List properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8313a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8313a-108">Prerequisites</span></span>
<span data-ttu-id="8313a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8313a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8313a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8313a-111">Permission type</span></span>|<span data-ttu-id="8313a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8313a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8313a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8313a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8313a-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8313a-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="8313a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8313a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8313a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8313a-116">Not supported.</span></span>|
|<span data-ttu-id="8313a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8313a-117">Application</span></span>|<span data-ttu-id="8313a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8313a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8313a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8313a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8313a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8313a-120">Request headers</span></span>
|<span data-ttu-id="8313a-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8313a-121">Header</span></span>|<span data-ttu-id="8313a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8313a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8313a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8313a-123">Authorization</span></span>|<span data-ttu-id="8313a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8313a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8313a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8313a-125">Accept</span></span>|<span data-ttu-id="8313a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8313a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8313a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8313a-127">Request body</span></span>
<span data-ttu-id="8313a-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8313a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8313a-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="8313a-129">Response</span></span>
<span data-ttu-id="8313a-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8313a-130">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8313a-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8313a-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="8313a-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8313a-132">Request</span></span>
<span data-ttu-id="8313a-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8313a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="8313a-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="8313a-134">Response</span></span>
<span data-ttu-id="8313a-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8313a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2664

{
  "value": [
    {
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
      "androidForWorkRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value"
      },
      "macRestriction": {
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
  ]
}
```





