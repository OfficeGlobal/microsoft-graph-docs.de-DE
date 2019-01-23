---
title: Erstellen von groupPolicyPresentationLongDecimalTextBox
description: Erstellen eines neuen GroupPolicyPresentationLongDecimalTextBox-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d1fd47d422358dd0cd4a23ff35137654787498bf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430020"
---
# <a name="create-grouppolicypresentationlongdecimaltextbox"></a><span data-ttu-id="2f18b-103">Erstellen von groupPolicyPresentationLongDecimalTextBox</span><span class="sxs-lookup"><span data-stu-id="2f18b-103">Create groupPolicyPresentationLongDecimalTextBox</span></span>

> <span data-ttu-id="2f18b-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="2f18b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2f18b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2f18b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2f18b-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2f18b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f18b-107">Erstellen eines neuen [GroupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2f18b-107">Create a new [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f18b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2f18b-108">Prerequisites</span></span>
<span data-ttu-id="2f18b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2f18b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2f18b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2f18b-111">Permission type</span></span>|<span data-ttu-id="2f18b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2f18b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f18b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2f18b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f18b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f18b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2f18b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2f18b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f18b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f18b-116">Not supported.</span></span>|
|<span data-ttu-id="2f18b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2f18b-117">Application</span></span>|<span data-ttu-id="2f18b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f18b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f18b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f18b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="2f18b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2f18b-120">Request headers</span></span>
|<span data-ttu-id="2f18b-121">Header</span><span class="sxs-lookup"><span data-stu-id="2f18b-121">Header</span></span>|<span data-ttu-id="2f18b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="2f18b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f18b-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="2f18b-123">Authorization</span></span>|<span data-ttu-id="2f18b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2f18b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f18b-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2f18b-125">Accept</span></span>|<span data-ttu-id="2f18b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f18b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f18b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2f18b-127">Request body</span></span>
<span data-ttu-id="2f18b-128">Geben Sie im Textkörper Anforderung für das Objekt GroupPolicyPresentationLongDecimalTextBox eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="2f18b-128">In the request body, supply a JSON representation for the groupPolicyPresentationLongDecimalTextBox object.</span></span>

<span data-ttu-id="2f18b-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die GroupPolicyPresentationLongDecimalTextBox erstellen.</span><span class="sxs-lookup"><span data-stu-id="2f18b-129">The following table shows the properties that are required when you create the groupPolicyPresentationLongDecimalTextBox.</span></span>

|<span data-ttu-id="2f18b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2f18b-130">Property</span></span>|<span data-ttu-id="2f18b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="2f18b-131">Type</span></span>|<span data-ttu-id="2f18b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2f18b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f18b-133">label</span><span class="sxs-lookup"><span data-stu-id="2f18b-133">label</span></span>|<span data-ttu-id="2f18b-134">String</span><span class="sxs-lookup"><span data-stu-id="2f18b-134">String</span></span>|<span data-ttu-id="2f18b-135">Lokalisierte Beschriftung für jede Entität Präsentation.</span><span class="sxs-lookup"><span data-stu-id="2f18b-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="2f18b-136">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="2f18b-136">The default value is empty.</span></span> <span data-ttu-id="2f18b-137">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="2f18b-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="2f18b-138">id</span><span class="sxs-lookup"><span data-stu-id="2f18b-138">id</span></span>|<span data-ttu-id="2f18b-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2f18b-139">String</span></span>|<span data-ttu-id="2f18b-140">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2f18b-140">Key of the entity.</span></span> <span data-ttu-id="2f18b-141">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="2f18b-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="2f18b-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f18b-142">lastModifiedDateTime</span></span>|<span data-ttu-id="2f18b-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f18b-143">DateTimeOffset</span></span>|<span data-ttu-id="2f18b-144">Datum und Uhrzeit der letzten Änderung die Entität.</span><span class="sxs-lookup"><span data-stu-id="2f18b-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="2f18b-145">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="2f18b-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="2f18b-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="2f18b-146">defaultValue</span></span>|<span data-ttu-id="2f18b-147">Int64</span><span class="sxs-lookup"><span data-stu-id="2f18b-147">Int64</span></span>|<span data-ttu-id="2f18b-148">Eine ganze Zahl ohne Vorzeichen, die den Anfangswert des Textfelds decimal angibt.</span><span class="sxs-lookup"><span data-stu-id="2f18b-148">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="2f18b-149">Der Standardwert ist 1.</span><span class="sxs-lookup"><span data-stu-id="2f18b-149">The default value is 1.</span></span>|
|<span data-ttu-id="2f18b-150">Drehfeld</span><span class="sxs-lookup"><span data-stu-id="2f18b-150">spin</span></span>|<span data-ttu-id="2f18b-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f18b-151">Boolean</span></span>|<span data-ttu-id="2f18b-152">Wenn true, erstellen Sie ein Drehfeld-Steuerelement. Erstellen Sie andernfalls ein Textfeld für numerische Eingabe.</span><span class="sxs-lookup"><span data-stu-id="2f18b-152">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="2f18b-153">Der Standardwert ist true.</span><span class="sxs-lookup"><span data-stu-id="2f18b-153">The default value is true.</span></span>|
|<span data-ttu-id="2f18b-154">spinStep</span><span class="sxs-lookup"><span data-stu-id="2f18b-154">spinStep</span></span>|<span data-ttu-id="2f18b-155">Int64</span><span class="sxs-lookup"><span data-stu-id="2f18b-155">Int64</span></span>|<span data-ttu-id="2f18b-156">Eine ganze Zahl ohne Vorzeichen, die die Schrittweite der Änderung für das Drehfeld-Steuerelement angibt.</span><span class="sxs-lookup"><span data-stu-id="2f18b-156">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="2f18b-157">Der Standardwert ist 1.</span><span class="sxs-lookup"><span data-stu-id="2f18b-157">The default value is 1.</span></span>|
|<span data-ttu-id="2f18b-158">erforderlich</span><span class="sxs-lookup"><span data-stu-id="2f18b-158">required</span></span>|<span data-ttu-id="2f18b-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f18b-159">Boolean</span></span>|<span data-ttu-id="2f18b-160">Anforderung im Parameter einen Wert eingeben.</span><span class="sxs-lookup"><span data-stu-id="2f18b-160">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="2f18b-161">Der Standardwert ist false.</span><span class="sxs-lookup"><span data-stu-id="2f18b-161">The default value is false.</span></span>|
|<span data-ttu-id="2f18b-162">minValue</span><span class="sxs-lookup"><span data-stu-id="2f18b-162">minValue</span></span>|<span data-ttu-id="2f18b-163">Int64</span><span class="sxs-lookup"><span data-stu-id="2f18b-163">Int64</span></span>|<span data-ttu-id="2f18b-164">Eine nicht signierte Long-Wert, der angibt, der den zulässigen Mindestwert.</span><span class="sxs-lookup"><span data-stu-id="2f18b-164">An unsigned long that specifies the minimum allowed value.</span></span> <span data-ttu-id="2f18b-165">Der Standardwert ist 0.</span><span class="sxs-lookup"><span data-stu-id="2f18b-165">The default value is 0.</span></span>|
|<span data-ttu-id="2f18b-166">maxValue</span><span class="sxs-lookup"><span data-stu-id="2f18b-166">maxValue</span></span>|<span data-ttu-id="2f18b-167">Int64</span><span class="sxs-lookup"><span data-stu-id="2f18b-167">Int64</span></span>|<span data-ttu-id="2f18b-168">Eine nicht signierte Long-Wert, der den maximal zulässigen Wert angibt.</span><span class="sxs-lookup"><span data-stu-id="2f18b-168">An unsigned long that specifies the maximum allowed value.</span></span> <span data-ttu-id="2f18b-169">Der Standardwert ist 9999.</span><span class="sxs-lookup"><span data-stu-id="2f18b-169">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="2f18b-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f18b-170">Response</span></span>
<span data-ttu-id="2f18b-171">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [GroupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="2f18b-171">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f18b-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f18b-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f18b-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f18b-173">Request</span></span>
<span data-ttu-id="2f18b-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2f18b-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
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

### <a name="response"></a><span data-ttu-id="2f18b-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f18b-175">Response</span></span>
<span data-ttu-id="2f18b-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2f18b-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




