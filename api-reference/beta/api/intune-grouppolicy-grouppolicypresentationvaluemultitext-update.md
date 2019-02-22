---
title: GroupPolicyPresentationValueMultiText aktualisieren
description: Aktualisieren der Eigenschaften eines groupPolicyPresentationValueMultiText-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 28afb8f58808f8a528f933fbe10d9cefaefd1378
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152717"
---
# <a name="update-grouppolicypresentationvaluemultitext"></a><span data-ttu-id="1e513-103">GroupPolicyPresentationValueMultiText aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1e513-103">Update groupPolicyPresentationValueMultiText</span></span>

> <span data-ttu-id="1e513-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1e513-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e513-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1e513-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e513-106">Aktualisieren der Eigenschaften eines [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="1e513-106">Update the properties of a [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e513-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1e513-107">Prerequisites</span></span>
<span data-ttu-id="1e513-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1e513-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1e513-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1e513-110">Permission type</span></span>|<span data-ttu-id="1e513-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1e513-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e513-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1e513-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1e513-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e513-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1e513-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1e513-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e513-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1e513-115">Not supported.</span></span>|
|<span data-ttu-id="1e513-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1e513-116">Application</span></span>|<span data-ttu-id="1e513-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1e513-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e513-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1e513-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="1e513-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1e513-119">Request headers</span></span>
|<span data-ttu-id="1e513-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1e513-120">Header</span></span>|<span data-ttu-id="1e513-121">Wert</span><span class="sxs-lookup"><span data-stu-id="1e513-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e513-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e513-122">Authorization</span></span>|<span data-ttu-id="1e513-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1e513-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e513-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1e513-124">Accept</span></span>|<span data-ttu-id="1e513-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1e513-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e513-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1e513-126">Request body</span></span>
<span data-ttu-id="1e513-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="1e513-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object.</span></span>

<span data-ttu-id="1e513-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="1e513-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md).</span></span>

|<span data-ttu-id="1e513-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1e513-129">Property</span></span>|<span data-ttu-id="1e513-130">Typ</span><span class="sxs-lookup"><span data-stu-id="1e513-130">Type</span></span>|<span data-ttu-id="1e513-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1e513-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e513-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e513-132">lastModifiedDateTime</span></span>|<span data-ttu-id="1e513-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e513-133">DateTimeOffset</span></span>|<span data-ttu-id="1e513-134">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="1e513-134">The date and time the object was last modified.</span></span> <span data-ttu-id="1e513-135">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="1e513-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="1e513-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1e513-136">createdDateTime</span></span>|<span data-ttu-id="1e513-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e513-137">DateTimeOffset</span></span>|<span data-ttu-id="1e513-138">Das Datum und die Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="1e513-138">The date and time the object was created.</span></span> <span data-ttu-id="1e513-139">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="1e513-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="1e513-140">id</span><span class="sxs-lookup"><span data-stu-id="1e513-140">id</span></span>|<span data-ttu-id="1e513-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1e513-141">String</span></span>|<span data-ttu-id="1e513-142">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="1e513-142">Key of the entity.</span></span> <span data-ttu-id="1e513-143">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="1e513-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="1e513-144">values</span><span class="sxs-lookup"><span data-stu-id="1e513-144">values</span></span>|<span data-ttu-id="1e513-145">String collection</span><span class="sxs-lookup"><span data-stu-id="1e513-145">String collection</span></span>|<span data-ttu-id="1e513-146">Eine Auflistung von nicht leeren Zeichenfolgen für die zugeordnete Präsentation.</span><span class="sxs-lookup"><span data-stu-id="1e513-146">A collection of non-empty strings for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="1e513-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="1e513-147">Response</span></span>
<span data-ttu-id="1e513-148">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1e513-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e513-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1e513-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e513-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1e513-150">Request</span></span>
<span data-ttu-id="1e513-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1e513-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
  "values": [
    "Values value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="1e513-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="1e513-152">Response</span></span>
<span data-ttu-id="1e513-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1e513-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 292

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "5156903b-903b-5156-3b90-56513b905651",
  "values": [
    "Values value"
  ]
}
```




