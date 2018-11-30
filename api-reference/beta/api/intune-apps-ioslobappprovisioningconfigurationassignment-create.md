---
title: Erstellen von iosLobAppProvisioningConfigurationAssignment
description: Erstellen eines neuen IosLobAppProvisioningConfigurationAssignment-Objekts.
ms.openlocfilehash: 5d3a51aab8560e4922d74e48675aa95c25be5c72
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058588"
---
# <a name="create-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="18d38-103">Erstellen von iosLobAppProvisioningConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="18d38-103">Create iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="18d38-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="18d38-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18d38-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="18d38-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="18d38-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="18d38-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18d38-107">Erstellen eines neuen [IosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="18d38-107">Create a new [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="18d38-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="18d38-108">Prerequisites</span></span>
<span data-ttu-id="18d38-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18d38-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18d38-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="18d38-111">Permission type</span></span>|<span data-ttu-id="18d38-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="18d38-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18d38-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="18d38-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18d38-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18d38-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="18d38-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="18d38-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18d38-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="18d38-116">Not supported.</span></span>|
|<span data-ttu-id="18d38-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="18d38-117">Application</span></span>|<span data-ttu-id="18d38-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="18d38-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18d38-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="18d38-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="18d38-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="18d38-120">Request headers</span></span>
|<span data-ttu-id="18d38-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="18d38-121">Header</span></span>|<span data-ttu-id="18d38-122">Wert</span><span class="sxs-lookup"><span data-stu-id="18d38-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18d38-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="18d38-123">Authorization</span></span>|<span data-ttu-id="18d38-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="18d38-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18d38-125">Accept</span><span class="sxs-lookup"><span data-stu-id="18d38-125">Accept</span></span>|<span data-ttu-id="18d38-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18d38-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18d38-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="18d38-127">Request body</span></span>
<span data-ttu-id="18d38-128">Geben Sie im Textkörper Anforderung für das Objekt IosLobAppProvisioningConfigurationAssignment eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="18d38-128">In the request body, supply a JSON representation for the iosLobAppProvisioningConfigurationAssignment object.</span></span>

<span data-ttu-id="18d38-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die IosLobAppProvisioningConfigurationAssignment erstellen.</span><span class="sxs-lookup"><span data-stu-id="18d38-129">The following table shows the properties that are required when you create the iosLobAppProvisioningConfigurationAssignment.</span></span>

|<span data-ttu-id="18d38-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="18d38-130">Property</span></span>|<span data-ttu-id="18d38-131">Typ</span><span class="sxs-lookup"><span data-stu-id="18d38-131">Type</span></span>|<span data-ttu-id="18d38-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="18d38-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18d38-133">id</span><span class="sxs-lookup"><span data-stu-id="18d38-133">id</span></span>|<span data-ttu-id="18d38-134">String</span><span class="sxs-lookup"><span data-stu-id="18d38-134">String</span></span>|<span data-ttu-id="18d38-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="18d38-135">Key of the entity.</span></span>|
|<span data-ttu-id="18d38-136">target</span><span class="sxs-lookup"><span data-stu-id="18d38-136">target</span></span>|[<span data-ttu-id="18d38-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="18d38-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="18d38-138">Die vom Administrator definierte Zielgruppenzuordnung</span><span class="sxs-lookup"><span data-stu-id="18d38-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="18d38-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="18d38-139">Response</span></span>
<span data-ttu-id="18d38-140">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [IosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="18d38-140">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18d38-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="18d38-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="18d38-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="18d38-142">Request</span></span>
<span data-ttu-id="18d38-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="18d38-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
Content-type: application/json
Content-length: 184

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="18d38-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="18d38-144">Response</span></span>
<span data-ttu-id="18d38-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="18d38-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 233

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "id": "eac7008e-008e-eac7-8e00-c7ea8e00c7ea",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





