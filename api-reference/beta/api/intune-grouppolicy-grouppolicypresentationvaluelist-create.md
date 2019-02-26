---
title: GroupPolicyPresentationValueList erstellen
description: Erstellen eines neuen groupPolicyPresentationValueList-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0fcd3dcb33b0442fb96ea16de1faf25c76f3a9e6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139004"
---
# <a name="create-grouppolicypresentationvaluelist"></a><span data-ttu-id="0573a-103">GroupPolicyPresentationValueList erstellen</span><span class="sxs-lookup"><span data-stu-id="0573a-103">Create groupPolicyPresentationValueList</span></span>

> <span data-ttu-id="0573a-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0573a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0573a-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0573a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0573a-106">Erstellen eines neuen [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0573a-106">Create a new [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0573a-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0573a-107">Prerequisites</span></span>
<span data-ttu-id="0573a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0573a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0573a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0573a-110">Permission type</span></span>|<span data-ttu-id="0573a-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0573a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0573a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0573a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0573a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0573a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0573a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0573a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0573a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0573a-115">Not supported.</span></span>|
|<span data-ttu-id="0573a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0573a-116">Application</span></span>|<span data-ttu-id="0573a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0573a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0573a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0573a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="0573a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0573a-119">Request headers</span></span>
|<span data-ttu-id="0573a-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0573a-120">Header</span></span>|<span data-ttu-id="0573a-121">Wert</span><span class="sxs-lookup"><span data-stu-id="0573a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0573a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0573a-122">Authorization</span></span>|<span data-ttu-id="0573a-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0573a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0573a-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0573a-124">Accept</span></span>|<span data-ttu-id="0573a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0573a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0573a-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0573a-126">Request body</span></span>
<span data-ttu-id="0573a-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das groupPolicyPresentationValueList-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="0573a-127">In the request body, supply a JSON representation for the groupPolicyPresentationValueList object.</span></span>

<span data-ttu-id="0573a-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der groupPolicyPresentationValueList erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="0573a-128">The following table shows the properties that are required when you create the groupPolicyPresentationValueList.</span></span>

|<span data-ttu-id="0573a-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0573a-129">Property</span></span>|<span data-ttu-id="0573a-130">Typ</span><span class="sxs-lookup"><span data-stu-id="0573a-130">Type</span></span>|<span data-ttu-id="0573a-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0573a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0573a-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0573a-132">lastModifiedDateTime</span></span>|<span data-ttu-id="0573a-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0573a-133">DateTimeOffset</span></span>|<span data-ttu-id="0573a-134">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0573a-134">The date and time the object was last modified.</span></span> <span data-ttu-id="0573a-135">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="0573a-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="0573a-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0573a-136">createdDateTime</span></span>|<span data-ttu-id="0573a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0573a-137">DateTimeOffset</span></span>|<span data-ttu-id="0573a-138">Das Datum und die Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0573a-138">The date and time the object was created.</span></span> <span data-ttu-id="0573a-139">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="0573a-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="0573a-140">id</span><span class="sxs-lookup"><span data-stu-id="0573a-140">id</span></span>|<span data-ttu-id="0573a-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0573a-141">String</span></span>|<span data-ttu-id="0573a-142">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0573a-142">Key of the entity.</span></span> <span data-ttu-id="0573a-143">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="0573a-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="0573a-144">values</span><span class="sxs-lookup"><span data-stu-id="0573a-144">values</span></span>|<span data-ttu-id="0573a-145">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="0573a-145">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="0573a-146">Eine Liste von Paaren für die zugeordnete Präsentation.</span><span class="sxs-lookup"><span data-stu-id="0573a-146">A list of pairs for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="0573a-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="0573a-147">Response</span></span>
<span data-ttu-id="0573a-148">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0573a-148">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0573a-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0573a-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="0573a-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0573a-150">Request</span></span>
<span data-ttu-id="0573a-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0573a-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
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

### <a name="response"></a><span data-ttu-id="0573a-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="0573a-152">Response</span></span>
<span data-ttu-id="0573a-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0573a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




