---
title: managedDeviceMobileAppConfigurationAssignment abrufen
description: Lesen von Eigenschaften und Beziehungen des managedDeviceMobileAppConfigurationAssignment-Objekts.
ms.openlocfilehash: 91d4089c93f9490ed654572032a648ab03dce14f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064541"
---
# <a name="get-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="202ff-103">managedDeviceMobileAppConfigurationAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="202ff-103">Get managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="202ff-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="202ff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="202ff-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="202ff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="202ff-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="202ff-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="202ff-107">Lesen von Eigenschaften und Beziehungen des [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="202ff-107">Read properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="202ff-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="202ff-108">Prerequisites</span></span>
<span data-ttu-id="202ff-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="202ff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="202ff-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="202ff-111">Permission type</span></span>|<span data-ttu-id="202ff-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="202ff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="202ff-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="202ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="202ff-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="202ff-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="202ff-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="202ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="202ff-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="202ff-116">Not supported.</span></span>|
|<span data-ttu-id="202ff-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="202ff-117">Application</span></span>|<span data-ttu-id="202ff-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="202ff-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="202ff-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="202ff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="202ff-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="202ff-120">Optional query parameters</span></span>
<span data-ttu-id="202ff-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="202ff-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="202ff-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="202ff-122">Request headers</span></span>
|<span data-ttu-id="202ff-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="202ff-123">Header</span></span>|<span data-ttu-id="202ff-124">Wert</span><span class="sxs-lookup"><span data-stu-id="202ff-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="202ff-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="202ff-125">Authorization</span></span>|<span data-ttu-id="202ff-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="202ff-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="202ff-127">Accept</span><span class="sxs-lookup"><span data-stu-id="202ff-127">Accept</span></span>|<span data-ttu-id="202ff-128">application/json</span><span class="sxs-lookup"><span data-stu-id="202ff-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="202ff-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="202ff-129">Request body</span></span>
<span data-ttu-id="202ff-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="202ff-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="202ff-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="202ff-131">Response</span></span>
<span data-ttu-id="202ff-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="202ff-132">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="202ff-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="202ff-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="202ff-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="202ff-134">Request</span></span>
<span data-ttu-id="202ff-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="202ff-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="202ff-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="202ff-136">Response</span></span>
<span data-ttu-id="202ff-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="202ff-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 263

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
    "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```




