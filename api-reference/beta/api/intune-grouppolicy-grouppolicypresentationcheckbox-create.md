---
title: Erstellen von groupPolicyPresentationCheckBox
description: Erstellen eines neuen GroupPolicyPresentationCheckBox-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dc0d5ff04aedfbbf0e9bac3967f5f502a13e5e57
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430031"
---
# <a name="create-grouppolicypresentationcheckbox"></a><span data-ttu-id="7fb20-103">Erstellen von groupPolicyPresentationCheckBox</span><span class="sxs-lookup"><span data-stu-id="7fb20-103">Create groupPolicyPresentationCheckBox</span></span>

> <span data-ttu-id="7fb20-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="7fb20-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7fb20-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7fb20-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7fb20-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7fb20-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7fb20-107">Erstellen eines neuen [GroupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="7fb20-107">Create a new [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7fb20-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7fb20-108">Prerequisites</span></span>
<span data-ttu-id="7fb20-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7fb20-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7fb20-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7fb20-111">Permission type</span></span>|<span data-ttu-id="7fb20-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7fb20-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fb20-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7fb20-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7fb20-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fb20-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7fb20-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7fb20-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7fb20-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7fb20-116">Not supported.</span></span>|
|<span data-ttu-id="7fb20-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7fb20-117">Application</span></span>|<span data-ttu-id="7fb20-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7fb20-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fb20-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7fb20-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="7fb20-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7fb20-120">Request headers</span></span>
|<span data-ttu-id="7fb20-121">Header</span><span class="sxs-lookup"><span data-stu-id="7fb20-121">Header</span></span>|<span data-ttu-id="7fb20-122">Wert</span><span class="sxs-lookup"><span data-stu-id="7fb20-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7fb20-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="7fb20-123">Authorization</span></span>|<span data-ttu-id="7fb20-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7fb20-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7fb20-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7fb20-125">Accept</span></span>|<span data-ttu-id="7fb20-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7fb20-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fb20-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7fb20-127">Request body</span></span>
<span data-ttu-id="7fb20-128">Geben Sie im Textkörper Anforderung für das Objekt GroupPolicyPresentationCheckBox eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="7fb20-128">In the request body, supply a JSON representation for the groupPolicyPresentationCheckBox object.</span></span>

<span data-ttu-id="7fb20-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die GroupPolicyPresentationCheckBox erstellen.</span><span class="sxs-lookup"><span data-stu-id="7fb20-129">The following table shows the properties that are required when you create the groupPolicyPresentationCheckBox.</span></span>

|<span data-ttu-id="7fb20-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7fb20-130">Property</span></span>|<span data-ttu-id="7fb20-131">Typ</span><span class="sxs-lookup"><span data-stu-id="7fb20-131">Type</span></span>|<span data-ttu-id="7fb20-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7fb20-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fb20-133">label</span><span class="sxs-lookup"><span data-stu-id="7fb20-133">label</span></span>|<span data-ttu-id="7fb20-134">String</span><span class="sxs-lookup"><span data-stu-id="7fb20-134">String</span></span>|<span data-ttu-id="7fb20-135">Lokalisierte Beschriftung für jede Entität Präsentation.</span><span class="sxs-lookup"><span data-stu-id="7fb20-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="7fb20-136">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="7fb20-136">The default value is empty.</span></span> <span data-ttu-id="7fb20-137">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="7fb20-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="7fb20-138">id</span><span class="sxs-lookup"><span data-stu-id="7fb20-138">id</span></span>|<span data-ttu-id="7fb20-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7fb20-139">String</span></span>|<span data-ttu-id="7fb20-140">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7fb20-140">Key of the entity.</span></span> <span data-ttu-id="7fb20-141">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="7fb20-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="7fb20-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7fb20-142">lastModifiedDateTime</span></span>|<span data-ttu-id="7fb20-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7fb20-143">DateTimeOffset</span></span>|<span data-ttu-id="7fb20-144">Datum und Uhrzeit der letzten Änderung die Entität.</span><span class="sxs-lookup"><span data-stu-id="7fb20-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="7fb20-145">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="7fb20-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="7fb20-146">defaultChecked</span><span class="sxs-lookup"><span data-stu-id="7fb20-146">defaultChecked</span></span>|<span data-ttu-id="7fb20-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="7fb20-147">Boolean</span></span>|<span data-ttu-id="7fb20-148">Der Standardwert für das entsprechende Kontrollkästchen.</span><span class="sxs-lookup"><span data-stu-id="7fb20-148">Default value for the check box.</span></span> <span data-ttu-id="7fb20-149">Der Standardwert ist false.</span><span class="sxs-lookup"><span data-stu-id="7fb20-149">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="7fb20-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="7fb20-150">Response</span></span>
<span data-ttu-id="7fb20-151">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [GroupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="7fb20-151">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fb20-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7fb20-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="7fb20-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7fb20-153">Request</span></span>
<span data-ttu-id="7fb20-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7fb20-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
  "label": "Label value",
  "defaultChecked": true
}
```

### <a name="response"></a><span data-ttu-id="7fb20-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="7fb20-155">Response</span></span>
<span data-ttu-id="7fb20-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7fb20-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




