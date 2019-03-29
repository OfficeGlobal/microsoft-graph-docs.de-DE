---
title: TermsAndConditionsGroupAssignment aktualisieren
description: Aktualisieren der Eigenschaften eines termsAndConditionsGroupAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d76b67f72b18ed29cc98c4bad7c9c035b4ee01ca
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975882"
---
# <a name="update-termsandconditionsgroupassignment"></a><span data-ttu-id="5ff08-103">TermsAndConditionsGroupAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5ff08-103">Update termsAndConditionsGroupAssignment</span></span>

> <span data-ttu-id="5ff08-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5ff08-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ff08-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5ff08-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ff08-106">Aktualisieren der Eigenschaften eines [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5ff08-106">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ff08-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5ff08-107">Prerequisites</span></span>
<span data-ttu-id="5ff08-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ff08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ff08-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5ff08-110">Permission type</span></span>|<span data-ttu-id="5ff08-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5ff08-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ff08-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5ff08-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5ff08-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ff08-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5ff08-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5ff08-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ff08-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5ff08-115">Not supported.</span></span>|
|<span data-ttu-id="5ff08-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5ff08-116">Application</span></span>|<span data-ttu-id="5ff08-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5ff08-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ff08-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5ff08-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="5ff08-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5ff08-119">Request headers</span></span>
|<span data-ttu-id="5ff08-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5ff08-120">Header</span></span>|<span data-ttu-id="5ff08-121">Wert</span><span class="sxs-lookup"><span data-stu-id="5ff08-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ff08-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ff08-122">Authorization</span></span>|<span data-ttu-id="5ff08-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5ff08-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ff08-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5ff08-124">Accept</span></span>|<span data-ttu-id="5ff08-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5ff08-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ff08-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5ff08-126">Request body</span></span>
<span data-ttu-id="5ff08-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="5ff08-127">In the request body, supply a JSON representation for the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

<span data-ttu-id="5ff08-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="5ff08-128">The following table shows the properties that are required when you create the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>

|<span data-ttu-id="5ff08-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5ff08-129">Property</span></span>|<span data-ttu-id="5ff08-130">Typ</span><span class="sxs-lookup"><span data-stu-id="5ff08-130">Type</span></span>|<span data-ttu-id="5ff08-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5ff08-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ff08-132">id</span><span class="sxs-lookup"><span data-stu-id="5ff08-132">id</span></span>|<span data-ttu-id="5ff08-133">String</span><span class="sxs-lookup"><span data-stu-id="5ff08-133">String</span></span>|<span data-ttu-id="5ff08-134">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="5ff08-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="5ff08-135">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="5ff08-135">targetGroupId</span></span>|<span data-ttu-id="5ff08-136">String</span><span class="sxs-lookup"><span data-stu-id="5ff08-136">String</span></span>|<span data-ttu-id="5ff08-137">Eindeutiger Bezeichner einer Gruppe, der die T&C-Richtlinie zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="5ff08-137">Unique identifier of a group that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="5ff08-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="5ff08-138">Response</span></span>
<span data-ttu-id="5ff08-139">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5ff08-139">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ff08-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5ff08-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ff08-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5ff08-141">Request</span></span>
<span data-ttu-id="5ff08-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5ff08-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="5ff08-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="5ff08-143">Response</span></span>
<span data-ttu-id="5ff08-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5ff08-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 169

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "id": "2eb1aab7-aab7-2eb1-b7aa-b12eb7aab12e",
  "targetGroupId": "Target Group Id value"
}
```




