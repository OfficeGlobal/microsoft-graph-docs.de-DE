---
title: enrollmentConfigurationAssignment erstellen
description: Erstellen eines neuen enrollmentConfigurationAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0910dcafd8888fcdae03f1efe23802246afac689
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979690"
---
# <a name="create-enrollmentconfigurationassignment"></a><span data-ttu-id="e9143-103">enrollmentConfigurationAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="e9143-103">Create enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="e9143-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e9143-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9143-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e9143-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9143-106">Erstellen eines neuen [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e9143-106">Create a new [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9143-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e9143-107">Prerequisites</span></span>
<span data-ttu-id="e9143-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9143-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9143-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e9143-110">Permission type</span></span>|<span data-ttu-id="e9143-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e9143-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9143-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e9143-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e9143-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9143-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e9143-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e9143-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9143-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e9143-115">Not supported.</span></span>|
|<span data-ttu-id="e9143-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e9143-116">Application</span></span>|<span data-ttu-id="e9143-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e9143-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9143-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e9143-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="e9143-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e9143-119">Request headers</span></span>
|<span data-ttu-id="e9143-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e9143-120">Header</span></span>|<span data-ttu-id="e9143-121">Wert</span><span class="sxs-lookup"><span data-stu-id="e9143-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9143-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9143-122">Authorization</span></span>|<span data-ttu-id="e9143-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e9143-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9143-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e9143-124">Accept</span></span>|<span data-ttu-id="e9143-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e9143-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9143-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e9143-126">Request body</span></span>
<span data-ttu-id="e9143-127">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs enrollmentConfigurationAssignment an.</span><span class="sxs-lookup"><span data-stu-id="e9143-127">In the request body, supply a JSON representation for the enrollmentConfigurationAssignment object.</span></span>

<span data-ttu-id="e9143-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des enrollmentConfigurationAssignment-Objekts erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e9143-128">The following table shows the properties that are required when you create the enrollmentConfigurationAssignment.</span></span>

|<span data-ttu-id="e9143-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e9143-129">Property</span></span>|<span data-ttu-id="e9143-130">Typ</span><span class="sxs-lookup"><span data-stu-id="e9143-130">Type</span></span>|<span data-ttu-id="e9143-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e9143-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9143-132">id</span><span class="sxs-lookup"><span data-stu-id="e9143-132">id</span></span>|<span data-ttu-id="e9143-133">String</span><span class="sxs-lookup"><span data-stu-id="e9143-133">String</span></span>|<span data-ttu-id="e9143-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e9143-134">Not yet documented</span></span>|
|<span data-ttu-id="e9143-135">target</span><span class="sxs-lookup"><span data-stu-id="e9143-135">target</span></span>|[<span data-ttu-id="e9143-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e9143-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e9143-137">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e9143-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e9143-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="e9143-138">Response</span></span>
<span data-ttu-id="e9143-139">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e9143-139">If successful, this method returns a `201 Created` response code and a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9143-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e9143-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9143-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e9143-141">Request</span></span>
<span data-ttu-id="e9143-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e9143-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="e9143-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="e9143-143">Response</span></span>
<span data-ttu-id="e9143-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e9143-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 222

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "705b021c-021c-705b-1c02-5b701c025b70",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




