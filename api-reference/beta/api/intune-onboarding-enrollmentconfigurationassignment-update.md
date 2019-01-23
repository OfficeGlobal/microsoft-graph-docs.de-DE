---
title: enrollmentConfigurationAssignment aktualisieren
description: Aktualisieren der Eigenschaften eines enrollmentConfigurationAssignment-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 928abb0869a401015a6485e240d5ebd2336a7d3f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403602"
---
# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="28601-103">enrollmentConfigurationAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="28601-103">Update enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="28601-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="28601-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="28601-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="28601-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="28601-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="28601-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28601-107">Aktualisieren der Eigenschaften eines [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="28601-107">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28601-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="28601-108">Prerequisites</span></span>
<span data-ttu-id="28601-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="28601-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="28601-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="28601-111">Permission type</span></span>|<span data-ttu-id="28601-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="28601-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28601-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="28601-113">Delegated (work or school account)</span></span>|<span data-ttu-id="28601-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28601-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="28601-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="28601-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28601-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="28601-116">Not supported.</span></span>|
|<span data-ttu-id="28601-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="28601-117">Application</span></span>|<span data-ttu-id="28601-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="28601-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28601-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="28601-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="28601-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="28601-120">Request headers</span></span>
|<span data-ttu-id="28601-121">Header</span><span class="sxs-lookup"><span data-stu-id="28601-121">Header</span></span>|<span data-ttu-id="28601-122">Wert</span><span class="sxs-lookup"><span data-stu-id="28601-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28601-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="28601-123">Authorization</span></span>|<span data-ttu-id="28601-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="28601-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28601-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="28601-125">Accept</span></span>|<span data-ttu-id="28601-126">application/json</span><span class="sxs-lookup"><span data-stu-id="28601-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28601-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="28601-127">Request body</span></span>
<span data-ttu-id="28601-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="28601-128">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="28601-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)-Objekts erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="28601-129">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="28601-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="28601-130">Property</span></span>|<span data-ttu-id="28601-131">Typ</span><span class="sxs-lookup"><span data-stu-id="28601-131">Type</span></span>|<span data-ttu-id="28601-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28601-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28601-133">id</span><span class="sxs-lookup"><span data-stu-id="28601-133">id</span></span>|<span data-ttu-id="28601-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="28601-134">String</span></span>|<span data-ttu-id="28601-135">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="28601-135">Not yet documented</span></span>|
|<span data-ttu-id="28601-136">target</span><span class="sxs-lookup"><span data-stu-id="28601-136">target</span></span>|[<span data-ttu-id="28601-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="28601-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="28601-138">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="28601-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="28601-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="28601-139">Response</span></span>
<span data-ttu-id="28601-140">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="28601-140">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28601-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="28601-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="28601-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="28601-142">Request</span></span>
<span data-ttu-id="28601-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="28601-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="28601-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="28601-144">Response</span></span>
<span data-ttu-id="28601-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="28601-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




