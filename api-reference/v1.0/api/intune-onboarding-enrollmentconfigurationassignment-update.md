---
title: enrollmentConfigurationAssignment aktualisieren
description: Aktualisieren der Eigenschaften eines enrollmentConfigurationAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9ff6d9a778390b319338f253d94b50ffc6386dee
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969764"
---
# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="02b92-103">enrollmentConfigurationAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="02b92-103">Update enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="02b92-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="02b92-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02b92-105">Aktualisieren der Eigenschaften eines [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="02b92-105">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02b92-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="02b92-106">Prerequisites</span></span>
<span data-ttu-id="02b92-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02b92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02b92-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="02b92-109">Permission type</span></span>|<span data-ttu-id="02b92-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="02b92-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02b92-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="02b92-111">Delegated (work or school account)</span></span>|<span data-ttu-id="02b92-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02b92-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="02b92-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="02b92-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02b92-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="02b92-114">Not supported.</span></span>|
|<span data-ttu-id="02b92-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="02b92-115">Application</span></span>|<span data-ttu-id="02b92-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="02b92-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02b92-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="02b92-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="02b92-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="02b92-118">Request headers</span></span>
|<span data-ttu-id="02b92-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="02b92-119">Header</span></span>|<span data-ttu-id="02b92-120">Wert</span><span class="sxs-lookup"><span data-stu-id="02b92-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02b92-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="02b92-121">Authorization</span></span>|<span data-ttu-id="02b92-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="02b92-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02b92-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="02b92-123">Accept</span></span>|<span data-ttu-id="02b92-124">application/json</span><span class="sxs-lookup"><span data-stu-id="02b92-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02b92-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="02b92-125">Request body</span></span>
<span data-ttu-id="02b92-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="02b92-126">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="02b92-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)-Objekts erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="02b92-127">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="02b92-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="02b92-128">Property</span></span>|<span data-ttu-id="02b92-129">Typ</span><span class="sxs-lookup"><span data-stu-id="02b92-129">Type</span></span>|<span data-ttu-id="02b92-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="02b92-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02b92-131">id</span><span class="sxs-lookup"><span data-stu-id="02b92-131">id</span></span>|<span data-ttu-id="02b92-132">String</span><span class="sxs-lookup"><span data-stu-id="02b92-132">String</span></span>|<span data-ttu-id="02b92-133">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="02b92-133">Not yet documented</span></span>|
|<span data-ttu-id="02b92-134">target</span><span class="sxs-lookup"><span data-stu-id="02b92-134">target</span></span>|[<span data-ttu-id="02b92-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="02b92-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="02b92-136">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="02b92-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="02b92-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="02b92-137">Response</span></span>
<span data-ttu-id="02b92-138">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="02b92-138">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02b92-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="02b92-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="02b92-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="02b92-140">Request</span></span>
<span data-ttu-id="02b92-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="02b92-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="02b92-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="02b92-142">Response</span></span>
<span data-ttu-id="02b92-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="02b92-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



