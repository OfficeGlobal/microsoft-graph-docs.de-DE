---
title: Aktualisieren von „termsAndConditionsAssignment“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs termsAndConditionsAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 17051c4b665f171d6ce2d2c3fbe4c09acbe3fc45
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964976"
---
# <a name="update-termsandconditionsassignment"></a><span data-ttu-id="74577-103">Aktualisieren von „termsAndConditionsAssignment“</span><span class="sxs-lookup"><span data-stu-id="74577-103">Update termsAndConditionsAssignment</span></span>

> <span data-ttu-id="74577-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="74577-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74577-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="74577-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74577-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="74577-106">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74577-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="74577-107">Prerequisites</span></span>
<span data-ttu-id="74577-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74577-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74577-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="74577-110">Permission type</span></span>|<span data-ttu-id="74577-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="74577-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74577-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="74577-112">Delegated (work or school account)</span></span>|<span data-ttu-id="74577-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74577-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="74577-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="74577-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74577-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="74577-115">Not supported.</span></span>|
|<span data-ttu-id="74577-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="74577-116">Application</span></span>|<span data-ttu-id="74577-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="74577-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74577-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="74577-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="74577-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="74577-119">Request headers</span></span>
|<span data-ttu-id="74577-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="74577-120">Header</span></span>|<span data-ttu-id="74577-121">Wert</span><span class="sxs-lookup"><span data-stu-id="74577-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74577-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="74577-122">Authorization</span></span>|<span data-ttu-id="74577-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="74577-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74577-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="74577-124">Accept</span></span>|<span data-ttu-id="74577-125">application/json</span><span class="sxs-lookup"><span data-stu-id="74577-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74577-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="74577-126">Request body</span></span>
<span data-ttu-id="74577-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="74577-127">In the request body, supply a JSON representation for the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

<span data-ttu-id="74577-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="74577-128">The following table shows the properties that are required when you create the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>

|<span data-ttu-id="74577-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="74577-129">Property</span></span>|<span data-ttu-id="74577-130">Typ</span><span class="sxs-lookup"><span data-stu-id="74577-130">Type</span></span>|<span data-ttu-id="74577-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="74577-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74577-132">id</span><span class="sxs-lookup"><span data-stu-id="74577-132">id</span></span>|<span data-ttu-id="74577-133">String</span><span class="sxs-lookup"><span data-stu-id="74577-133">String</span></span>|<span data-ttu-id="74577-134">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="74577-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="74577-135">target</span><span class="sxs-lookup"><span data-stu-id="74577-135">target</span></span>|[<span data-ttu-id="74577-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="74577-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="74577-137">Zuweisungsziel, dem die Geschäftsbedingungen-Richtlinie zugewiesen ist</span><span class="sxs-lookup"><span data-stu-id="74577-137">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="74577-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="74577-138">Response</span></span>
<span data-ttu-id="74577-139">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="74577-139">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74577-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="74577-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="74577-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74577-141">Request</span></span>
<span data-ttu-id="74577-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="74577-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
Content-type: application/json
Content-length: 168

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="74577-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="74577-143">Response</span></span>
<span data-ttu-id="74577-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="74577-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 217

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




