---
title: MobileAppProvisioningConfigGroupAssignment aktualisieren
description: Aktualisieren der Eigenschaften eines mobileAppProvisioningConfigGroupAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 21c4c65dc6deec19cda232d4c5be377e38e92a9a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144401"
---
# <a name="update-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="33f96-103">MobileAppProvisioningConfigGroupAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="33f96-103">Update mobileAppProvisioningConfigGroupAssignment</span></span>

> <span data-ttu-id="33f96-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="33f96-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33f96-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="33f96-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33f96-106">Aktualisieren der Eigenschaften eines [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="33f96-106">Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33f96-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="33f96-107">Prerequisites</span></span>
<span data-ttu-id="33f96-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="33f96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="33f96-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="33f96-110">Permission type</span></span>|<span data-ttu-id="33f96-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="33f96-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33f96-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="33f96-112">Delegated (work or school account)</span></span>|<span data-ttu-id="33f96-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33f96-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="33f96-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="33f96-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33f96-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="33f96-115">Not supported.</span></span>|
|<span data-ttu-id="33f96-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="33f96-116">Application</span></span>|<span data-ttu-id="33f96-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="33f96-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33f96-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="33f96-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="33f96-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="33f96-119">Request headers</span></span>
|<span data-ttu-id="33f96-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="33f96-120">Header</span></span>|<span data-ttu-id="33f96-121">Wert</span><span class="sxs-lookup"><span data-stu-id="33f96-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33f96-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="33f96-122">Authorization</span></span>|<span data-ttu-id="33f96-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="33f96-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33f96-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="33f96-124">Accept</span></span>|<span data-ttu-id="33f96-125">application/json</span><span class="sxs-lookup"><span data-stu-id="33f96-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33f96-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="33f96-126">Request body</span></span>
<span data-ttu-id="33f96-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="33f96-127">In the request body, supply a JSON representation for the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

<span data-ttu-id="33f96-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="33f96-128">The following table shows the properties that are required when you create the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>

|<span data-ttu-id="33f96-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="33f96-129">Property</span></span>|<span data-ttu-id="33f96-130">Typ</span><span class="sxs-lookup"><span data-stu-id="33f96-130">Type</span></span>|<span data-ttu-id="33f96-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="33f96-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33f96-132">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="33f96-132">targetGroupId</span></span>|<span data-ttu-id="33f96-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33f96-133">String</span></span>|<span data-ttu-id="33f96-134">Die ID der AAD-Gruppe, in der die APP-Konfigurations Konfiguration gezielt wird.</span><span class="sxs-lookup"><span data-stu-id="33f96-134">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="33f96-135">id</span><span class="sxs-lookup"><span data-stu-id="33f96-135">id</span></span>|<span data-ttu-id="33f96-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33f96-136">String</span></span>|<span data-ttu-id="33f96-137">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="33f96-137">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="33f96-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="33f96-138">Response</span></span>
<span data-ttu-id="33f96-139">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="33f96-139">If successful, this method returns a `200 OK` response code and an updated [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33f96-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="33f96-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="33f96-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="33f96-141">Request</span></span>
<span data-ttu-id="33f96-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="33f96-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="33f96-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="33f96-143">Response</span></span>
<span data-ttu-id="33f96-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="33f96-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




