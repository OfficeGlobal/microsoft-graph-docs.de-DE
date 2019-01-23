---
title: Erstellen von groupPolicyPresentationValue
description: Erstellen eines neuen GroupPolicyPresentationValue-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a6fbf02bdf9fb1c5d7f5fe5790943a956f2200c2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430091"
---
# <a name="create-grouppolicypresentationvalue"></a><span data-ttu-id="0861a-103">Erstellen von groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="0861a-103">Create groupPolicyPresentationValue</span></span>

> <span data-ttu-id="0861a-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="0861a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0861a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0861a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0861a-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0861a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0861a-107">Erstellen eines neuen [GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0861a-107">Create a new [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0861a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0861a-108">Prerequisites</span></span>
<span data-ttu-id="0861a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0861a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0861a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0861a-111">Permission type</span></span>|<span data-ttu-id="0861a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0861a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0861a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0861a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0861a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0861a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0861a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0861a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0861a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0861a-116">Not supported.</span></span>|
|<span data-ttu-id="0861a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0861a-117">Application</span></span>|<span data-ttu-id="0861a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0861a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0861a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0861a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="0861a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0861a-120">Request headers</span></span>
|<span data-ttu-id="0861a-121">Header</span><span class="sxs-lookup"><span data-stu-id="0861a-121">Header</span></span>|<span data-ttu-id="0861a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0861a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0861a-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0861a-123">Authorization</span></span>|<span data-ttu-id="0861a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0861a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0861a-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0861a-125">Accept</span></span>|<span data-ttu-id="0861a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0861a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0861a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0861a-127">Request body</span></span>
<span data-ttu-id="0861a-128">Geben Sie im Textkörper Anforderung für das Objekt GroupPolicyPresentationValue eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="0861a-128">In the request body, supply a JSON representation for the groupPolicyPresentationValue object.</span></span>

<span data-ttu-id="0861a-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die GroupPolicyPresentationValue erstellen.</span><span class="sxs-lookup"><span data-stu-id="0861a-129">The following table shows the properties that are required when you create the groupPolicyPresentationValue.</span></span>

|<span data-ttu-id="0861a-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0861a-130">Property</span></span>|<span data-ttu-id="0861a-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0861a-131">Type</span></span>|<span data-ttu-id="0861a-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0861a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0861a-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0861a-133">lastModifiedDateTime</span></span>|<span data-ttu-id="0861a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0861a-134">DateTimeOffset</span></span>|<span data-ttu-id="0861a-135">Das Datum und die Zeit, die das Objekt zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="0861a-135">The date and time the object was last modified.</span></span>|
|<span data-ttu-id="0861a-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0861a-136">createdDateTime</span></span>|<span data-ttu-id="0861a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0861a-137">DateTimeOffset</span></span>|<span data-ttu-id="0861a-138">Das Datum und die Zeit, die das Objekt erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="0861a-138">The date and time the object was created.</span></span>|
|<span data-ttu-id="0861a-139">id</span><span class="sxs-lookup"><span data-stu-id="0861a-139">id</span></span>|<span data-ttu-id="0861a-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0861a-140">String</span></span>|<span data-ttu-id="0861a-141">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0861a-141">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="0861a-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="0861a-142">Response</span></span>
<span data-ttu-id="0861a-143">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0861a-143">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0861a-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0861a-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="0861a-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0861a-145">Request</span></span>
<span data-ttu-id="0861a-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0861a-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 70

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue"
}
```

### <a name="response"></a><span data-ttu-id="0861a-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="0861a-147">Response</span></span>
<span data-ttu-id="0861a-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0861a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




