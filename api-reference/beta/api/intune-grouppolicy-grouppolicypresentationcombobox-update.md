---
title: GroupPolicyPresentationComboBox aktualisieren
description: Aktualisieren Sie die Eigenschaften eines GroupPolicyPresentationComboBox-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6302d52e91e5fe1cf8a21e525d0eccef608b3b24
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430141"
---
# <a name="update-grouppolicypresentationcombobox"></a><span data-ttu-id="c1beb-103">GroupPolicyPresentationComboBox aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c1beb-103">Update groupPolicyPresentationComboBox</span></span>

> <span data-ttu-id="c1beb-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="c1beb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c1beb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c1beb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1beb-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c1beb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1beb-107">Aktualisieren Sie die Eigenschaften eines [GroupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c1beb-107">Update the properties of a [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1beb-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c1beb-108">Prerequisites</span></span>
<span data-ttu-id="c1beb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c1beb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c1beb-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c1beb-111">Permission type</span></span>|<span data-ttu-id="c1beb-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c1beb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1beb-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c1beb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c1beb-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1beb-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c1beb-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c1beb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1beb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1beb-116">Not supported.</span></span>|
|<span data-ttu-id="c1beb-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c1beb-117">Application</span></span>|<span data-ttu-id="c1beb-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1beb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1beb-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1beb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="c1beb-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c1beb-120">Request headers</span></span>
|<span data-ttu-id="c1beb-121">Header</span><span class="sxs-lookup"><span data-stu-id="c1beb-121">Header</span></span>|<span data-ttu-id="c1beb-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c1beb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1beb-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c1beb-123">Authorization</span></span>|<span data-ttu-id="c1beb-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c1beb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1beb-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c1beb-125">Accept</span></span>|<span data-ttu-id="c1beb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c1beb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1beb-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c1beb-127">Request body</span></span>
<span data-ttu-id="c1beb-128">Geben Sie im Textkörper Anforderung für das Objekt [GroupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="c1beb-128">In the request body, supply a JSON representation for the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

<span data-ttu-id="c1beb-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [GroupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="c1beb-129">The following table shows the properties that are required when you create the [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md).</span></span>

|<span data-ttu-id="c1beb-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c1beb-130">Property</span></span>|<span data-ttu-id="c1beb-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c1beb-131">Type</span></span>|<span data-ttu-id="c1beb-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c1beb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1beb-133">label</span><span class="sxs-lookup"><span data-stu-id="c1beb-133">label</span></span>|<span data-ttu-id="c1beb-134">String</span><span class="sxs-lookup"><span data-stu-id="c1beb-134">String</span></span>|<span data-ttu-id="c1beb-135">Lokalisierte Beschriftung für jede Entität Präsentation.</span><span class="sxs-lookup"><span data-stu-id="c1beb-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="c1beb-136">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="c1beb-136">The default value is empty.</span></span> <span data-ttu-id="c1beb-137">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="c1beb-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="c1beb-138">id</span><span class="sxs-lookup"><span data-stu-id="c1beb-138">id</span></span>|<span data-ttu-id="c1beb-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1beb-139">String</span></span>|<span data-ttu-id="c1beb-140">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c1beb-140">Key of the entity.</span></span> <span data-ttu-id="c1beb-141">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="c1beb-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="c1beb-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1beb-142">lastModifiedDateTime</span></span>|<span data-ttu-id="c1beb-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1beb-143">DateTimeOffset</span></span>|<span data-ttu-id="c1beb-144">Datum und Uhrzeit der letzten Änderung die Entität.</span><span class="sxs-lookup"><span data-stu-id="c1beb-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="c1beb-145">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="c1beb-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="c1beb-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="c1beb-146">defaultValue</span></span>|<span data-ttu-id="c1beb-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1beb-147">String</span></span>|<span data-ttu-id="c1beb-148">Lokalisierte Standardzeichenfolge im Kombinationsfeld angezeigt.</span><span class="sxs-lookup"><span data-stu-id="c1beb-148">Localized default string displayed in the combo box.</span></span> <span data-ttu-id="c1beb-149">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="c1beb-149">The default value is empty.</span></span>|
|<span data-ttu-id="c1beb-150">Vorschläge</span><span class="sxs-lookup"><span data-stu-id="c1beb-150">suggestions</span></span>|<span data-ttu-id="c1beb-151">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="c1beb-151">String collection</span></span>|<span data-ttu-id="c1beb-152">Es werden lokalisierte Zeichenfolgen, die in der Dropdown Liste des Kombinationsfelds aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="c1beb-152">Localized strings listed in the drop-down list of the combo box.</span></span> <span data-ttu-id="c1beb-153">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="c1beb-153">The default value is empty.</span></span>|
|<span data-ttu-id="c1beb-154">erforderlich</span><span class="sxs-lookup"><span data-stu-id="c1beb-154">required</span></span>|<span data-ttu-id="c1beb-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1beb-155">Boolean</span></span>|<span data-ttu-id="c1beb-156">Gibt an, ob ein Wert für den Parameter angegeben werden muss.</span><span class="sxs-lookup"><span data-stu-id="c1beb-156">Specifies whether a value must be specified for the parameter.</span></span> <span data-ttu-id="c1beb-157">Der Standardwert ist false.</span><span class="sxs-lookup"><span data-stu-id="c1beb-157">The default value is false.</span></span>|
|<span data-ttu-id="c1beb-158">maxLength</span><span class="sxs-lookup"><span data-stu-id="c1beb-158">maxLength</span></span>|<span data-ttu-id="c1beb-159">Int64</span><span class="sxs-lookup"><span data-stu-id="c1beb-159">Int64</span></span>|<span data-ttu-id="c1beb-160">Eine ganze Zahl ohne Vorzeichen, die die maximale Anzahl von Textzeichen für den Parameter angibt.</span><span class="sxs-lookup"><span data-stu-id="c1beb-160">An unsigned integer that specifies the maximum number of text characters for the parameter.</span></span> <span data-ttu-id="c1beb-161">Der Standardwert ist 1023.</span><span class="sxs-lookup"><span data-stu-id="c1beb-161">The default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="c1beb-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1beb-162">Response</span></span>
<span data-ttu-id="c1beb-163">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [GroupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="c1beb-163">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1beb-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c1beb-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1beb-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1beb-165">Request</span></span>
<span data-ttu-id="c1beb-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c1beb-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 233

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationComboBox",
  "label": "Label value",
  "defaultValue": "Default Value value",
  "suggestions": [
    "Suggestions value"
  ],
  "required": true,
  "maxLength": 9
}
```

### <a name="response"></a><span data-ttu-id="c1beb-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1beb-167">Response</span></span>
<span data-ttu-id="c1beb-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c1beb-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationComboBox",
  "label": "Label value",
  "id": "44332a1d-2a1d-4433-1d2a-33441d2a3344",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": "Default Value value",
  "suggestions": [
    "Suggestions value"
  ],
  "required": true,
  "maxLength": 9
}
```




