---
title: Erstellen von „termsAndConditions“
description: Diese Methode erstellt ein neues Objekt des Typs termsAndConditions.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 262390218470408edbf7d63ee00142c9b8e2b789
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972271"
---
# <a name="create-termsandconditions"></a><span data-ttu-id="8696b-103">Erstellen von „termsAndConditions“</span><span class="sxs-lookup"><span data-stu-id="8696b-103">Create termsAndConditions</span></span>

> <span data-ttu-id="8696b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8696b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8696b-105">Diese Methode erstellt ein neues Objekt des Typs [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="8696b-105">Create a new [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8696b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8696b-106">Prerequisites</span></span>
<span data-ttu-id="8696b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8696b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8696b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8696b-109">Permission type</span></span>|<span data-ttu-id="8696b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8696b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8696b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8696b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8696b-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8696b-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8696b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8696b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8696b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8696b-114">Not supported.</span></span>|
|<span data-ttu-id="8696b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8696b-115">Application</span></span>|<span data-ttu-id="8696b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8696b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8696b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8696b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="8696b-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8696b-118">Request headers</span></span>
|<span data-ttu-id="8696b-119">Header</span><span class="sxs-lookup"><span data-stu-id="8696b-119">Header</span></span>|<span data-ttu-id="8696b-120">Wert</span><span class="sxs-lookup"><span data-stu-id="8696b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8696b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8696b-121">Authorization</span></span>|<span data-ttu-id="8696b-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8696b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8696b-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8696b-123">Accept</span></span>|<span data-ttu-id="8696b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8696b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8696b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8696b-125">Request body</span></span>
<span data-ttu-id="8696b-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „termsAndConditions“ an.</span><span class="sxs-lookup"><span data-stu-id="8696b-126">In the request body, supply a JSON representation for the termsAndConditions object.</span></span>

<span data-ttu-id="8696b-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „termsAndConditions“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="8696b-127">The following table shows the properties that are required when you create the termsAndConditions.</span></span>

|<span data-ttu-id="8696b-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8696b-128">Property</span></span>|<span data-ttu-id="8696b-129">Typ</span><span class="sxs-lookup"><span data-stu-id="8696b-129">Type</span></span>|<span data-ttu-id="8696b-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8696b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8696b-131">id</span><span class="sxs-lookup"><span data-stu-id="8696b-131">id</span></span>|<span data-ttu-id="8696b-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8696b-132">String</span></span>|<span data-ttu-id="8696b-133">Eindeutiger Bezeichner der Geschäftsbedingungen-Richtlinie</span><span class="sxs-lookup"><span data-stu-id="8696b-133">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="8696b-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8696b-134">createdDateTime</span></span>|<span data-ttu-id="8696b-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8696b-135">DateTimeOffset</span></span>|<span data-ttu-id="8696b-136">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8696b-136">DateTime the object was created.</span></span>|
|<span data-ttu-id="8696b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8696b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8696b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8696b-138">DateTimeOffset</span></span>|<span data-ttu-id="8696b-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="8696b-139">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="8696b-140">displayName</span><span class="sxs-lookup"><span data-stu-id="8696b-140">displayName</span></span>|<span data-ttu-id="8696b-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8696b-141">String</span></span>|<span data-ttu-id="8696b-142">Name der Geschäftsbedingungen-Richtlinie (vom Administrator festgelegt)</span><span class="sxs-lookup"><span data-stu-id="8696b-142">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="8696b-143">description</span><span class="sxs-lookup"><span data-stu-id="8696b-143">description</span></span>|<span data-ttu-id="8696b-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8696b-144">String</span></span>|<span data-ttu-id="8696b-145">Beschreibung der Geschäftsbedingungen-Richtlinie (vom Administrator festgelegt)</span><span class="sxs-lookup"><span data-stu-id="8696b-145">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="8696b-146">title</span><span class="sxs-lookup"><span data-stu-id="8696b-146">title</span></span>|<span data-ttu-id="8696b-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8696b-147">String</span></span>|<span data-ttu-id="8696b-148">Titel der Geschäftsbedingungen (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="8696b-148">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="8696b-149">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="8696b-149">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="8696b-150">bodyText</span><span class="sxs-lookup"><span data-stu-id="8696b-150">bodyText</span></span>|<span data-ttu-id="8696b-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8696b-151">String</span></span>|<span data-ttu-id="8696b-152">Text der Geschäftsbedingungen (vom Administrator festgelegt). In der Regel handelt es sich um die Bedingungen selbst.</span><span class="sxs-lookup"><span data-stu-id="8696b-152">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="8696b-153">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="8696b-153">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="8696b-154">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="8696b-154">acceptanceStatement</span></span>|<span data-ttu-id="8696b-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8696b-155">String</span></span>|<span data-ttu-id="8696b-156">Erläuterung der Geschäftsbedingungen (vom Administrator bereitgestellt). Sie beschreibt in der Regel, was es für den Benutzer bedeutet, wenn er die Geschäftsbedingungen in der Geschäftsbedingungen-Richtlinie annimmt.</span><span class="sxs-lookup"><span data-stu-id="8696b-156">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="8696b-157">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="8696b-157">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="8696b-158">Version</span><span class="sxs-lookup"><span data-stu-id="8696b-158">version</span></span>|<span data-ttu-id="8696b-159">Int32</span><span class="sxs-lookup"><span data-stu-id="8696b-159">Int32</span></span>|<span data-ttu-id="8696b-160">Ganze Zahl, die die aktuelle Version der Geschäftsbedingungen angibt.</span><span class="sxs-lookup"><span data-stu-id="8696b-160">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="8696b-161">Sie wird heraufgesetzt, wenn ein Administrator die Bedingungen ändert und festlegt, dass Benutzer die geänderte Geschäftsbedingungen-Richtlinie erneut annehmen müssen.</span><span class="sxs-lookup"><span data-stu-id="8696b-161">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="8696b-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="8696b-162">Response</span></span>
<span data-ttu-id="8696b-163">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8696b-163">If successful, this method returns a `201 Created` response code and a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8696b-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8696b-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="8696b-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8696b-165">Request</span></span>
<span data-ttu-id="8696b-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8696b-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8696b-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="8696b-167">Response</span></span>
<span data-ttu-id="8696b-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8696b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



