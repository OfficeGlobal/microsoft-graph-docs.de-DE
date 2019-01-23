---
title: GroupPolicyPresentation aktualisieren
description: Aktualisieren Sie die Eigenschaften eines GroupPolicyPresentation-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 26f185d1474402f77f8dab09c500a1c11892f77b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431522"
---
# <a name="update-grouppolicypresentation"></a><span data-ttu-id="cfb6b-103">GroupPolicyPresentation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="cfb6b-103">Update groupPolicyPresentation</span></span>

> <span data-ttu-id="cfb6b-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="cfb6b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cfb6b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cfb6b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cfb6b-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cfb6b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfb6b-107">Aktualisieren Sie die Eigenschaften eines [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="cfb6b-107">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cfb6b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cfb6b-108">Prerequisites</span></span>
<span data-ttu-id="cfb6b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="cfb6b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cfb6b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cfb6b-111">Permission type</span></span>|<span data-ttu-id="cfb6b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cfb6b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cfb6b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cfb6b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cfb6b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfb6b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cfb6b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cfb6b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cfb6b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cfb6b-116">Not supported.</span></span>|
|<span data-ttu-id="cfb6b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cfb6b-117">Application</span></span>|<span data-ttu-id="cfb6b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cfb6b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cfb6b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cfb6b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="cfb6b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cfb6b-120">Request headers</span></span>
|<span data-ttu-id="cfb6b-121">Header</span><span class="sxs-lookup"><span data-stu-id="cfb6b-121">Header</span></span>|<span data-ttu-id="cfb6b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="cfb6b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cfb6b-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="cfb6b-123">Authorization</span></span>|<span data-ttu-id="cfb6b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cfb6b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cfb6b-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="cfb6b-125">Accept</span></span>|<span data-ttu-id="cfb6b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cfb6b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfb6b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cfb6b-127">Request body</span></span>
<span data-ttu-id="cfb6b-128">Geben Sie im Textkörper Anforderung für das Objekt [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="cfb6b-128">In the request body, supply a JSON representation for the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

<span data-ttu-id="cfb6b-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="cfb6b-129">The following table shows the properties that are required when you create the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md).</span></span>

|<span data-ttu-id="cfb6b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cfb6b-130">Property</span></span>|<span data-ttu-id="cfb6b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="cfb6b-131">Type</span></span>|<span data-ttu-id="cfb6b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cfb6b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfb6b-133">label</span><span class="sxs-lookup"><span data-stu-id="cfb6b-133">label</span></span>|<span data-ttu-id="cfb6b-134">String</span><span class="sxs-lookup"><span data-stu-id="cfb6b-134">String</span></span>|<span data-ttu-id="cfb6b-135">Lokalisierte Beschriftung für jede Entität Präsentation.</span><span class="sxs-lookup"><span data-stu-id="cfb6b-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="cfb6b-136">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="cfb6b-136">The default value is empty.</span></span>|
|<span data-ttu-id="cfb6b-137">id</span><span class="sxs-lookup"><span data-stu-id="cfb6b-137">id</span></span>|<span data-ttu-id="cfb6b-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cfb6b-138">String</span></span>|<span data-ttu-id="cfb6b-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="cfb6b-139">Key of the entity.</span></span>|
|<span data-ttu-id="cfb6b-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cfb6b-140">lastModifiedDateTime</span></span>|<span data-ttu-id="cfb6b-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfb6b-141">DateTimeOffset</span></span>|<span data-ttu-id="cfb6b-142">Datum und Uhrzeit der letzten Änderung die Entität.</span><span class="sxs-lookup"><span data-stu-id="cfb6b-142">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="cfb6b-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="cfb6b-143">Response</span></span>
<span data-ttu-id="cfb6b-144">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="cfb6b-144">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfb6b-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cfb6b-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="cfb6b-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cfb6b-146">Request</span></span>
<span data-ttu-id="cfb6b-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cfb6b-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="cfb6b-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="cfb6b-148">Response</span></span>
<span data-ttu-id="cfb6b-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cfb6b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 205

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "Label value",
  "id": "a33caa6a-aa6a-a33c-6aaa-3ca36aaa3ca3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




