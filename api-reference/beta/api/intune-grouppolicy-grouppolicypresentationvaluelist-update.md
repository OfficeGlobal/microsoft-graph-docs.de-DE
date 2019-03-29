---
title: GroupPolicyPresentationValueList aktualisieren
description: Aktualisieren der Eigenschaften eines groupPolicyPresentationValueList-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1e2be7f3f6f1cab47174f8be78ec9655e1d368fd
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983470"
---
# <a name="update-grouppolicypresentationvaluelist"></a><span data-ttu-id="b9bf3-103">GroupPolicyPresentationValueList aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b9bf3-103">Update groupPolicyPresentationValueList</span></span>

> <span data-ttu-id="b9bf3-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b9bf3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9bf3-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b9bf3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9bf3-106">Aktualisieren der Eigenschaften eines [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b9bf3-106">Update the properties of a [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9bf3-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b9bf3-107">Prerequisites</span></span>
<span data-ttu-id="b9bf3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9bf3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9bf3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b9bf3-110">Permission type</span></span>|<span data-ttu-id="b9bf3-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b9bf3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9bf3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b9bf3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b9bf3-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9bf3-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b9bf3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b9bf3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9bf3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9bf3-115">Not supported.</span></span>|
|<span data-ttu-id="b9bf3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b9bf3-116">Application</span></span>|<span data-ttu-id="b9bf3-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9bf3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9bf3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9bf3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="b9bf3-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b9bf3-119">Request headers</span></span>
|<span data-ttu-id="b9bf3-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b9bf3-120">Header</span></span>|<span data-ttu-id="b9bf3-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b9bf3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9bf3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9bf3-122">Authorization</span></span>|<span data-ttu-id="b9bf3-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b9bf3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9bf3-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b9bf3-124">Accept</span></span>|<span data-ttu-id="b9bf3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b9bf3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9bf3-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b9bf3-126">Request body</span></span>
<span data-ttu-id="b9bf3-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="b9bf3-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

<span data-ttu-id="b9bf3-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b9bf3-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md).</span></span>

|<span data-ttu-id="b9bf3-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b9bf3-129">Property</span></span>|<span data-ttu-id="b9bf3-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b9bf3-130">Type</span></span>|<span data-ttu-id="b9bf3-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9bf3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9bf3-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9bf3-132">lastModifiedDateTime</span></span>|<span data-ttu-id="b9bf3-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9bf3-133">DateTimeOffset</span></span>|<span data-ttu-id="b9bf3-134">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b9bf3-134">The date and time the object was last modified.</span></span> <span data-ttu-id="b9bf3-135">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b9bf3-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="b9bf3-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b9bf3-136">createdDateTime</span></span>|<span data-ttu-id="b9bf3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9bf3-137">DateTimeOffset</span></span>|<span data-ttu-id="b9bf3-138">Das Datum und die Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b9bf3-138">The date and time the object was created.</span></span> <span data-ttu-id="b9bf3-139">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b9bf3-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="b9bf3-140">id</span><span class="sxs-lookup"><span data-stu-id="b9bf3-140">id</span></span>|<span data-ttu-id="b9bf3-141">String</span><span class="sxs-lookup"><span data-stu-id="b9bf3-141">String</span></span>|<span data-ttu-id="b9bf3-142">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b9bf3-142">Key of the entity.</span></span> <span data-ttu-id="b9bf3-143">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b9bf3-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="b9bf3-144">values</span><span class="sxs-lookup"><span data-stu-id="b9bf3-144">values</span></span>|<span data-ttu-id="b9bf3-145">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b9bf3-145">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b9bf3-146">Eine Liste von Paaren für die zugeordnete Präsentation.</span><span class="sxs-lookup"><span data-stu-id="b9bf3-146">A list of pairs for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="b9bf3-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9bf3-147">Response</span></span>
<span data-ttu-id="b9bf3-148">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b9bf3-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9bf3-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b9bf3-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9bf3-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9bf3-150">Request</span></span>
<span data-ttu-id="b9bf3-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b9bf3-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 222

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueList",
  "values": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b9bf3-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9bf3-152">Response</span></span>
<span data-ttu-id="b9bf3-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b9bf3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 394

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueList",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "1dbb7865-7865-1dbb-6578-bb1d6578bb1d",
  "values": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ]
}
```




