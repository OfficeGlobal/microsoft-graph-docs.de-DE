---
title: GroupPolicyPresentationCheckBox aktualisieren
description: Aktualisieren Sie die Eigenschaften eines GroupPolicyPresentationCheckBox-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4150e662109b9dc9d0ebee6a66be12ad1c2473bc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430119"
---
# <a name="update-grouppolicypresentationcheckbox"></a><span data-ttu-id="d6d5b-103">GroupPolicyPresentationCheckBox aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d6d5b-103">Update groupPolicyPresentationCheckBox</span></span>

> <span data-ttu-id="d6d5b-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="d6d5b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d6d5b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d6d5b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6d5b-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d6d5b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6d5b-107">Aktualisieren Sie die Eigenschaften eines [GroupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d6d5b-107">Update the properties of a [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6d5b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d6d5b-108">Prerequisites</span></span>
<span data-ttu-id="d6d5b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d6d5b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d6d5b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d6d5b-111">Permission type</span></span>|<span data-ttu-id="d6d5b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d6d5b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6d5b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d6d5b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d6d5b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6d5b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d6d5b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d6d5b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6d5b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d6d5b-116">Not supported.</span></span>|
|<span data-ttu-id="d6d5b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d6d5b-117">Application</span></span>|<span data-ttu-id="d6d5b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d6d5b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6d5b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d6d5b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="d6d5b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d6d5b-120">Request headers</span></span>
|<span data-ttu-id="d6d5b-121">Header</span><span class="sxs-lookup"><span data-stu-id="d6d5b-121">Header</span></span>|<span data-ttu-id="d6d5b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d6d5b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6d5b-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d6d5b-123">Authorization</span></span>|<span data-ttu-id="d6d5b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d6d5b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6d5b-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d6d5b-125">Accept</span></span>|<span data-ttu-id="d6d5b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6d5b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6d5b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d6d5b-127">Request body</span></span>
<span data-ttu-id="d6d5b-128">Geben Sie im Textkörper Anforderung für das Objekt [GroupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="d6d5b-128">In the request body, supply a JSON representation for the [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

<span data-ttu-id="d6d5b-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [GroupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="d6d5b-129">The following table shows the properties that are required when you create the [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md).</span></span>

|<span data-ttu-id="d6d5b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d6d5b-130">Property</span></span>|<span data-ttu-id="d6d5b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="d6d5b-131">Type</span></span>|<span data-ttu-id="d6d5b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d6d5b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6d5b-133">label</span><span class="sxs-lookup"><span data-stu-id="d6d5b-133">label</span></span>|<span data-ttu-id="d6d5b-134">String</span><span class="sxs-lookup"><span data-stu-id="d6d5b-134">String</span></span>|<span data-ttu-id="d6d5b-135">Lokalisierte Beschriftung für jede Entität Präsentation.</span><span class="sxs-lookup"><span data-stu-id="d6d5b-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="d6d5b-136">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="d6d5b-136">The default value is empty.</span></span> <span data-ttu-id="d6d5b-137">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="d6d5b-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="d6d5b-138">id</span><span class="sxs-lookup"><span data-stu-id="d6d5b-138">id</span></span>|<span data-ttu-id="d6d5b-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d6d5b-139">String</span></span>|<span data-ttu-id="d6d5b-140">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d6d5b-140">Key of the entity.</span></span> <span data-ttu-id="d6d5b-141">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="d6d5b-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="d6d5b-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6d5b-142">lastModifiedDateTime</span></span>|<span data-ttu-id="d6d5b-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6d5b-143">DateTimeOffset</span></span>|<span data-ttu-id="d6d5b-144">Datum und Uhrzeit der letzten Änderung die Entität.</span><span class="sxs-lookup"><span data-stu-id="d6d5b-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="d6d5b-145">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="d6d5b-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="d6d5b-146">defaultChecked</span><span class="sxs-lookup"><span data-stu-id="d6d5b-146">defaultChecked</span></span>|<span data-ttu-id="d6d5b-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="d6d5b-147">Boolean</span></span>|<span data-ttu-id="d6d5b-148">Der Standardwert für das entsprechende Kontrollkästchen.</span><span class="sxs-lookup"><span data-stu-id="d6d5b-148">Default value for the check box.</span></span> <span data-ttu-id="d6d5b-149">Der Standardwert ist false.</span><span class="sxs-lookup"><span data-stu-id="d6d5b-149">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="d6d5b-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="d6d5b-150">Response</span></span>
<span data-ttu-id="d6d5b-151">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [GroupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d6d5b-151">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6d5b-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d6d5b-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6d5b-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d6d5b-153">Request</span></span>
<span data-ttu-id="d6d5b-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d6d5b-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
  "label": "Label value",
  "defaultChecked": true
}
```

### <a name="response"></a><span data-ttu-id="d6d5b-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="d6d5b-155">Response</span></span>
<span data-ttu-id="d6d5b-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d6d5b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 240

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
  "label": "Label value",
  "id": "7748190f-190f-7748-0f19-48770f194877",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultChecked": true
}
```




