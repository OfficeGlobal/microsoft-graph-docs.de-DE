---
title: Erstellen von groupPolicyPresentationValueText
description: Erstellen eines neuen GroupPolicyPresentationValueText-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b71d21691ade34a827e06198d387c21585576297
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431501"
---
# <a name="create-grouppolicypresentationvaluetext"></a><span data-ttu-id="2ebc1-103">Erstellen von groupPolicyPresentationValueText</span><span class="sxs-lookup"><span data-stu-id="2ebc1-103">Create groupPolicyPresentationValueText</span></span>

> <span data-ttu-id="2ebc1-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="2ebc1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2ebc1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2ebc1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2ebc1-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2ebc1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ebc1-107">Erstellen eines neuen [GroupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2ebc1-107">Create a new [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ebc1-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2ebc1-108">Prerequisites</span></span>
<span data-ttu-id="2ebc1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2ebc1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2ebc1-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2ebc1-111">Permission type</span></span>|<span data-ttu-id="2ebc1-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2ebc1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ebc1-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2ebc1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2ebc1-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ebc1-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2ebc1-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2ebc1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ebc1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2ebc1-116">Not supported.</span></span>|
|<span data-ttu-id="2ebc1-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2ebc1-117">Application</span></span>|<span data-ttu-id="2ebc1-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2ebc1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ebc1-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2ebc1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="2ebc1-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2ebc1-120">Request headers</span></span>
|<span data-ttu-id="2ebc1-121">Header</span><span class="sxs-lookup"><span data-stu-id="2ebc1-121">Header</span></span>|<span data-ttu-id="2ebc1-122">Wert</span><span class="sxs-lookup"><span data-stu-id="2ebc1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ebc1-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="2ebc1-123">Authorization</span></span>|<span data-ttu-id="2ebc1-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2ebc1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ebc1-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2ebc1-125">Accept</span></span>|<span data-ttu-id="2ebc1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2ebc1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ebc1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2ebc1-127">Request body</span></span>
<span data-ttu-id="2ebc1-128">Geben Sie im Textkörper Anforderung für das Objekt GroupPolicyPresentationValueText eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="2ebc1-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueText object.</span></span>

<span data-ttu-id="2ebc1-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die GroupPolicyPresentationValueText erstellen.</span><span class="sxs-lookup"><span data-stu-id="2ebc1-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueText.</span></span>

|<span data-ttu-id="2ebc1-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2ebc1-130">Property</span></span>|<span data-ttu-id="2ebc1-131">Typ</span><span class="sxs-lookup"><span data-stu-id="2ebc1-131">Type</span></span>|<span data-ttu-id="2ebc1-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2ebc1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ebc1-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ebc1-133">lastModifiedDateTime</span></span>|<span data-ttu-id="2ebc1-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ebc1-134">DateTimeOffset</span></span>|<span data-ttu-id="2ebc1-135">Das Datum und die Zeit, die das Objekt zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="2ebc1-135">The date and time the object was last modified.</span></span> <span data-ttu-id="2ebc1-136">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="2ebc1-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="2ebc1-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2ebc1-137">createdDateTime</span></span>|<span data-ttu-id="2ebc1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ebc1-138">DateTimeOffset</span></span>|<span data-ttu-id="2ebc1-139">Das Datum und die Zeit, die das Objekt erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="2ebc1-139">The date and time the object was created.</span></span> <span data-ttu-id="2ebc1-140">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="2ebc1-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="2ebc1-141">id</span><span class="sxs-lookup"><span data-stu-id="2ebc1-141">id</span></span>|<span data-ttu-id="2ebc1-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2ebc1-142">String</span></span>|<span data-ttu-id="2ebc1-143">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2ebc1-143">Key of the entity.</span></span> <span data-ttu-id="2ebc1-144">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="2ebc1-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="2ebc1-145">Wert</span><span class="sxs-lookup"><span data-stu-id="2ebc1-145">value</span></span>|<span data-ttu-id="2ebc1-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2ebc1-146">String</span></span>|<span data-ttu-id="2ebc1-147">Ein String-Wert für die zugehörige Präsentation.</span><span class="sxs-lookup"><span data-stu-id="2ebc1-147">A string value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="2ebc1-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="2ebc1-148">Response</span></span>
<span data-ttu-id="2ebc1-149">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [GroupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="2ebc1-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ebc1-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2ebc1-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ebc1-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2ebc1-151">Request</span></span>
<span data-ttu-id="2ebc1-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2ebc1-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 101

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "value": "Value value"
}
```

### <a name="response"></a><span data-ttu-id="2ebc1-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="2ebc1-153">Response</span></span>
<span data-ttu-id="2ebc1-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2ebc1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




