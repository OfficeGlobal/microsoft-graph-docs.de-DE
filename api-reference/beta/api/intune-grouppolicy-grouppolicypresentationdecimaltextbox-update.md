---
title: GroupPolicyPresentationDecimalTextBox aktualisieren
description: Aktualisieren der Eigenschaften eines groupPolicyPresentationDecimalTextBox-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 67a535327d62ccdb8901ed0776ab1b992641ccf7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154978"
---
# <a name="update-grouppolicypresentationdecimaltextbox"></a><span data-ttu-id="728be-103">GroupPolicyPresentationDecimalTextBox aktualisieren</span><span class="sxs-lookup"><span data-stu-id="728be-103">Update groupPolicyPresentationDecimalTextBox</span></span>

> <span data-ttu-id="728be-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="728be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="728be-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="728be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="728be-106">Aktualisieren der Eigenschaften eines [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="728be-106">Update the properties of a [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="728be-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="728be-107">Prerequisites</span></span>
<span data-ttu-id="728be-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="728be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="728be-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="728be-110">Permission type</span></span>|<span data-ttu-id="728be-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="728be-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="728be-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="728be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="728be-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="728be-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="728be-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="728be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="728be-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="728be-115">Not supported.</span></span>|
|<span data-ttu-id="728be-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="728be-116">Application</span></span>|<span data-ttu-id="728be-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="728be-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="728be-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="728be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="728be-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="728be-119">Request headers</span></span>
|<span data-ttu-id="728be-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="728be-120">Header</span></span>|<span data-ttu-id="728be-121">Wert</span><span class="sxs-lookup"><span data-stu-id="728be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="728be-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="728be-122">Authorization</span></span>|<span data-ttu-id="728be-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="728be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="728be-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="728be-124">Accept</span></span>|<span data-ttu-id="728be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="728be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="728be-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="728be-126">Request body</span></span>
<span data-ttu-id="728be-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="728be-127">In the request body, supply a JSON representation for the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

<span data-ttu-id="728be-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="728be-128">The following table shows the properties that are required when you create the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md).</span></span>

|<span data-ttu-id="728be-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="728be-129">Property</span></span>|<span data-ttu-id="728be-130">Typ</span><span class="sxs-lookup"><span data-stu-id="728be-130">Type</span></span>|<span data-ttu-id="728be-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="728be-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="728be-132">label</span><span class="sxs-lookup"><span data-stu-id="728be-132">label</span></span>|<span data-ttu-id="728be-133">String</span><span class="sxs-lookup"><span data-stu-id="728be-133">String</span></span>|<span data-ttu-id="728be-134">Lokalisierte Textbezeichnung für eine beliebige Präsentations Entität.</span><span class="sxs-lookup"><span data-stu-id="728be-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="728be-135">Der Standardwert ist Empty.</span><span class="sxs-lookup"><span data-stu-id="728be-135">The default value is empty.</span></span> <span data-ttu-id="728be-136">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="728be-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="728be-137">id</span><span class="sxs-lookup"><span data-stu-id="728be-137">id</span></span>|<span data-ttu-id="728be-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="728be-138">String</span></span>|<span data-ttu-id="728be-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="728be-139">Key of the entity.</span></span> <span data-ttu-id="728be-140">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="728be-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="728be-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="728be-141">lastModifiedDateTime</span></span>|<span data-ttu-id="728be-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="728be-142">DateTimeOffset</span></span>|<span data-ttu-id="728be-143">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="728be-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="728be-144">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="728be-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="728be-145">defaultValue</span><span class="sxs-lookup"><span data-stu-id="728be-145">defaultValue</span></span>|<span data-ttu-id="728be-146">Int64</span><span class="sxs-lookup"><span data-stu-id="728be-146">Int64</span></span>|<span data-ttu-id="728be-147">Eine ganze Zahl ohne Vorzeichen, die den Anfangswert für das Dezimal Textfeld angibt.</span><span class="sxs-lookup"><span data-stu-id="728be-147">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="728be-148">Der Standardwert ist 1.</span><span class="sxs-lookup"><span data-stu-id="728be-148">The default value is 1.</span></span>|
|<span data-ttu-id="728be-149">Spin</span><span class="sxs-lookup"><span data-stu-id="728be-149">spin</span></span>|<span data-ttu-id="728be-150">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="728be-150">Boolean</span></span>|<span data-ttu-id="728be-151">Wenn true, erstellen Sie ein Drehfeld-Steuerelement; Erstellen Sie andernfalls ein Textfeld für die numerische Eingabe.</span><span class="sxs-lookup"><span data-stu-id="728be-151">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="728be-152">Der Standardwert ist true.</span><span class="sxs-lookup"><span data-stu-id="728be-152">The default value is true.</span></span>|
|<span data-ttu-id="728be-153">spinStep</span><span class="sxs-lookup"><span data-stu-id="728be-153">spinStep</span></span>|<span data-ttu-id="728be-154">Int64</span><span class="sxs-lookup"><span data-stu-id="728be-154">Int64</span></span>|<span data-ttu-id="728be-155">Eine ganze Zahl ohne Vorzeichen, die die Schrittweite der Änderung für das Drehfeld-Steuerelement angibt.</span><span class="sxs-lookup"><span data-stu-id="728be-155">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="728be-156">Der Standardwert ist 1.</span><span class="sxs-lookup"><span data-stu-id="728be-156">The default value is 1.</span></span>|
|<span data-ttu-id="728be-157">erforderlich</span><span class="sxs-lookup"><span data-stu-id="728be-157">required</span></span>|<span data-ttu-id="728be-158">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="728be-158">Boolean</span></span>|<span data-ttu-id="728be-159">Anforderung zur Eingabe eines Werts im Parameterfeld.</span><span class="sxs-lookup"><span data-stu-id="728be-159">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="728be-160">Der Standardwert ist false.</span><span class="sxs-lookup"><span data-stu-id="728be-160">The default value is false.</span></span>|
|<span data-ttu-id="728be-161">minValue</span><span class="sxs-lookup"><span data-stu-id="728be-161">minValue</span></span>|<span data-ttu-id="728be-162">Int64</span><span class="sxs-lookup"><span data-stu-id="728be-162">Int64</span></span>|<span data-ttu-id="728be-163">Eine ganze Zahl ohne Vorzeichen, die den minimal zulässigen Wert angibt.</span><span class="sxs-lookup"><span data-stu-id="728be-163">An unsigned integer that specifies the minimum allowed value.</span></span> <span data-ttu-id="728be-164">Der Standardwert ist 0.</span><span class="sxs-lookup"><span data-stu-id="728be-164">The default value is 0.</span></span>|
|<span data-ttu-id="728be-165">maxValue</span><span class="sxs-lookup"><span data-stu-id="728be-165">maxValue</span></span>|<span data-ttu-id="728be-166">Int64</span><span class="sxs-lookup"><span data-stu-id="728be-166">Int64</span></span>|<span data-ttu-id="728be-167">Eine ganze Zahl ohne Vorzeichen, die den maximal zulässigen Wert angibt.</span><span class="sxs-lookup"><span data-stu-id="728be-167">An unsigned integer that specifies the maximum allowed value.</span></span> <span data-ttu-id="728be-168">Der Standardwert ist 9999.</span><span class="sxs-lookup"><span data-stu-id="728be-168">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="728be-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="728be-169">Response</span></span>
<span data-ttu-id="728be-170">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="728be-170">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="728be-171">Beispiel</span><span class="sxs-lookup"><span data-stu-id="728be-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="728be-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="728be-172">Request</span></span>
<span data-ttu-id="728be-173">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="728be-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="728be-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="728be-174">Response</span></span>
<span data-ttu-id="728be-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="728be-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




