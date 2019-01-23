---
title: Auflisten von „managedDeviceMobileAppConfigurationAssignment“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs managedDeviceMobileAppConfigurationAssignment auf.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 967b4fae913ff8c26ffaeb081159a106738da605
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397736"
---
# <a name="list-manageddevicemobileappconfigurationassignments"></a><span data-ttu-id="f591d-103">Auflisten von „managedDeviceMobileAppConfigurationAssignment“</span><span class="sxs-lookup"><span data-stu-id="f591d-103">List managedDeviceMobileAppConfigurationAssignments</span></span>

> <span data-ttu-id="f591d-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="f591d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f591d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f591d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f591d-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f591d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f591d-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) auf.</span><span class="sxs-lookup"><span data-stu-id="f591d-107">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f591d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f591d-108">Prerequisites</span></span>
<span data-ttu-id="f591d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f591d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f591d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f591d-111">Permission type</span></span>|<span data-ttu-id="f591d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f591d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f591d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f591d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f591d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f591d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f591d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f591d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f591d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f591d-116">Not supported.</span></span>|
|<span data-ttu-id="f591d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f591d-117">Application</span></span>|<span data-ttu-id="f591d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f591d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f591d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f591d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="f591d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f591d-120">Request headers</span></span>
|<span data-ttu-id="f591d-121">Header</span><span class="sxs-lookup"><span data-stu-id="f591d-121">Header</span></span>|<span data-ttu-id="f591d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f591d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f591d-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f591d-123">Authorization</span></span>|<span data-ttu-id="f591d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f591d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f591d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f591d-125">Accept</span></span>|<span data-ttu-id="f591d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f591d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f591d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f591d-127">Request body</span></span>
<span data-ttu-id="f591d-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f591d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f591d-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f591d-129">Response</span></span>
<span data-ttu-id="f591d-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f591d-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f591d-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f591d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f591d-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f591d-132">Request</span></span>
<span data-ttu-id="f591d-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f591d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="f591d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f591d-134">Response</span></span>
<span data-ttu-id="f591d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f591d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
      "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```




