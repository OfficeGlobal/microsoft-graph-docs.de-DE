---
title: GroupPolicyPresentationText erstellen
description: Erstellen eines neuen groupPolicyPresentationText-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9e15635842499472d831af066cf6b25b2c830e9a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172030"
---
# <a name="create-grouppolicypresentationtext"></a><span data-ttu-id="77548-103">GroupPolicyPresentationText erstellen</span><span class="sxs-lookup"><span data-stu-id="77548-103">Create groupPolicyPresentationText</span></span>

> <span data-ttu-id="77548-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="77548-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77548-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="77548-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77548-106">Erstellen eines neuen [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="77548-106">Create a new [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77548-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="77548-107">Prerequisites</span></span>
<span data-ttu-id="77548-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="77548-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="77548-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="77548-110">Permission type</span></span>|<span data-ttu-id="77548-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="77548-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77548-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="77548-112">Delegated (work or school account)</span></span>|<span data-ttu-id="77548-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77548-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="77548-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="77548-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77548-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77548-115">Not supported.</span></span>|
|<span data-ttu-id="77548-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="77548-116">Application</span></span>|<span data-ttu-id="77548-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77548-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77548-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="77548-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="77548-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="77548-119">Request headers</span></span>
|<span data-ttu-id="77548-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="77548-120">Header</span></span>|<span data-ttu-id="77548-121">Wert</span><span class="sxs-lookup"><span data-stu-id="77548-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77548-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="77548-122">Authorization</span></span>|<span data-ttu-id="77548-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="77548-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77548-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="77548-124">Accept</span></span>|<span data-ttu-id="77548-125">application/json</span><span class="sxs-lookup"><span data-stu-id="77548-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77548-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="77548-126">Request body</span></span>
<span data-ttu-id="77548-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das groupPolicyPresentationText-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="77548-127">In the request body, supply a JSON representation for the groupPolicyPresentationText object.</span></span>

<span data-ttu-id="77548-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der groupPolicyPresentationText erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="77548-128">The following table shows the properties that are required when you create the groupPolicyPresentationText.</span></span>

|<span data-ttu-id="77548-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="77548-129">Property</span></span>|<span data-ttu-id="77548-130">Typ</span><span class="sxs-lookup"><span data-stu-id="77548-130">Type</span></span>|<span data-ttu-id="77548-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77548-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77548-132">label</span><span class="sxs-lookup"><span data-stu-id="77548-132">label</span></span>|<span data-ttu-id="77548-133">String</span><span class="sxs-lookup"><span data-stu-id="77548-133">String</span></span>|<span data-ttu-id="77548-134">Lokalisierte Textbezeichnung für eine beliebige Präsentations Entität.</span><span class="sxs-lookup"><span data-stu-id="77548-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="77548-135">Der Standardwert ist Empty.</span><span class="sxs-lookup"><span data-stu-id="77548-135">The default value is empty.</span></span> <span data-ttu-id="77548-136">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="77548-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="77548-137">id</span><span class="sxs-lookup"><span data-stu-id="77548-137">id</span></span>|<span data-ttu-id="77548-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="77548-138">String</span></span>|<span data-ttu-id="77548-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="77548-139">Key of the entity.</span></span> <span data-ttu-id="77548-140">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="77548-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="77548-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="77548-141">lastModifiedDateTime</span></span>|<span data-ttu-id="77548-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77548-142">DateTimeOffset</span></span>|<span data-ttu-id="77548-143">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="77548-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="77548-144">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="77548-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|



## <a name="response"></a><span data-ttu-id="77548-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="77548-145">Response</span></span>
<span data-ttu-id="77548-146">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="77548-146">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77548-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="77548-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="77548-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="77548-148">Request</span></span>
<span data-ttu-id="77548-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="77548-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="77548-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="77548-150">Response</span></span>
<span data-ttu-id="77548-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="77548-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 209

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "Label value",
  "id": "bc77d545-d545-bc77-45d5-77bc45d577bc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




