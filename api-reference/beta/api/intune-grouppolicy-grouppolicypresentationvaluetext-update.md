---
title: GroupPolicyPresentationValueText aktualisieren
description: Aktualisieren der Eigenschaften eines groupPolicyPresentationValueText-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 59705a0463cd313cbc8fb8af0f267a09f5929fac
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150932"
---
# <a name="update-grouppolicypresentationvaluetext"></a><span data-ttu-id="fbc74-103">GroupPolicyPresentationValueText aktualisieren</span><span class="sxs-lookup"><span data-stu-id="fbc74-103">Update groupPolicyPresentationValueText</span></span>

> <span data-ttu-id="fbc74-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fbc74-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbc74-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="fbc74-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbc74-106">Aktualisieren der Eigenschaften eines [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="fbc74-106">Update the properties of a [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fbc74-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fbc74-107">Prerequisites</span></span>
<span data-ttu-id="fbc74-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fbc74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fbc74-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fbc74-110">Permission type</span></span>|<span data-ttu-id="fbc74-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fbc74-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbc74-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fbc74-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fbc74-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbc74-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fbc74-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fbc74-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbc74-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fbc74-115">Not supported.</span></span>|
|<span data-ttu-id="fbc74-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fbc74-116">Application</span></span>|<span data-ttu-id="fbc74-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fbc74-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbc74-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fbc74-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="fbc74-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fbc74-119">Request headers</span></span>
|<span data-ttu-id="fbc74-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fbc74-120">Header</span></span>|<span data-ttu-id="fbc74-121">Wert</span><span class="sxs-lookup"><span data-stu-id="fbc74-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbc74-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbc74-122">Authorization</span></span>|<span data-ttu-id="fbc74-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fbc74-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbc74-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fbc74-124">Accept</span></span>|<span data-ttu-id="fbc74-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fbc74-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbc74-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fbc74-126">Request body</span></span>
<span data-ttu-id="fbc74-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="fbc74-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

<span data-ttu-id="fbc74-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="fbc74-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md).</span></span>

|<span data-ttu-id="fbc74-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fbc74-129">Property</span></span>|<span data-ttu-id="fbc74-130">Typ</span><span class="sxs-lookup"><span data-stu-id="fbc74-130">Type</span></span>|<span data-ttu-id="fbc74-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fbc74-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbc74-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fbc74-132">lastModifiedDateTime</span></span>|<span data-ttu-id="fbc74-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbc74-133">DateTimeOffset</span></span>|<span data-ttu-id="fbc74-134">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="fbc74-134">The date and time the object was last modified.</span></span> <span data-ttu-id="fbc74-135">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="fbc74-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="fbc74-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fbc74-136">createdDateTime</span></span>|<span data-ttu-id="fbc74-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbc74-137">DateTimeOffset</span></span>|<span data-ttu-id="fbc74-138">Das Datum und die Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="fbc74-138">The date and time the object was created.</span></span> <span data-ttu-id="fbc74-139">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="fbc74-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="fbc74-140">id</span><span class="sxs-lookup"><span data-stu-id="fbc74-140">id</span></span>|<span data-ttu-id="fbc74-141">String</span><span class="sxs-lookup"><span data-stu-id="fbc74-141">String</span></span>|<span data-ttu-id="fbc74-142">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="fbc74-142">Key of the entity.</span></span> <span data-ttu-id="fbc74-143">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="fbc74-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="fbc74-144">Wert</span><span class="sxs-lookup"><span data-stu-id="fbc74-144">value</span></span>|<span data-ttu-id="fbc74-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fbc74-145">String</span></span>|<span data-ttu-id="fbc74-146">Ein String-Wert für die zugeordnete Präsentation.</span><span class="sxs-lookup"><span data-stu-id="fbc74-146">A string value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="fbc74-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="fbc74-147">Response</span></span>
<span data-ttu-id="fbc74-148">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fbc74-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbc74-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fbc74-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbc74-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fbc74-150">Request</span></span>
<span data-ttu-id="fbc74-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fbc74-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 101

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "value": "Value value"
}
```

### <a name="response"></a><span data-ttu-id="fbc74-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="fbc74-152">Response</span></span>
<span data-ttu-id="fbc74-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fbc74-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "a3883444-3444-a388-4434-88a3443488a3",
  "value": "Value value"
}
```




