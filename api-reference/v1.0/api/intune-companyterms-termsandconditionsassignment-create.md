---
title: Erstellen von „termsAndConditionsAssignment“
description: Diese Methode erstellt ein neues Objekt des Typs termsAndConditionsAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2fba749b6963dd462740eacf772e6e864c77ab4d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947484"
---
# <a name="create-termsandconditionsassignment"></a><span data-ttu-id="7ff0c-103">Erstellen von „termsAndConditionsAssignment“</span><span class="sxs-lookup"><span data-stu-id="7ff0c-103">Create termsAndConditionsAssignment</span></span>

> <span data-ttu-id="7ff0c-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7ff0c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7ff0c-105">Diese Methode erstellt ein neues Objekt des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7ff0c-105">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7ff0c-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7ff0c-106">Prerequisites</span></span>
<span data-ttu-id="7ff0c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ff0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ff0c-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7ff0c-109">Permission type</span></span>|<span data-ttu-id="7ff0c-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7ff0c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ff0c-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7ff0c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7ff0c-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ff0c-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7ff0c-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7ff0c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ff0c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7ff0c-114">Not supported.</span></span>|
|<span data-ttu-id="7ff0c-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7ff0c-115">Application</span></span>|<span data-ttu-id="7ff0c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7ff0c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ff0c-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7ff0c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="7ff0c-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7ff0c-118">Request headers</span></span>
|<span data-ttu-id="7ff0c-119">Header</span><span class="sxs-lookup"><span data-stu-id="7ff0c-119">Header</span></span>|<span data-ttu-id="7ff0c-120">Wert</span><span class="sxs-lookup"><span data-stu-id="7ff0c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ff0c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ff0c-121">Authorization</span></span>|<span data-ttu-id="7ff0c-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7ff0c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ff0c-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7ff0c-123">Accept</span></span>|<span data-ttu-id="7ff0c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7ff0c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ff0c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7ff0c-125">Request body</span></span>
<span data-ttu-id="7ff0c-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „termsAndConditionsAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="7ff0c-126">In the request body, supply a JSON representation for the termsAndConditionsAssignment object.</span></span>

<span data-ttu-id="7ff0c-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „termsAndConditionsAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="7ff0c-127">The following table shows the properties that are required when you create the termsAndConditionsAssignment.</span></span>

|<span data-ttu-id="7ff0c-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7ff0c-128">Property</span></span>|<span data-ttu-id="7ff0c-129">Typ</span><span class="sxs-lookup"><span data-stu-id="7ff0c-129">Type</span></span>|<span data-ttu-id="7ff0c-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7ff0c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ff0c-131">id</span><span class="sxs-lookup"><span data-stu-id="7ff0c-131">id</span></span>|<span data-ttu-id="7ff0c-132">String</span><span class="sxs-lookup"><span data-stu-id="7ff0c-132">String</span></span>|<span data-ttu-id="7ff0c-133">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="7ff0c-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="7ff0c-134">target</span><span class="sxs-lookup"><span data-stu-id="7ff0c-134">target</span></span>|[<span data-ttu-id="7ff0c-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7ff0c-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7ff0c-136">Zuweisungsziel, dem die Geschäftsbedingungen-Richtlinie zugewiesen ist</span><span class="sxs-lookup"><span data-stu-id="7ff0c-136">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="7ff0c-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="7ff0c-137">Response</span></span>
<span data-ttu-id="7ff0c-138">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7ff0c-138">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ff0c-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7ff0c-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="7ff0c-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7ff0c-140">Request</span></span>
<span data-ttu-id="7ff0c-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7ff0c-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
Content-type: application/json
Content-length: 168

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="7ff0c-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="7ff0c-142">Response</span></span>
<span data-ttu-id="7ff0c-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7ff0c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



