---
title: Erstellen von groupPolicyConfiguration
description: Erstellen eines neuen GroupPolicyConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f5ce3f8408d8a6e404ac17e865cc81bb2094c0cc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430214"
---
# <a name="create-grouppolicyconfiguration"></a><span data-ttu-id="9366c-103">Erstellen von groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="9366c-103">Create groupPolicyConfiguration</span></span>

> <span data-ttu-id="9366c-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="9366c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9366c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9366c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9366c-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9366c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9366c-107">Erstellen eines neuen [GroupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="9366c-107">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9366c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9366c-108">Prerequisites</span></span>
<span data-ttu-id="9366c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9366c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9366c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9366c-111">Permission type</span></span>|<span data-ttu-id="9366c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9366c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9366c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9366c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9366c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9366c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9366c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9366c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9366c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9366c-116">Not supported.</span></span>|
|<span data-ttu-id="9366c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9366c-117">Application</span></span>|<span data-ttu-id="9366c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9366c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9366c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9366c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9366c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9366c-120">Request headers</span></span>
|<span data-ttu-id="9366c-121">Header</span><span class="sxs-lookup"><span data-stu-id="9366c-121">Header</span></span>|<span data-ttu-id="9366c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="9366c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9366c-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9366c-123">Authorization</span></span>|<span data-ttu-id="9366c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9366c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9366c-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9366c-125">Accept</span></span>|<span data-ttu-id="9366c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9366c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9366c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9366c-127">Request body</span></span>
<span data-ttu-id="9366c-128">Geben Sie im Textkörper Anforderung für das Objekt GroupPolicyConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="9366c-128">In the request body, supply a JSON representation for the groupPolicyConfiguration object.</span></span>

<span data-ttu-id="9366c-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die GroupPolicyConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="9366c-129">The following table shows the properties that are required when you create the groupPolicyConfiguration.</span></span>

|<span data-ttu-id="9366c-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9366c-130">Property</span></span>|<span data-ttu-id="9366c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="9366c-131">Type</span></span>|<span data-ttu-id="9366c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9366c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9366c-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9366c-133">createdDateTime</span></span>|<span data-ttu-id="9366c-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9366c-134">DateTimeOffset</span></span>|<span data-ttu-id="9366c-135">Das Datum und die Zeit, die das Objekt erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="9366c-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="9366c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9366c-136">displayName</span></span>|<span data-ttu-id="9366c-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9366c-137">String</span></span>|<span data-ttu-id="9366c-138">Der vom Benutzer bereitgestellte Name für das Resource-Objekt.</span><span class="sxs-lookup"><span data-stu-id="9366c-138">User provided name for the resource object.</span></span>|
|<span data-ttu-id="9366c-139">description</span><span class="sxs-lookup"><span data-stu-id="9366c-139">description</span></span>|<span data-ttu-id="9366c-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9366c-140">String</span></span>|<span data-ttu-id="9366c-141">Vom Benutzer bereitgestellte Beschreibung für das Resource-Objekt.</span><span class="sxs-lookup"><span data-stu-id="9366c-141">User provided description for the resource object.</span></span>|
|<span data-ttu-id="9366c-142">id</span><span class="sxs-lookup"><span data-stu-id="9366c-142">id</span></span>|<span data-ttu-id="9366c-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9366c-143">String</span></span>|<span data-ttu-id="9366c-144">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9366c-144">Key of the entity.</span></span>|
|<span data-ttu-id="9366c-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9366c-145">lastModifiedDateTime</span></span>|<span data-ttu-id="9366c-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9366c-146">DateTimeOffset</span></span>|<span data-ttu-id="9366c-147">Datum und Uhrzeit der letzten Änderung die Entität.</span><span class="sxs-lookup"><span data-stu-id="9366c-147">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="9366c-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="9366c-148">Response</span></span>
<span data-ttu-id="9366c-149">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [GroupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="9366c-149">If successful, this method returns a `201 Created` response code and a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9366c-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9366c-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="9366c-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9366c-151">Request</span></span>
<span data-ttu-id="9366c-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9366c-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations
Content-type: application/json
Content-length: 145

{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="9366c-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="9366c-153">Response</span></span>
<span data-ttu-id="9366c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9366c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 317

{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "id": "27b935ec-35ec-27b9-ec35-b927ec35b927",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




