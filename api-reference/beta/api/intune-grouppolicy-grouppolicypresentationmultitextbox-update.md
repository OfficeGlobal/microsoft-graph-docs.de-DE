---
title: GroupPolicyPresentationMultiTextBox aktualisieren
description: Aktualisieren der Eigenschaften eines groupPolicyPresentationMultiTextBox-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ce98df8c43404516d403eb767d195213ecbe5348
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972361"
---
# <a name="update-grouppolicypresentationmultitextbox"></a><span data-ttu-id="d32a9-103">GroupPolicyPresentationMultiTextBox aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d32a9-103">Update groupPolicyPresentationMultiTextBox</span></span>

> <span data-ttu-id="d32a9-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d32a9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d32a9-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d32a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d32a9-106">Aktualisieren der Eigenschaften eines [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d32a9-106">Update the properties of a [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d32a9-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d32a9-107">Prerequisites</span></span>
<span data-ttu-id="d32a9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d32a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d32a9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d32a9-110">Permission type</span></span>|<span data-ttu-id="d32a9-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d32a9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d32a9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d32a9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d32a9-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d32a9-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d32a9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d32a9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d32a9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d32a9-115">Not supported.</span></span>|
|<span data-ttu-id="d32a9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d32a9-116">Application</span></span>|<span data-ttu-id="d32a9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d32a9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d32a9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d32a9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="d32a9-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d32a9-119">Request headers</span></span>
|<span data-ttu-id="d32a9-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d32a9-120">Header</span></span>|<span data-ttu-id="d32a9-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d32a9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d32a9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d32a9-122">Authorization</span></span>|<span data-ttu-id="d32a9-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d32a9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d32a9-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d32a9-124">Accept</span></span>|<span data-ttu-id="d32a9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d32a9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d32a9-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d32a9-126">Request body</span></span>
<span data-ttu-id="d32a9-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="d32a9-127">In the request body, supply a JSON representation for the [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

<span data-ttu-id="d32a9-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="d32a9-128">The following table shows the properties that are required when you create the [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md).</span></span>

|<span data-ttu-id="d32a9-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d32a9-129">Property</span></span>|<span data-ttu-id="d32a9-130">Typ</span><span class="sxs-lookup"><span data-stu-id="d32a9-130">Type</span></span>|<span data-ttu-id="d32a9-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d32a9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d32a9-132">label</span><span class="sxs-lookup"><span data-stu-id="d32a9-132">label</span></span>|<span data-ttu-id="d32a9-133">String</span><span class="sxs-lookup"><span data-stu-id="d32a9-133">String</span></span>|<span data-ttu-id="d32a9-134">Lokalisierte Textbezeichnung für eine beliebige Präsentations Entität.</span><span class="sxs-lookup"><span data-stu-id="d32a9-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="d32a9-135">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="d32a9-135">The default value is empty.</span></span> <span data-ttu-id="d32a9-136">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="d32a9-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="d32a9-137">id</span><span class="sxs-lookup"><span data-stu-id="d32a9-137">id</span></span>|<span data-ttu-id="d32a9-138">String</span><span class="sxs-lookup"><span data-stu-id="d32a9-138">String</span></span>|<span data-ttu-id="d32a9-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d32a9-139">Key of the entity.</span></span> <span data-ttu-id="d32a9-140">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="d32a9-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="d32a9-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d32a9-141">lastModifiedDateTime</span></span>|<span data-ttu-id="d32a9-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d32a9-142">DateTimeOffset</span></span>|<span data-ttu-id="d32a9-143">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="d32a9-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="d32a9-144">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="d32a9-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="d32a9-145">erforderlich</span><span class="sxs-lookup"><span data-stu-id="d32a9-145">required</span></span>|<span data-ttu-id="d32a9-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d32a9-146">Boolean</span></span>|<span data-ttu-id="d32a9-147">Anforderung zur Eingabe eines Werts in das Textfeld.</span><span class="sxs-lookup"><span data-stu-id="d32a9-147">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="d32a9-148">Standardwert ist "false".</span><span class="sxs-lookup"><span data-stu-id="d32a9-148">Default value is false.</span></span>|
|<span data-ttu-id="d32a9-149">maxLength</span><span class="sxs-lookup"><span data-stu-id="d32a9-149">maxLength</span></span>|<span data-ttu-id="d32a9-150">Int64</span><span class="sxs-lookup"><span data-stu-id="d32a9-150">Int64</span></span>|<span data-ttu-id="d32a9-151">Eine ganze Zahl ohne Vorzeichen, die die maximale Anzahl von Textzeichen angibt.</span><span class="sxs-lookup"><span data-stu-id="d32a9-151">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="d32a9-152">Der Standardwert ist 1023.</span><span class="sxs-lookup"><span data-stu-id="d32a9-152">Default value is 1023.</span></span>|
|<span data-ttu-id="d32a9-153">maxStrings</span><span class="sxs-lookup"><span data-stu-id="d32a9-153">maxStrings</span></span>|<span data-ttu-id="d32a9-154">Int64</span><span class="sxs-lookup"><span data-stu-id="d32a9-154">Int64</span></span>|<span data-ttu-id="d32a9-155">Eine ganze Zahl ohne Vorzeichen, die die maximale Anzahl von Zeichenfolgen angibt.</span><span class="sxs-lookup"><span data-stu-id="d32a9-155">An unsigned integer that specifies the maximum number of strings.</span></span> <span data-ttu-id="d32a9-156">Der Standardwert ist 0.</span><span class="sxs-lookup"><span data-stu-id="d32a9-156">Default value is 0.</span></span>|



## <a name="response"></a><span data-ttu-id="d32a9-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="d32a9-157">Response</span></span>
<span data-ttu-id="d32a9-158">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d32a9-158">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d32a9-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d32a9-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="d32a9-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d32a9-160">Request</span></span>
<span data-ttu-id="d32a9-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d32a9-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 165

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
  "label": "Label value",
  "required": true,
  "maxLength": 9,
  "maxStrings": 10
}
```

### <a name="response"></a><span data-ttu-id="d32a9-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="d32a9-162">Response</span></span>
<span data-ttu-id="d32a9-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d32a9-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 278

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
  "label": "Label value",
  "id": "381ac035-c035-381a-35c0-1a3835c01a38",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "required": true,
  "maxLength": 9,
  "maxStrings": 10
}
```




