---
title: Aktualisieren von „termsAndConditions“
description: Aktualisieren der Eigenschaften eines termsAndConditions-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 688e0b980e468172fdfd6037327e1e543ae6fb3b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160200"
---
# <a name="update-termsandconditions"></a><span data-ttu-id="0c89b-103">Aktualisieren von „termsAndConditions“</span><span class="sxs-lookup"><span data-stu-id="0c89b-103">Update termsAndConditions</span></span>

> <span data-ttu-id="0c89b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0c89b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c89b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0c89b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c89b-106">Aktualisieren der Eigenschaften eines [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0c89b-106">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c89b-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0c89b-107">Prerequisites</span></span>
<span data-ttu-id="0c89b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0c89b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0c89b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0c89b-110">Permission type</span></span>|<span data-ttu-id="0c89b-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0c89b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c89b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0c89b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0c89b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c89b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0c89b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0c89b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c89b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0c89b-115">Not supported.</span></span>|
|<span data-ttu-id="0c89b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0c89b-116">Application</span></span>|<span data-ttu-id="0c89b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0c89b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c89b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0c89b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}/termsAndConditions
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="0c89b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0c89b-119">Request headers</span></span>
|<span data-ttu-id="0c89b-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0c89b-120">Header</span></span>|<span data-ttu-id="0c89b-121">Wert</span><span class="sxs-lookup"><span data-stu-id="0c89b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c89b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c89b-122">Authorization</span></span>|<span data-ttu-id="0c89b-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0c89b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c89b-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0c89b-124">Accept</span></span>|<span data-ttu-id="0c89b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0c89b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c89b-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0c89b-126">Request body</span></span>
<span data-ttu-id="0c89b-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="0c89b-127">In the request body, supply a JSON representation for the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

<span data-ttu-id="0c89b-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="0c89b-128">The following table shows the properties that are required when you create the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>

|<span data-ttu-id="0c89b-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0c89b-129">Property</span></span>|<span data-ttu-id="0c89b-130">Typ</span><span class="sxs-lookup"><span data-stu-id="0c89b-130">Type</span></span>|<span data-ttu-id="0c89b-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0c89b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c89b-132">id</span><span class="sxs-lookup"><span data-stu-id="0c89b-132">id</span></span>|<span data-ttu-id="0c89b-133">string</span><span class="sxs-lookup"><span data-stu-id="0c89b-133">String</span></span>|<span data-ttu-id="0c89b-134">Eindeutiger Bezeichner der Geschäftsbedingungen-Richtlinie</span><span class="sxs-lookup"><span data-stu-id="0c89b-134">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="0c89b-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0c89b-135">createdDateTime</span></span>|<span data-ttu-id="0c89b-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c89b-136">DateTimeOffset</span></span>|<span data-ttu-id="0c89b-137">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0c89b-137">DateTime the object was created.</span></span>|
|<span data-ttu-id="0c89b-138">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c89b-138">modifiedDateTime</span></span>|<span data-ttu-id="0c89b-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c89b-139">DateTimeOffset</span></span>|<span data-ttu-id="0c89b-140">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0c89b-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="0c89b-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c89b-141">lastModifiedDateTime</span></span>|<span data-ttu-id="0c89b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c89b-142">DateTimeOffset</span></span>|<span data-ttu-id="0c89b-143">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0c89b-143">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="0c89b-144">displayName</span><span class="sxs-lookup"><span data-stu-id="0c89b-144">displayName</span></span>|<span data-ttu-id="0c89b-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0c89b-145">String</span></span>|<span data-ttu-id="0c89b-146">Name der Geschäftsbedingungen-Richtlinie (vom Administrator festgelegt)</span><span class="sxs-lookup"><span data-stu-id="0c89b-146">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="0c89b-147">description</span><span class="sxs-lookup"><span data-stu-id="0c89b-147">description</span></span>|<span data-ttu-id="0c89b-148">String</span><span class="sxs-lookup"><span data-stu-id="0c89b-148">String</span></span>|<span data-ttu-id="0c89b-149">Beschreibung der Geschäftsbedingungen-Richtlinie (vom Administrator festgelegt)</span><span class="sxs-lookup"><span data-stu-id="0c89b-149">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="0c89b-150">title</span><span class="sxs-lookup"><span data-stu-id="0c89b-150">title</span></span>|<span data-ttu-id="0c89b-151">String</span><span class="sxs-lookup"><span data-stu-id="0c89b-151">String</span></span>|<span data-ttu-id="0c89b-152">Titel der Geschäftsbedingungen (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="0c89b-152">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="0c89b-153">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="0c89b-153">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="0c89b-154">bodyText</span><span class="sxs-lookup"><span data-stu-id="0c89b-154">bodyText</span></span>|<span data-ttu-id="0c89b-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0c89b-155">String</span></span>|<span data-ttu-id="0c89b-156">Text der Geschäftsbedingungen (vom Administrator festgelegt). In der Regel handelt es sich um die Bedingungen selbst.</span><span class="sxs-lookup"><span data-stu-id="0c89b-156">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="0c89b-157">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="0c89b-157">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="0c89b-158">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="0c89b-158">acceptanceStatement</span></span>|<span data-ttu-id="0c89b-159">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0c89b-159">String</span></span>|<span data-ttu-id="0c89b-160">Erläuterung der Geschäftsbedingungen (vom Administrator bereitgestellt). Sie beschreibt in der Regel, was es für den Benutzer bedeutet, wenn er die Geschäftsbedingungen in der Geschäftsbedingungen-Richtlinie annimmt.</span><span class="sxs-lookup"><span data-stu-id="0c89b-160">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="0c89b-161">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="0c89b-161">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="0c89b-162">Version</span><span class="sxs-lookup"><span data-stu-id="0c89b-162">version</span></span>|<span data-ttu-id="0c89b-163">Int32</span><span class="sxs-lookup"><span data-stu-id="0c89b-163">Int32</span></span>|<span data-ttu-id="0c89b-164">Ganze Zahl, die die aktuelle Version der Geschäftsbedingungen angibt.</span><span class="sxs-lookup"><span data-stu-id="0c89b-164">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="0c89b-165">Sie wird heraufgesetzt, wenn ein Administrator die Bedingungen ändert und festlegt, dass Benutzer die geänderte Geschäftsbedingungen-Richtlinie erneut annehmen müssen.</span><span class="sxs-lookup"><span data-stu-id="0c89b-165">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="0c89b-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="0c89b-166">Response</span></span>
<span data-ttu-id="0c89b-167">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0c89b-167">If successful, this method returns a `200 OK` response code and an updated [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c89b-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0c89b-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c89b-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0c89b-169">Request</span></span>
<span data-ttu-id="0c89b-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0c89b-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}
Content-type: application/json
Content-length: 273

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="0c89b-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="0c89b-171">Response</span></span>
<span data-ttu-id="0c89b-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0c89b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 505

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```




