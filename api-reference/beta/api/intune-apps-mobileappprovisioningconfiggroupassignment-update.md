---
title: MobileAppProvisioningConfigGroupAssignment aktualisieren
description: Aktualisieren Sie die Eigenschaften eines MobileAppProvisioningConfigGroupAssignment-Objekts.
ms.openlocfilehash: 81e9efc268130cbdc2baf44e098d6f11a949e90f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063403"
---
# <a name="update-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="b368c-103">MobileAppProvisioningConfigGroupAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b368c-103">Update mobileAppProvisioningConfigGroupAssignment</span></span>

> <span data-ttu-id="b368c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b368c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b368c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b368c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b368c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b368c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b368c-107">Aktualisieren Sie die Eigenschaften eines [MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b368c-107">Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b368c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b368c-108">Prerequisites</span></span>
<span data-ttu-id="b368c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b368c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b368c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b368c-111">Permission type</span></span>|<span data-ttu-id="b368c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b368c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b368c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b368c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b368c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b368c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b368c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b368c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b368c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b368c-116">Not supported.</span></span>|
|<span data-ttu-id="b368c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b368c-117">Application</span></span>|<span data-ttu-id="b368c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b368c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b368c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b368c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b368c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b368c-120">Request headers</span></span>
|<span data-ttu-id="b368c-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b368c-121">Header</span></span>|<span data-ttu-id="b368c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b368c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b368c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b368c-123">Authorization</span></span>|<span data-ttu-id="b368c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b368c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b368c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b368c-125">Accept</span></span>|<span data-ttu-id="b368c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b368c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b368c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b368c-127">Request body</span></span>
<span data-ttu-id="b368c-128">Geben Sie im Textkörper Anforderung für das Objekt [MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="b368c-128">In the request body, supply a JSON representation for the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

<span data-ttu-id="b368c-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="b368c-129">The following table shows the properties that are required when you create the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>

|<span data-ttu-id="b368c-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b368c-130">Property</span></span>|<span data-ttu-id="b368c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b368c-131">Type</span></span>|<span data-ttu-id="b368c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b368c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b368c-133">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="b368c-133">targetGroupId</span></span>|<span data-ttu-id="b368c-134">String</span><span class="sxs-lookup"><span data-stu-id="b368c-134">String</span></span>|<span data-ttu-id="b368c-135">Die ID der Gruppe der AAD, in der die app-Bereitstellung Konfiguration vorgesehen ist.</span><span class="sxs-lookup"><span data-stu-id="b368c-135">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="b368c-136">id</span><span class="sxs-lookup"><span data-stu-id="b368c-136">id</span></span>|<span data-ttu-id="b368c-137">String</span><span class="sxs-lookup"><span data-stu-id="b368c-137">String</span></span>|<span data-ttu-id="b368c-138">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b368c-138">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="b368c-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="b368c-139">Response</span></span>
<span data-ttu-id="b368c-140">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b368c-140">If successful, this method returns a `200 OK` response code and an updated [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b368c-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b368c-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="b368c-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b368c-142">Request</span></span>
<span data-ttu-id="b368c-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b368c-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
Content-type: application/json
Content-length: 48

{
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="b368c-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="b368c-144">Response</span></span>
<span data-ttu-id="b368c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b368c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 178

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
}
```





