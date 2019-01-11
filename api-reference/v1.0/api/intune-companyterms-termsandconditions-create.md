---
title: Erstellen von „termsAndConditions“
description: Diese Methode erstellt ein neues Objekt des Typs termsAndConditions.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f2cd2350f3faa04883e3e65312b103c7cef96d41
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835847"
---
# <a name="create-termsandconditions"></a><span data-ttu-id="21903-103">Erstellen von „termsAndConditions“</span><span class="sxs-lookup"><span data-stu-id="21903-103">Create termsAndConditions</span></span>

> <span data-ttu-id="21903-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="21903-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21903-105">Diese Methode erstellt ein neues Objekt des Typs [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="21903-105">Create a new [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="21903-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="21903-106">Prerequisites</span></span>
<span data-ttu-id="21903-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21903-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21903-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="21903-109">Permission type</span></span>|<span data-ttu-id="21903-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="21903-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21903-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="21903-111">Delegated (work or school account)</span></span>|<span data-ttu-id="21903-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21903-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="21903-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="21903-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21903-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="21903-114">Not supported.</span></span>|
|<span data-ttu-id="21903-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="21903-115">Application</span></span>|<span data-ttu-id="21903-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="21903-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21903-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="21903-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="21903-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="21903-118">Request headers</span></span>
|<span data-ttu-id="21903-119">Header</span><span class="sxs-lookup"><span data-stu-id="21903-119">Header</span></span>|<span data-ttu-id="21903-120">Wert</span><span class="sxs-lookup"><span data-stu-id="21903-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21903-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="21903-121">Authorization</span></span>|<span data-ttu-id="21903-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="21903-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21903-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="21903-123">Accept</span></span>|<span data-ttu-id="21903-124">application/json</span><span class="sxs-lookup"><span data-stu-id="21903-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21903-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="21903-125">Request body</span></span>
<span data-ttu-id="21903-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „termsAndConditions“ an.</span><span class="sxs-lookup"><span data-stu-id="21903-126">In the request body, supply a JSON representation for the termsAndConditions object.</span></span>

<span data-ttu-id="21903-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „termsAndConditions“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="21903-127">The following table shows the properties that are required when you create the termsAndConditions.</span></span>

|<span data-ttu-id="21903-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="21903-128">Property</span></span>|<span data-ttu-id="21903-129">Typ</span><span class="sxs-lookup"><span data-stu-id="21903-129">Type</span></span>|<span data-ttu-id="21903-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="21903-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21903-131">id</span><span class="sxs-lookup"><span data-stu-id="21903-131">id</span></span>|<span data-ttu-id="21903-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21903-132">String</span></span>|<span data-ttu-id="21903-133">Eindeutiger Bezeichner der Geschäftsbedingungen-Richtlinie</span><span class="sxs-lookup"><span data-stu-id="21903-133">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="21903-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="21903-134">createdDateTime</span></span>|<span data-ttu-id="21903-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21903-135">DateTimeOffset</span></span>|<span data-ttu-id="21903-136">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="21903-136">DateTime the object was created.</span></span>|
|<span data-ttu-id="21903-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="21903-137">lastModifiedDateTime</span></span>|<span data-ttu-id="21903-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21903-138">DateTimeOffset</span></span>|<span data-ttu-id="21903-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="21903-139">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="21903-140">displayName</span><span class="sxs-lookup"><span data-stu-id="21903-140">displayName</span></span>|<span data-ttu-id="21903-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21903-141">String</span></span>|<span data-ttu-id="21903-142">Name der Geschäftsbedingungen-Richtlinie (vom Administrator festgelegt)</span><span class="sxs-lookup"><span data-stu-id="21903-142">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="21903-143">description</span><span class="sxs-lookup"><span data-stu-id="21903-143">description</span></span>|<span data-ttu-id="21903-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21903-144">String</span></span>|<span data-ttu-id="21903-145">Beschreibung der Geschäftsbedingungen-Richtlinie (vom Administrator festgelegt)</span><span class="sxs-lookup"><span data-stu-id="21903-145">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="21903-146">title</span><span class="sxs-lookup"><span data-stu-id="21903-146">title</span></span>|<span data-ttu-id="21903-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21903-147">String</span></span>|<span data-ttu-id="21903-148">Titel der Geschäftsbedingungen (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="21903-148">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="21903-149">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="21903-149">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="21903-150">bodyText</span><span class="sxs-lookup"><span data-stu-id="21903-150">bodyText</span></span>|<span data-ttu-id="21903-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21903-151">String</span></span>|<span data-ttu-id="21903-152">Text der Geschäftsbedingungen (vom Administrator festgelegt). In der Regel handelt es sich um die Bedingungen selbst.</span><span class="sxs-lookup"><span data-stu-id="21903-152">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="21903-153">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="21903-153">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="21903-154">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="21903-154">acceptanceStatement</span></span>|<span data-ttu-id="21903-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21903-155">String</span></span>|<span data-ttu-id="21903-156">Erläuterung der Geschäftsbedingungen (vom Administrator bereitgestellt). Sie beschreibt in der Regel, was es für den Benutzer bedeutet, wenn er die Geschäftsbedingungen in der Geschäftsbedingungen-Richtlinie annimmt.</span><span class="sxs-lookup"><span data-stu-id="21903-156">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="21903-157">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="21903-157">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="21903-158">Version</span><span class="sxs-lookup"><span data-stu-id="21903-158">version</span></span>|<span data-ttu-id="21903-159">Int32</span><span class="sxs-lookup"><span data-stu-id="21903-159">Int32</span></span>|<span data-ttu-id="21903-160">Ganze Zahl, die die aktuelle Version der Geschäftsbedingungen angibt.</span><span class="sxs-lookup"><span data-stu-id="21903-160">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="21903-161">Sie wird heraufgesetzt, wenn ein Administrator die Bedingungen ändert und festlegt, dass Benutzer die geänderte Geschäftsbedingungen-Richtlinie erneut annehmen müssen.</span><span class="sxs-lookup"><span data-stu-id="21903-161">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="21903-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="21903-162">Response</span></span>
<span data-ttu-id="21903-163">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="21903-163">If successful, this method returns a `201 Created` response code and a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21903-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="21903-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="21903-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="21903-165">Request</span></span>
<span data-ttu-id="21903-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="21903-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions
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

### <a name="response"></a><span data-ttu-id="21903-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="21903-167">Response</span></span>
<span data-ttu-id="21903-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="21903-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 445

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```



