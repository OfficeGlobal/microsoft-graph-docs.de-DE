---
title: GroupPolicyConfiguration erstellen
description: Erstellen eines neuen groupPolicyConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 307c12d5b91759618c01f9fa219f50779394a0bf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174713"
---
# <a name="create-grouppolicyconfiguration"></a><span data-ttu-id="ba728-103">GroupPolicyConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="ba728-103">Create groupPolicyConfiguration</span></span>

> <span data-ttu-id="ba728-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ba728-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba728-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ba728-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba728-106">Erstellen eines neuen [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ba728-106">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba728-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ba728-107">Prerequisites</span></span>
<span data-ttu-id="ba728-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ba728-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ba728-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ba728-110">Permission type</span></span>|<span data-ttu-id="ba728-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ba728-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba728-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ba728-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ba728-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba728-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ba728-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ba728-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba728-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ba728-115">Not supported.</span></span>|
|<span data-ttu-id="ba728-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ba728-116">Application</span></span>|<span data-ttu-id="ba728-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ba728-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba728-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ba728-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ba728-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ba728-119">Request headers</span></span>
|<span data-ttu-id="ba728-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ba728-120">Header</span></span>|<span data-ttu-id="ba728-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ba728-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba728-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba728-122">Authorization</span></span>|<span data-ttu-id="ba728-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ba728-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba728-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ba728-124">Accept</span></span>|<span data-ttu-id="ba728-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ba728-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba728-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ba728-126">Request body</span></span>
<span data-ttu-id="ba728-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das groupPolicyConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="ba728-127">In the request body, supply a JSON representation for the groupPolicyConfiguration object.</span></span>

<span data-ttu-id="ba728-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der groupPolicyConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="ba728-128">The following table shows the properties that are required when you create the groupPolicyConfiguration.</span></span>

|<span data-ttu-id="ba728-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ba728-129">Property</span></span>|<span data-ttu-id="ba728-130">Typ</span><span class="sxs-lookup"><span data-stu-id="ba728-130">Type</span></span>|<span data-ttu-id="ba728-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ba728-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba728-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ba728-132">createdDateTime</span></span>|<span data-ttu-id="ba728-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba728-133">DateTimeOffset</span></span>|<span data-ttu-id="ba728-134">Das Datum und die Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="ba728-134">The date and time the object was created.</span></span>|
|<span data-ttu-id="ba728-135">displayName</span><span class="sxs-lookup"><span data-stu-id="ba728-135">displayName</span></span>|<span data-ttu-id="ba728-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ba728-136">String</span></span>|<span data-ttu-id="ba728-137">Vom Benutzer bereitgestellter Name für das Resource-Objekt.</span><span class="sxs-lookup"><span data-stu-id="ba728-137">User provided name for the resource object.</span></span>|
|<span data-ttu-id="ba728-138">description</span><span class="sxs-lookup"><span data-stu-id="ba728-138">description</span></span>|<span data-ttu-id="ba728-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ba728-139">String</span></span>|<span data-ttu-id="ba728-140">Vom Benutzer bereitgestellte Beschreibung für das Resource-Objekt.</span><span class="sxs-lookup"><span data-stu-id="ba728-140">User provided description for the resource object.</span></span>|
|<span data-ttu-id="ba728-141">id</span><span class="sxs-lookup"><span data-stu-id="ba728-141">id</span></span>|<span data-ttu-id="ba728-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ba728-142">String</span></span>|<span data-ttu-id="ba728-143">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ba728-143">Key of the entity.</span></span>|
|<span data-ttu-id="ba728-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba728-144">lastModifiedDateTime</span></span>|<span data-ttu-id="ba728-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba728-145">DateTimeOffset</span></span>|<span data-ttu-id="ba728-146">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="ba728-146">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="ba728-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="ba728-147">Response</span></span>
<span data-ttu-id="ba728-148">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ba728-148">If successful, this method returns a `201 Created` response code and a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba728-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ba728-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba728-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ba728-150">Request</span></span>
<span data-ttu-id="ba728-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ba728-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ba728-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="ba728-152">Response</span></span>
<span data-ttu-id="ba728-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ba728-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




