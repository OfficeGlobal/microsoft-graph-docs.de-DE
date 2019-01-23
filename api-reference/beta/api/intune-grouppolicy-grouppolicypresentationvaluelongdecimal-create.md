---
title: Erstellen von groupPolicyPresentationValueLongDecimal
description: Erstellen eines neuen GroupPolicyPresentationValueLongDecimal-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 51dacbea1970d042d4fe1fb5b3b2bd42f522b131
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430149"
---
# <a name="create-grouppolicypresentationvaluelongdecimal"></a><span data-ttu-id="f19bf-103">Erstellen von groupPolicyPresentationValueLongDecimal</span><span class="sxs-lookup"><span data-stu-id="f19bf-103">Create groupPolicyPresentationValueLongDecimal</span></span>

> <span data-ttu-id="f19bf-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="f19bf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f19bf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f19bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f19bf-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f19bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f19bf-107">Erstellen eines neuen [GroupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f19bf-107">Create a new [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f19bf-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f19bf-108">Prerequisites</span></span>
<span data-ttu-id="f19bf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f19bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f19bf-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f19bf-111">Permission type</span></span>|<span data-ttu-id="f19bf-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f19bf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f19bf-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f19bf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f19bf-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f19bf-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f19bf-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f19bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f19bf-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f19bf-116">Not supported.</span></span>|
|<span data-ttu-id="f19bf-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f19bf-117">Application</span></span>|<span data-ttu-id="f19bf-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f19bf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f19bf-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f19bf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="f19bf-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f19bf-120">Request headers</span></span>
|<span data-ttu-id="f19bf-121">Header</span><span class="sxs-lookup"><span data-stu-id="f19bf-121">Header</span></span>|<span data-ttu-id="f19bf-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f19bf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f19bf-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f19bf-123">Authorization</span></span>|<span data-ttu-id="f19bf-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f19bf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f19bf-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f19bf-125">Accept</span></span>|<span data-ttu-id="f19bf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f19bf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f19bf-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f19bf-127">Request body</span></span>
<span data-ttu-id="f19bf-128">Geben Sie im Textkörper Anforderung für das Objekt GroupPolicyPresentationValueLongDecimal eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="f19bf-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueLongDecimal object.</span></span>

<span data-ttu-id="f19bf-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die GroupPolicyPresentationValueLongDecimal erstellen.</span><span class="sxs-lookup"><span data-stu-id="f19bf-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueLongDecimal.</span></span>

|<span data-ttu-id="f19bf-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f19bf-130">Property</span></span>|<span data-ttu-id="f19bf-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f19bf-131">Type</span></span>|<span data-ttu-id="f19bf-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f19bf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f19bf-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f19bf-133">lastModifiedDateTime</span></span>|<span data-ttu-id="f19bf-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f19bf-134">DateTimeOffset</span></span>|<span data-ttu-id="f19bf-135">Das Datum und die Zeit, die das Objekt zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="f19bf-135">The date and time the object was last modified.</span></span> <span data-ttu-id="f19bf-136">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="f19bf-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="f19bf-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f19bf-137">createdDateTime</span></span>|<span data-ttu-id="f19bf-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f19bf-138">DateTimeOffset</span></span>|<span data-ttu-id="f19bf-139">Das Datum und die Zeit, die das Objekt erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="f19bf-139">The date and time the object was created.</span></span> <span data-ttu-id="f19bf-140">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="f19bf-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="f19bf-141">id</span><span class="sxs-lookup"><span data-stu-id="f19bf-141">id</span></span>|<span data-ttu-id="f19bf-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f19bf-142">String</span></span>|<span data-ttu-id="f19bf-143">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f19bf-143">Key of the entity.</span></span> <span data-ttu-id="f19bf-144">Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="f19bf-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="f19bf-145">Wert</span><span class="sxs-lookup"><span data-stu-id="f19bf-145">value</span></span>|<span data-ttu-id="f19bf-146">Int64</span><span class="sxs-lookup"><span data-stu-id="f19bf-146">Int64</span></span>|<span data-ttu-id="f19bf-147">Eine nicht signierte long-Wert für die zugehörige Präsentation.</span><span class="sxs-lookup"><span data-stu-id="f19bf-147">An unsigned long value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="f19bf-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="f19bf-148">Response</span></span>
<span data-ttu-id="f19bf-149">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [GroupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f19bf-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f19bf-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f19bf-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="f19bf-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f19bf-151">Request</span></span>
<span data-ttu-id="f19bf-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f19bf-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="f19bf-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="f19bf-153">Response</span></span>
<span data-ttu-id="f19bf-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f19bf-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




