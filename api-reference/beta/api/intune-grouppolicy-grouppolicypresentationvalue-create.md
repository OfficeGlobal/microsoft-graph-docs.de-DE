---
title: GroupPolicyPresentationValue erstellen
description: Erstellen eines neuen groupPolicyPresentationValue-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e8e657917d0c07173e9a4a4553a7deaecc0f06f1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160900"
---
# <a name="create-grouppolicypresentationvalue"></a><span data-ttu-id="b75ac-103">GroupPolicyPresentationValue erstellen</span><span class="sxs-lookup"><span data-stu-id="b75ac-103">Create groupPolicyPresentationValue</span></span>

> <span data-ttu-id="b75ac-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b75ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b75ac-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b75ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b75ac-106">Erstellen eines neuen [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b75ac-106">Create a new [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b75ac-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b75ac-107">Prerequisites</span></span>
<span data-ttu-id="b75ac-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b75ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b75ac-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b75ac-110">Permission type</span></span>|<span data-ttu-id="b75ac-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b75ac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b75ac-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b75ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b75ac-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b75ac-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b75ac-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b75ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b75ac-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b75ac-115">Not supported.</span></span>|
|<span data-ttu-id="b75ac-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b75ac-116">Application</span></span>|<span data-ttu-id="b75ac-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b75ac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b75ac-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b75ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="b75ac-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b75ac-119">Request headers</span></span>
|<span data-ttu-id="b75ac-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b75ac-120">Header</span></span>|<span data-ttu-id="b75ac-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b75ac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b75ac-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b75ac-122">Authorization</span></span>|<span data-ttu-id="b75ac-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b75ac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b75ac-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b75ac-124">Accept</span></span>|<span data-ttu-id="b75ac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b75ac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b75ac-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b75ac-126">Request body</span></span>
<span data-ttu-id="b75ac-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das groupPolicyPresentationValue-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="b75ac-127">In the request body, supply a JSON representation for the groupPolicyPresentationValue object.</span></span>

<span data-ttu-id="b75ac-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der groupPolicyPresentationValue erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b75ac-128">The following table shows the properties that are required when you create the groupPolicyPresentationValue.</span></span>

|<span data-ttu-id="b75ac-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b75ac-129">Property</span></span>|<span data-ttu-id="b75ac-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b75ac-130">Type</span></span>|<span data-ttu-id="b75ac-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b75ac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b75ac-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b75ac-132">lastModifiedDateTime</span></span>|<span data-ttu-id="b75ac-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b75ac-133">DateTimeOffset</span></span>|<span data-ttu-id="b75ac-134">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b75ac-134">The date and time the object was last modified.</span></span>|
|<span data-ttu-id="b75ac-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b75ac-135">createdDateTime</span></span>|<span data-ttu-id="b75ac-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b75ac-136">DateTimeOffset</span></span>|<span data-ttu-id="b75ac-137">Das Datum und die Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b75ac-137">The date and time the object was created.</span></span>|
|<span data-ttu-id="b75ac-138">id</span><span class="sxs-lookup"><span data-stu-id="b75ac-138">id</span></span>|<span data-ttu-id="b75ac-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b75ac-139">String</span></span>|<span data-ttu-id="b75ac-140">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b75ac-140">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="b75ac-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="b75ac-141">Response</span></span>
<span data-ttu-id="b75ac-142">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b75ac-142">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b75ac-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b75ac-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="b75ac-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b75ac-144">Request</span></span>
<span data-ttu-id="b75ac-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b75ac-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 70

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue"
}
```

### <a name="response"></a><span data-ttu-id="b75ac-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="b75ac-146">Response</span></span>
<span data-ttu-id="b75ac-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b75ac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "8132eaab-eaab-8132-abea-3281abea3281"
}
```




