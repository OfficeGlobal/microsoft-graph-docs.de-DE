---
title: GroupPolicyPresentationValueLongDecimal erstellen
description: Erstellen eines neuen groupPolicyPresentationValueLongDecimal-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c9443f0aa2445979f0b960662e9d8d989c4ca3dd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160438"
---
# <a name="create-grouppolicypresentationvaluelongdecimal"></a><span data-ttu-id="b20a1-103">GroupPolicyPresentationValueLongDecimal erstellen</span><span class="sxs-lookup"><span data-stu-id="b20a1-103">Create groupPolicyPresentationValueLongDecimal</span></span>

> <span data-ttu-id="b20a1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b20a1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b20a1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b20a1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b20a1-106">Erstellen eines neuen [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b20a1-106">Create a new [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b20a1-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b20a1-107">Prerequisites</span></span>
<span data-ttu-id="b20a1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b20a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b20a1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b20a1-110">Permission type</span></span>|<span data-ttu-id="b20a1-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b20a1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b20a1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b20a1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b20a1-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b20a1-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b20a1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b20a1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b20a1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b20a1-115">Not supported.</span></span>|
|<span data-ttu-id="b20a1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b20a1-116">Application</span></span>|<span data-ttu-id="b20a1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b20a1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b20a1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b20a1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="b20a1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b20a1-119">Request headers</span></span>
|<span data-ttu-id="b20a1-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b20a1-120">Header</span></span>|<span data-ttu-id="b20a1-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b20a1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b20a1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b20a1-122">Authorization</span></span>|<span data-ttu-id="b20a1-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b20a1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b20a1-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b20a1-124">Accept</span></span>|<span data-ttu-id="b20a1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b20a1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b20a1-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b20a1-126">Request body</span></span>
<span data-ttu-id="b20a1-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das groupPolicyPresentationValueLongDecimal-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="b20a1-127">In the request body, supply a JSON representation for the groupPolicyPresentationValueLongDecimal object.</span></span>

<span data-ttu-id="b20a1-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der groupPolicyPresentationValueLongDecimal erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b20a1-128">The following table shows the properties that are required when you create the groupPolicyPresentationValueLongDecimal.</span></span>

|<span data-ttu-id="b20a1-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b20a1-129">Property</span></span>|<span data-ttu-id="b20a1-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b20a1-130">Type</span></span>|<span data-ttu-id="b20a1-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b20a1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b20a1-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b20a1-132">lastModifiedDateTime</span></span>|<span data-ttu-id="b20a1-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b20a1-133">DateTimeOffset</span></span>|<span data-ttu-id="b20a1-134">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b20a1-134">The date and time the object was last modified.</span></span> <span data-ttu-id="b20a1-135">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b20a1-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="b20a1-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b20a1-136">createdDateTime</span></span>|<span data-ttu-id="b20a1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b20a1-137">DateTimeOffset</span></span>|<span data-ttu-id="b20a1-138">Das Datum und die Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b20a1-138">The date and time the object was created.</span></span> <span data-ttu-id="b20a1-139">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b20a1-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="b20a1-140">id</span><span class="sxs-lookup"><span data-stu-id="b20a1-140">id</span></span>|<span data-ttu-id="b20a1-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b20a1-141">String</span></span>|<span data-ttu-id="b20a1-142">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b20a1-142">Key of the entity.</span></span> <span data-ttu-id="b20a1-143">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b20a1-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="b20a1-144">Wert</span><span class="sxs-lookup"><span data-stu-id="b20a1-144">value</span></span>|<span data-ttu-id="b20a1-145">Int64</span><span class="sxs-lookup"><span data-stu-id="b20a1-145">Int64</span></span>|<span data-ttu-id="b20a1-146">Ein unsigned long-Wert für die zugeordnete Präsentation.</span><span class="sxs-lookup"><span data-stu-id="b20a1-146">An unsigned long value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="b20a1-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="b20a1-147">Response</span></span>
<span data-ttu-id="b20a1-148">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b20a1-148">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b20a1-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b20a1-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="b20a1-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b20a1-150">Request</span></span>
<span data-ttu-id="b20a1-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b20a1-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="b20a1-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="b20a1-152">Response</span></span>
<span data-ttu-id="b20a1-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b20a1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 268

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "210f7078-7078-210f-7870-0f2178700f21",
  "value": 5
}
```




