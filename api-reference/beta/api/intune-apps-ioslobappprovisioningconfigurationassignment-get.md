---
title: Abrufen von iosLobAppProvisioningConfigurationAssignment
description: Lesen Sie Eigenschaften und Beziehungen des IosLobAppProvisioningConfigurationAssignment-Objekts.
ms.openlocfilehash: d2eb5ae3f68395bb4c33b7ec5f760e1f49cef5a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062611"
---
# <a name="get-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="fbdaa-103">Abrufen von iosLobAppProvisioningConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="fbdaa-103">Get iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="fbdaa-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fbdaa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fbdaa-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fbdaa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fbdaa-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fbdaa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fbdaa-107">Lesen Sie Eigenschaften und Beziehungen des [IosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="fbdaa-107">Read properties and relationships of the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fbdaa-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fbdaa-108">Prerequisites</span></span>
<span data-ttu-id="fbdaa-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbdaa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbdaa-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fbdaa-111">Permission type</span></span>|<span data-ttu-id="fbdaa-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fbdaa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbdaa-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fbdaa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fbdaa-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbdaa-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fbdaa-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fbdaa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbdaa-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fbdaa-116">Not supported.</span></span>|
|<span data-ttu-id="fbdaa-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fbdaa-117">Application</span></span>|<span data-ttu-id="fbdaa-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fbdaa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbdaa-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fbdaa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fbdaa-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fbdaa-120">Optional query parameters</span></span>
<span data-ttu-id="fbdaa-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fbdaa-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fbdaa-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fbdaa-122">Request headers</span></span>
|<span data-ttu-id="fbdaa-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fbdaa-123">Header</span></span>|<span data-ttu-id="fbdaa-124">Wert</span><span class="sxs-lookup"><span data-stu-id="fbdaa-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbdaa-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbdaa-125">Authorization</span></span>|<span data-ttu-id="fbdaa-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fbdaa-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbdaa-127">Accept</span><span class="sxs-lookup"><span data-stu-id="fbdaa-127">Accept</span></span>|<span data-ttu-id="fbdaa-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fbdaa-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbdaa-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fbdaa-129">Request body</span></span>
<span data-ttu-id="fbdaa-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fbdaa-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fbdaa-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="fbdaa-131">Response</span></span>
<span data-ttu-id="fbdaa-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [IosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="fbdaa-132">If successful, this method returns a `200 OK` response code and [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbdaa-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fbdaa-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="fbdaa-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fbdaa-134">Request</span></span>
<span data-ttu-id="fbdaa-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fbdaa-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="fbdaa-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="fbdaa-136">Response</span></span>
<span data-ttu-id="fbdaa-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fbdaa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 262

{
  "value": {
    "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
    "id": "eac7008e-008e-eac7-8e00-c7ea8e00c7ea",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```





