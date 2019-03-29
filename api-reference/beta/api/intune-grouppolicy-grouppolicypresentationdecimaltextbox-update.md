---
title: GroupPolicyPresentationDecimalTextBox aktualisieren
description: Aktualisieren der Eigenschaften eines groupPolicyPresentationDecimalTextBox-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb4ee69c80664c8cd46dc6d5e711c57bb307e940
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962400"
---
# <a name="update-grouppolicypresentationdecimaltextbox"></a><span data-ttu-id="381b4-103">GroupPolicyPresentationDecimalTextBox aktualisieren</span><span class="sxs-lookup"><span data-stu-id="381b4-103">Update groupPolicyPresentationDecimalTextBox</span></span>

> <span data-ttu-id="381b4-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="381b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="381b4-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="381b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="381b4-106">Aktualisieren der Eigenschaften eines [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="381b4-106">Update the properties of a [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="381b4-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="381b4-107">Prerequisites</span></span>
<span data-ttu-id="381b4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="381b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="381b4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="381b4-110">Permission type</span></span>|<span data-ttu-id="381b4-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="381b4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="381b4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="381b4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="381b4-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="381b4-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="381b4-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="381b4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="381b4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="381b4-115">Not supported.</span></span>|
|<span data-ttu-id="381b4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="381b4-116">Application</span></span>|<span data-ttu-id="381b4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="381b4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="381b4-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="381b4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="381b4-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="381b4-119">Request headers</span></span>
|<span data-ttu-id="381b4-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="381b4-120">Header</span></span>|<span data-ttu-id="381b4-121">Wert</span><span class="sxs-lookup"><span data-stu-id="381b4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="381b4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="381b4-122">Authorization</span></span>|<span data-ttu-id="381b4-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="381b4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="381b4-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="381b4-124">Accept</span></span>|<span data-ttu-id="381b4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="381b4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="381b4-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="381b4-126">Request body</span></span>
<span data-ttu-id="381b4-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="381b4-127">In the request body, supply a JSON representation for the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

<span data-ttu-id="381b4-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="381b4-128">The following table shows the properties that are required when you create the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md).</span></span>

|<span data-ttu-id="381b4-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="381b4-129">Property</span></span>|<span data-ttu-id="381b4-130">Typ</span><span class="sxs-lookup"><span data-stu-id="381b4-130">Type</span></span>|<span data-ttu-id="381b4-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="381b4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="381b4-132">label</span><span class="sxs-lookup"><span data-stu-id="381b4-132">label</span></span>|<span data-ttu-id="381b4-133">String</span><span class="sxs-lookup"><span data-stu-id="381b4-133">String</span></span>|<span data-ttu-id="381b4-134">Lokalisierte Textbezeichnung für eine beliebige Präsentations Entität.</span><span class="sxs-lookup"><span data-stu-id="381b4-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="381b4-135">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="381b4-135">The default value is empty.</span></span> <span data-ttu-id="381b4-136">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="381b4-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="381b4-137">id</span><span class="sxs-lookup"><span data-stu-id="381b4-137">id</span></span>|<span data-ttu-id="381b4-138">String</span><span class="sxs-lookup"><span data-stu-id="381b4-138">String</span></span>|<span data-ttu-id="381b4-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="381b4-139">Key of the entity.</span></span> <span data-ttu-id="381b4-140">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="381b4-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="381b4-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="381b4-141">lastModifiedDateTime</span></span>|<span data-ttu-id="381b4-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="381b4-142">DateTimeOffset</span></span>|<span data-ttu-id="381b4-143">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="381b4-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="381b4-144">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="381b4-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="381b4-145">defaultValue</span><span class="sxs-lookup"><span data-stu-id="381b4-145">defaultValue</span></span>|<span data-ttu-id="381b4-146">Int64</span><span class="sxs-lookup"><span data-stu-id="381b4-146">Int64</span></span>|<span data-ttu-id="381b4-147">Eine ganze Zahl ohne Vorzeichen, die den Anfangswert für das Dezimal Textfeld angibt.</span><span class="sxs-lookup"><span data-stu-id="381b4-147">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="381b4-148">Der Standardwert ist 1.</span><span class="sxs-lookup"><span data-stu-id="381b4-148">The default value is 1.</span></span>|
|<span data-ttu-id="381b4-149">Spin</span><span class="sxs-lookup"><span data-stu-id="381b4-149">spin</span></span>|<span data-ttu-id="381b4-150">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="381b4-150">Boolean</span></span>|<span data-ttu-id="381b4-151">Wenn true, erstellen Sie ein Drehfeld-Steuerelement; Erstellen Sie andernfalls ein Textfeld für die numerische Eingabe.</span><span class="sxs-lookup"><span data-stu-id="381b4-151">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="381b4-152">Der Standardwert ist "True".</span><span class="sxs-lookup"><span data-stu-id="381b4-152">The default value is true.</span></span>|
|<span data-ttu-id="381b4-153">spinStep</span><span class="sxs-lookup"><span data-stu-id="381b4-153">spinStep</span></span>|<span data-ttu-id="381b4-154">Int64</span><span class="sxs-lookup"><span data-stu-id="381b4-154">Int64</span></span>|<span data-ttu-id="381b4-155">Eine ganze Zahl ohne Vorzeichen, die die Schrittweite der Änderung für das Drehfeld-Steuerelement angibt.</span><span class="sxs-lookup"><span data-stu-id="381b4-155">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="381b4-156">Der Standardwert ist 1.</span><span class="sxs-lookup"><span data-stu-id="381b4-156">The default value is 1.</span></span>|
|<span data-ttu-id="381b4-157">erforderlich</span><span class="sxs-lookup"><span data-stu-id="381b4-157">required</span></span>|<span data-ttu-id="381b4-158">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="381b4-158">Boolean</span></span>|<span data-ttu-id="381b4-159">Anforderung zur Eingabe eines Werts im Parameterfeld.</span><span class="sxs-lookup"><span data-stu-id="381b4-159">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="381b4-160">Der Standardwert ist false.</span><span class="sxs-lookup"><span data-stu-id="381b4-160">The default value is false.</span></span>|
|<span data-ttu-id="381b4-161">minValue</span><span class="sxs-lookup"><span data-stu-id="381b4-161">minValue</span></span>|<span data-ttu-id="381b4-162">Int64</span><span class="sxs-lookup"><span data-stu-id="381b4-162">Int64</span></span>|<span data-ttu-id="381b4-163">Eine ganze Zahl ohne Vorzeichen, die den minimal zulässigen Wert angibt.</span><span class="sxs-lookup"><span data-stu-id="381b4-163">An unsigned integer that specifies the minimum allowed value.</span></span> <span data-ttu-id="381b4-164">Der Standardwert ist 0.</span><span class="sxs-lookup"><span data-stu-id="381b4-164">The default value is 0.</span></span>|
|<span data-ttu-id="381b4-165">maxValue</span><span class="sxs-lookup"><span data-stu-id="381b4-165">maxValue</span></span>|<span data-ttu-id="381b4-166">Int64</span><span class="sxs-lookup"><span data-stu-id="381b4-166">Int64</span></span>|<span data-ttu-id="381b4-167">Eine ganze Zahl ohne Vorzeichen, die den maximal zulässigen Wert angibt.</span><span class="sxs-lookup"><span data-stu-id="381b4-167">An unsigned integer that specifies the maximum allowed value.</span></span> <span data-ttu-id="381b4-168">Der Standardwert ist 9999.</span><span class="sxs-lookup"><span data-stu-id="381b4-168">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="381b4-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="381b4-169">Response</span></span>
<span data-ttu-id="381b4-170">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="381b4-170">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="381b4-171">Beispiel</span><span class="sxs-lookup"><span data-stu-id="381b4-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="381b4-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="381b4-172">Request</span></span>
<span data-ttu-id="381b4-173">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="381b4-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 221

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDecimalTextBox",
  "label": "Label value",
  "defaultValue": 12,
  "spin": true,
  "spinStep": 8,
  "required": true,
  "minValue": 8,
  "maxValue": 8
}
```

### <a name="response"></a><span data-ttu-id="381b4-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="381b4-174">Response</span></span>
<span data-ttu-id="381b4-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="381b4-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 334

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDecimalTextBox",
  "label": "Label value",
  "id": "988daea7-aea7-988d-a7ae-8d98a7ae8d98",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": 12,
  "spin": true,
  "spinStep": 8,
  "required": true,
  "minValue": 8,
  "maxValue": 8
}
```




