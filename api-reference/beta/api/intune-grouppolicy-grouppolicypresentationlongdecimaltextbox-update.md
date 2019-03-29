---
title: GroupPolicyPresentationLongDecimalTextBox aktualisieren
description: Aktualisieren der Eigenschaften eines groupPolicyPresentationLongDecimalTextBox-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 02bcc2147bccee59594627e5c2ce3eaac9c64c5e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978556"
---
# <a name="update-grouppolicypresentationlongdecimaltextbox"></a><span data-ttu-id="2a038-103">GroupPolicyPresentationLongDecimalTextBox aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2a038-103">Update groupPolicyPresentationLongDecimalTextBox</span></span>

> <span data-ttu-id="2a038-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2a038-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a038-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2a038-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a038-106">Aktualisieren der Eigenschaften eines [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2a038-106">Update the properties of a [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a038-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2a038-107">Prerequisites</span></span>
<span data-ttu-id="2a038-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a038-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a038-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2a038-110">Permission type</span></span>|<span data-ttu-id="2a038-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2a038-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a038-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2a038-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2a038-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a038-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2a038-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2a038-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a038-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a038-115">Not supported.</span></span>|
|<span data-ttu-id="2a038-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2a038-116">Application</span></span>|<span data-ttu-id="2a038-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a038-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a038-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a038-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="2a038-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2a038-119">Request headers</span></span>
|<span data-ttu-id="2a038-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2a038-120">Header</span></span>|<span data-ttu-id="2a038-121">Wert</span><span class="sxs-lookup"><span data-stu-id="2a038-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a038-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a038-122">Authorization</span></span>|<span data-ttu-id="2a038-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2a038-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a038-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2a038-124">Accept</span></span>|<span data-ttu-id="2a038-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2a038-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a038-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2a038-126">Request body</span></span>
<span data-ttu-id="2a038-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="2a038-127">In the request body, supply a JSON representation for the [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object.</span></span>

<span data-ttu-id="2a038-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="2a038-128">The following table shows the properties that are required when you create the [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md).</span></span>

|<span data-ttu-id="2a038-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2a038-129">Property</span></span>|<span data-ttu-id="2a038-130">Typ</span><span class="sxs-lookup"><span data-stu-id="2a038-130">Type</span></span>|<span data-ttu-id="2a038-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a038-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a038-132">label</span><span class="sxs-lookup"><span data-stu-id="2a038-132">label</span></span>|<span data-ttu-id="2a038-133">String</span><span class="sxs-lookup"><span data-stu-id="2a038-133">String</span></span>|<span data-ttu-id="2a038-134">Lokalisierte Textbezeichnung für eine beliebige Präsentations Entität.</span><span class="sxs-lookup"><span data-stu-id="2a038-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="2a038-135">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="2a038-135">The default value is empty.</span></span> <span data-ttu-id="2a038-136">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="2a038-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="2a038-137">id</span><span class="sxs-lookup"><span data-stu-id="2a038-137">id</span></span>|<span data-ttu-id="2a038-138">String</span><span class="sxs-lookup"><span data-stu-id="2a038-138">String</span></span>|<span data-ttu-id="2a038-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2a038-139">Key of the entity.</span></span> <span data-ttu-id="2a038-140">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="2a038-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="2a038-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2a038-141">lastModifiedDateTime</span></span>|<span data-ttu-id="2a038-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a038-142">DateTimeOffset</span></span>|<span data-ttu-id="2a038-143">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="2a038-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="2a038-144">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="2a038-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="2a038-145">defaultValue</span><span class="sxs-lookup"><span data-stu-id="2a038-145">defaultValue</span></span>|<span data-ttu-id="2a038-146">Int64</span><span class="sxs-lookup"><span data-stu-id="2a038-146">Int64</span></span>|<span data-ttu-id="2a038-147">Eine ganze Zahl ohne Vorzeichen, die den Anfangswert für das Dezimal Textfeld angibt.</span><span class="sxs-lookup"><span data-stu-id="2a038-147">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="2a038-148">Der Standardwert ist 1.</span><span class="sxs-lookup"><span data-stu-id="2a038-148">The default value is 1.</span></span>|
|<span data-ttu-id="2a038-149">Spin</span><span class="sxs-lookup"><span data-stu-id="2a038-149">spin</span></span>|<span data-ttu-id="2a038-150">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2a038-150">Boolean</span></span>|<span data-ttu-id="2a038-151">Wenn true, erstellen Sie ein Drehfeld-Steuerelement; Erstellen Sie andernfalls ein Textfeld für die numerische Eingabe.</span><span class="sxs-lookup"><span data-stu-id="2a038-151">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="2a038-152">Der Standardwert ist "True".</span><span class="sxs-lookup"><span data-stu-id="2a038-152">The default value is true.</span></span>|
|<span data-ttu-id="2a038-153">spinStep</span><span class="sxs-lookup"><span data-stu-id="2a038-153">spinStep</span></span>|<span data-ttu-id="2a038-154">Int64</span><span class="sxs-lookup"><span data-stu-id="2a038-154">Int64</span></span>|<span data-ttu-id="2a038-155">Eine ganze Zahl ohne Vorzeichen, die die Schrittweite der Änderung für das Drehfeld-Steuerelement angibt.</span><span class="sxs-lookup"><span data-stu-id="2a038-155">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="2a038-156">Der Standardwert ist 1.</span><span class="sxs-lookup"><span data-stu-id="2a038-156">The default value is 1.</span></span>|
|<span data-ttu-id="2a038-157">erforderlich</span><span class="sxs-lookup"><span data-stu-id="2a038-157">required</span></span>|<span data-ttu-id="2a038-158">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2a038-158">Boolean</span></span>|<span data-ttu-id="2a038-159">Anforderung zur Eingabe eines Werts im Parameterfeld.</span><span class="sxs-lookup"><span data-stu-id="2a038-159">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="2a038-160">Der Standardwert ist false.</span><span class="sxs-lookup"><span data-stu-id="2a038-160">The default value is false.</span></span>|
|<span data-ttu-id="2a038-161">minValue</span><span class="sxs-lookup"><span data-stu-id="2a038-161">minValue</span></span>|<span data-ttu-id="2a038-162">Int64</span><span class="sxs-lookup"><span data-stu-id="2a038-162">Int64</span></span>|<span data-ttu-id="2a038-163">Eine unsigned long, die den minimal zulässigen Wert angibt.</span><span class="sxs-lookup"><span data-stu-id="2a038-163">An unsigned long that specifies the minimum allowed value.</span></span> <span data-ttu-id="2a038-164">Der Standardwert ist 0.</span><span class="sxs-lookup"><span data-stu-id="2a038-164">The default value is 0.</span></span>|
|<span data-ttu-id="2a038-165">maxValue</span><span class="sxs-lookup"><span data-stu-id="2a038-165">maxValue</span></span>|<span data-ttu-id="2a038-166">Int64</span><span class="sxs-lookup"><span data-stu-id="2a038-166">Int64</span></span>|<span data-ttu-id="2a038-167">Eine unsigned long, die den maximal zulässigen Wert angibt.</span><span class="sxs-lookup"><span data-stu-id="2a038-167">An unsigned long that specifies the maximum allowed value.</span></span> <span data-ttu-id="2a038-168">Der Standardwert ist 9999.</span><span class="sxs-lookup"><span data-stu-id="2a038-168">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="2a038-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a038-169">Response</span></span>
<span data-ttu-id="2a038-170">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2a038-170">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a038-171">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2a038-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a038-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a038-172">Request</span></span>
<span data-ttu-id="2a038-173">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2a038-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 225

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationLongDecimalTextBox",
  "label": "Label value",
  "defaultValue": 12,
  "spin": true,
  "spinStep": 8,
  "required": true,
  "minValue": 8,
  "maxValue": 8
}
```

### <a name="response"></a><span data-ttu-id="2a038-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a038-174">Response</span></span>
<span data-ttu-id="2a038-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2a038-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 338

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationLongDecimalTextBox",
  "label": "Label value",
  "id": "754d8495-8495-754d-9584-4d7595844d75",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": 12,
  "spin": true,
  "spinStep": 8,
  "required": true,
  "minValue": 8,
  "maxValue": 8
}
```




