---
title: Aktualisieren von „termsAndConditionsAcceptanceStatus“
description: Aktualisieren der Eigenschaften eines termsAndConditionsAcceptanceStatus-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 846cb823ab567aebea75dacf78ee3a3d36082578
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986278"
---
# <a name="update-termsandconditionsacceptancestatus"></a><span data-ttu-id="1a8f8-103">Aktualisieren von „termsAndConditionsAcceptanceStatus“</span><span class="sxs-lookup"><span data-stu-id="1a8f8-103">Update termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="1a8f8-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1a8f8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a8f8-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1a8f8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a8f8-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="1a8f8-106">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a8f8-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1a8f8-107">Prerequisites</span></span>
<span data-ttu-id="1a8f8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a8f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a8f8-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1a8f8-110">Permission type</span></span>|<span data-ttu-id="1a8f8-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1a8f8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a8f8-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1a8f8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1a8f8-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a8f8-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1a8f8-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1a8f8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a8f8-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1a8f8-115">Not supported.</span></span>|
|<span data-ttu-id="1a8f8-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1a8f8-116">Application</span></span>|<span data-ttu-id="1a8f8-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1a8f8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a8f8-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1a8f8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="1a8f8-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1a8f8-119">Request headers</span></span>
|<span data-ttu-id="1a8f8-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1a8f8-120">Header</span></span>|<span data-ttu-id="1a8f8-121">Wert</span><span class="sxs-lookup"><span data-stu-id="1a8f8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a8f8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a8f8-122">Authorization</span></span>|<span data-ttu-id="1a8f8-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1a8f8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a8f8-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1a8f8-124">Accept</span></span>|<span data-ttu-id="1a8f8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1a8f8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a8f8-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1a8f8-126">Request body</span></span>
<span data-ttu-id="1a8f8-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) an.</span><span class="sxs-lookup"><span data-stu-id="1a8f8-127">In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

<span data-ttu-id="1a8f8-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="1a8f8-128">The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>

|<span data-ttu-id="1a8f8-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1a8f8-129">Property</span></span>|<span data-ttu-id="1a8f8-130">Typ</span><span class="sxs-lookup"><span data-stu-id="1a8f8-130">Type</span></span>|<span data-ttu-id="1a8f8-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1a8f8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a8f8-132">id</span><span class="sxs-lookup"><span data-stu-id="1a8f8-132">id</span></span>|<span data-ttu-id="1a8f8-133">String</span><span class="sxs-lookup"><span data-stu-id="1a8f8-133">String</span></span>|<span data-ttu-id="1a8f8-134">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="1a8f8-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="1a8f8-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="1a8f8-135">userDisplayName</span></span>|<span data-ttu-id="1a8f8-136">String</span><span class="sxs-lookup"><span data-stu-id="1a8f8-136">String</span></span>|<span data-ttu-id="1a8f8-137">Anzeigename des Benutzers, dessen Zustimmung die Entität darstellt</span><span class="sxs-lookup"><span data-stu-id="1a8f8-137">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="1a8f8-138">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="1a8f8-138">acceptedVersion</span></span>|<span data-ttu-id="1a8f8-139">Int32</span><span class="sxs-lookup"><span data-stu-id="1a8f8-139">Int32</span></span>|<span data-ttu-id="1a8f8-140">Versionsnummer der neuesten Version der Geschäftsbedingungen, die der Benutzer akzeptiert hat</span><span class="sxs-lookup"><span data-stu-id="1a8f8-140">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="1a8f8-141">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a8f8-141">acceptedDateTime</span></span>|<span data-ttu-id="1a8f8-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a8f8-142">DateTimeOffset</span></span>|<span data-ttu-id="1a8f8-143">Datum und Uhrzeit der letzten Zustimmung zu den Bedingungen durch den Benutzer</span><span class="sxs-lookup"><span data-stu-id="1a8f8-143">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="1a8f8-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="1a8f8-144">Response</span></span>
<span data-ttu-id="1a8f8-145">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1a8f8-145">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a8f8-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1a8f8-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a8f8-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1a8f8-147">Request</span></span>
<span data-ttu-id="1a8f8-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1a8f8-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="1a8f8-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="1a8f8-149">Response</span></span>
<span data-ttu-id="1a8f8-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1a8f8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```




