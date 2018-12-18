---
title: IosLobAppProvisioningConfigurationAssignment aktualisieren
description: Aktualisieren Sie die Eigenschaften eines IosLobAppProvisioningConfigurationAssignment-Objekts.
author: tfitzmac
ms.openlocfilehash: 0212d357ceee946e8515a5143ffd7bf7307a7773
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338878"
---
# <a name="update-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="01d77-103">IosLobAppProvisioningConfigurationAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="01d77-103">Update iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="01d77-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="01d77-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01d77-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="01d77-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="01d77-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="01d77-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01d77-107">Aktualisieren Sie die Eigenschaften eines [IosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="01d77-107">Update the properties of a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="01d77-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="01d77-108">Prerequisites</span></span>
<span data-ttu-id="01d77-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01d77-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01d77-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="01d77-111">Permission type</span></span>|<span data-ttu-id="01d77-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="01d77-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01d77-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="01d77-113">Delegated (work or school account)</span></span>|<span data-ttu-id="01d77-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01d77-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="01d77-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="01d77-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01d77-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="01d77-116">Not supported.</span></span>|
|<span data-ttu-id="01d77-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="01d77-117">Application</span></span>|<span data-ttu-id="01d77-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="01d77-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01d77-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="01d77-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="01d77-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="01d77-120">Request headers</span></span>
|<span data-ttu-id="01d77-121">Header</span><span class="sxs-lookup"><span data-stu-id="01d77-121">Header</span></span>|<span data-ttu-id="01d77-122">Wert</span><span class="sxs-lookup"><span data-stu-id="01d77-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01d77-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="01d77-123">Authorization</span></span>|<span data-ttu-id="01d77-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="01d77-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01d77-125">Accept</span><span class="sxs-lookup"><span data-stu-id="01d77-125">Accept</span></span>|<span data-ttu-id="01d77-126">application/json</span><span class="sxs-lookup"><span data-stu-id="01d77-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01d77-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="01d77-127">Request body</span></span>
<span data-ttu-id="01d77-128">Geben Sie im Textkörper Anforderung für das Objekt [IosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="01d77-128">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

<span data-ttu-id="01d77-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [IosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="01d77-129">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).</span></span>

|<span data-ttu-id="01d77-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="01d77-130">Property</span></span>|<span data-ttu-id="01d77-131">Typ</span><span class="sxs-lookup"><span data-stu-id="01d77-131">Type</span></span>|<span data-ttu-id="01d77-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="01d77-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01d77-133">id</span><span class="sxs-lookup"><span data-stu-id="01d77-133">id</span></span>|<span data-ttu-id="01d77-134">String</span><span class="sxs-lookup"><span data-stu-id="01d77-134">String</span></span>|<span data-ttu-id="01d77-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="01d77-135">Key of the entity.</span></span>|
|<span data-ttu-id="01d77-136">target</span><span class="sxs-lookup"><span data-stu-id="01d77-136">target</span></span>|[<span data-ttu-id="01d77-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="01d77-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="01d77-138">Die vom Administrator definierte Zielgruppenzuordnung</span><span class="sxs-lookup"><span data-stu-id="01d77-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="01d77-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="01d77-139">Response</span></span>
<span data-ttu-id="01d77-140">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [IosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="01d77-140">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01d77-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="01d77-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="01d77-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="01d77-142">Request</span></span>
<span data-ttu-id="01d77-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="01d77-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="01d77-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="01d77-144">Response</span></span>
<span data-ttu-id="01d77-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="01d77-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





