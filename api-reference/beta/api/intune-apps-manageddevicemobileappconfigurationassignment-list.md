---
title: Auflisten von „managedDeviceMobileAppConfigurationAssignment“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs managedDeviceMobileAppConfigurationAssignment auf.
ms.openlocfilehash: c189801537f0ae191e138edca95080c0cb6d55d6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060822"
---
# <a name="list-manageddevicemobileappconfigurationassignments"></a><span data-ttu-id="71c71-103">Auflisten von „managedDeviceMobileAppConfigurationAssignment“</span><span class="sxs-lookup"><span data-stu-id="71c71-103">List managedDeviceMobileAppConfigurationAssignments</span></span>

> <span data-ttu-id="71c71-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="71c71-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71c71-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="71c71-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="71c71-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="71c71-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71c71-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) auf.</span><span class="sxs-lookup"><span data-stu-id="71c71-107">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="71c71-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="71c71-108">Prerequisites</span></span>
<span data-ttu-id="71c71-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71c71-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71c71-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="71c71-111">Permission type</span></span>|<span data-ttu-id="71c71-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="71c71-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71c71-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="71c71-113">Delegated (work or school account)</span></span>|<span data-ttu-id="71c71-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="71c71-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="71c71-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="71c71-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71c71-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71c71-116">Not supported.</span></span>|
|<span data-ttu-id="71c71-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="71c71-117">Application</span></span>|<span data-ttu-id="71c71-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71c71-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71c71-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="71c71-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="71c71-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="71c71-120">Request headers</span></span>
|<span data-ttu-id="71c71-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="71c71-121">Header</span></span>|<span data-ttu-id="71c71-122">Wert</span><span class="sxs-lookup"><span data-stu-id="71c71-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71c71-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="71c71-123">Authorization</span></span>|<span data-ttu-id="71c71-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="71c71-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71c71-125">Accept</span><span class="sxs-lookup"><span data-stu-id="71c71-125">Accept</span></span>|<span data-ttu-id="71c71-126">application/json</span><span class="sxs-lookup"><span data-stu-id="71c71-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71c71-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="71c71-127">Request body</span></span>
<span data-ttu-id="71c71-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="71c71-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71c71-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="71c71-129">Response</span></span>
<span data-ttu-id="71c71-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="71c71-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71c71-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="71c71-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="71c71-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="71c71-132">Request</span></span>
<span data-ttu-id="71c71-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="71c71-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="71c71-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="71c71-134">Response</span></span>
<span data-ttu-id="71c71-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="71c71-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





