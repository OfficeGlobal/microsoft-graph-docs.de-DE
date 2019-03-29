---
title: IosLobAppProvisioningConfigurationAssignment erstellen
description: Erstellen eines neuen iosLobAppProvisioningConfigurationAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4ba1a87dc27f61de5d3b5ea5c3a2f75dada49289
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960489"
---
# <a name="create-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="f17e2-103">IosLobAppProvisioningConfigurationAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="f17e2-103">Create iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="f17e2-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f17e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f17e2-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f17e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f17e2-106">Erstellen eines neuen [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f17e2-106">Create a new [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f17e2-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f17e2-107">Prerequisites</span></span>
<span data-ttu-id="f17e2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f17e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f17e2-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f17e2-110">Permission type</span></span>|<span data-ttu-id="f17e2-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f17e2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f17e2-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f17e2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f17e2-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f17e2-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f17e2-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f17e2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f17e2-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f17e2-115">Not supported.</span></span>|
|<span data-ttu-id="f17e2-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f17e2-116">Application</span></span>|<span data-ttu-id="f17e2-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f17e2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f17e2-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f17e2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="f17e2-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f17e2-119">Request headers</span></span>
|<span data-ttu-id="f17e2-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f17e2-120">Header</span></span>|<span data-ttu-id="f17e2-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f17e2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f17e2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f17e2-122">Authorization</span></span>|<span data-ttu-id="f17e2-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f17e2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f17e2-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f17e2-124">Accept</span></span>|<span data-ttu-id="f17e2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f17e2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f17e2-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f17e2-126">Request body</span></span>
<span data-ttu-id="f17e2-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das iosLobAppProvisioningConfigurationAssignment-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="f17e2-127">In the request body, supply a JSON representation for the iosLobAppProvisioningConfigurationAssignment object.</span></span>

<span data-ttu-id="f17e2-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der iosLobAppProvisioningConfigurationAssignment erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="f17e2-128">The following table shows the properties that are required when you create the iosLobAppProvisioningConfigurationAssignment.</span></span>

|<span data-ttu-id="f17e2-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f17e2-129">Property</span></span>|<span data-ttu-id="f17e2-130">Typ</span><span class="sxs-lookup"><span data-stu-id="f17e2-130">Type</span></span>|<span data-ttu-id="f17e2-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f17e2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f17e2-132">id</span><span class="sxs-lookup"><span data-stu-id="f17e2-132">id</span></span>|<span data-ttu-id="f17e2-133">String</span><span class="sxs-lookup"><span data-stu-id="f17e2-133">String</span></span>|<span data-ttu-id="f17e2-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f17e2-134">Key of the entity.</span></span>|
|<span data-ttu-id="f17e2-135">target</span><span class="sxs-lookup"><span data-stu-id="f17e2-135">target</span></span>|[<span data-ttu-id="f17e2-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f17e2-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="f17e2-137">Die vom Administrator definierte Zielgruppenzuordnung</span><span class="sxs-lookup"><span data-stu-id="f17e2-137">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="f17e2-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="f17e2-138">Response</span></span>
<span data-ttu-id="f17e2-139">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f17e2-139">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f17e2-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f17e2-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="f17e2-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f17e2-141">Request</span></span>
<span data-ttu-id="f17e2-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f17e2-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f17e2-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="f17e2-143">Response</span></span>
<span data-ttu-id="f17e2-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f17e2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




