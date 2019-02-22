---
title: IosLobAppProvisioningConfigurationAssignment erstellen
description: Erstellen eines neuen iosLobAppProvisioningConfigurationAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 63f2862c9545a9683e66de58a0355299d0733092
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148384"
---
# <a name="create-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="21759-103">IosLobAppProvisioningConfigurationAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="21759-103">Create iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="21759-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="21759-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21759-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="21759-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21759-106">Erstellen eines neuen [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="21759-106">Create a new [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21759-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="21759-107">Prerequisites</span></span>
<span data-ttu-id="21759-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="21759-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="21759-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="21759-110">Permission type</span></span>|<span data-ttu-id="21759-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="21759-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21759-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="21759-112">Delegated (work or school account)</span></span>|<span data-ttu-id="21759-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21759-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="21759-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="21759-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21759-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="21759-115">Not supported.</span></span>|
|<span data-ttu-id="21759-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="21759-116">Application</span></span>|<span data-ttu-id="21759-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="21759-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21759-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="21759-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="21759-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="21759-119">Request headers</span></span>
|<span data-ttu-id="21759-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="21759-120">Header</span></span>|<span data-ttu-id="21759-121">Wert</span><span class="sxs-lookup"><span data-stu-id="21759-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21759-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="21759-122">Authorization</span></span>|<span data-ttu-id="21759-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="21759-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21759-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="21759-124">Accept</span></span>|<span data-ttu-id="21759-125">application/json</span><span class="sxs-lookup"><span data-stu-id="21759-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21759-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="21759-126">Request body</span></span>
<span data-ttu-id="21759-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das iosLobAppProvisioningConfigurationAssignment-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="21759-127">In the request body, supply a JSON representation for the iosLobAppProvisioningConfigurationAssignment object.</span></span>

<span data-ttu-id="21759-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der iosLobAppProvisioningConfigurationAssignment erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="21759-128">The following table shows the properties that are required when you create the iosLobAppProvisioningConfigurationAssignment.</span></span>

|<span data-ttu-id="21759-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="21759-129">Property</span></span>|<span data-ttu-id="21759-130">Typ</span><span class="sxs-lookup"><span data-stu-id="21759-130">Type</span></span>|<span data-ttu-id="21759-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="21759-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21759-132">id</span><span class="sxs-lookup"><span data-stu-id="21759-132">id</span></span>|<span data-ttu-id="21759-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21759-133">String</span></span>|<span data-ttu-id="21759-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="21759-134">Key of the entity.</span></span>|
|<span data-ttu-id="21759-135">target</span><span class="sxs-lookup"><span data-stu-id="21759-135">target</span></span>|[<span data-ttu-id="21759-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="21759-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="21759-137">Die vom Administrator definierte Zielgruppenzuordnung</span><span class="sxs-lookup"><span data-stu-id="21759-137">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="21759-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="21759-138">Response</span></span>
<span data-ttu-id="21759-139">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="21759-139">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21759-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="21759-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="21759-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="21759-141">Request</span></span>
<span data-ttu-id="21759-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="21759-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="21759-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="21759-143">Response</span></span>
<span data-ttu-id="21759-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="21759-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




