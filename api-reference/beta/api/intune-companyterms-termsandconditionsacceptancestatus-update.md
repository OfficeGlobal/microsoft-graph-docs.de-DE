---
title: Aktualisieren von „termsAndConditionsAcceptanceStatus“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs termsAndConditionsAcceptanceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b48633ca987558cc4521d406c0518f6ad07d5d58
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150806"
---
# <a name="update-termsandconditionsacceptancestatus"></a><span data-ttu-id="2eb20-103">Aktualisieren von „termsAndConditionsAcceptanceStatus“</span><span class="sxs-lookup"><span data-stu-id="2eb20-103">Update termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="2eb20-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2eb20-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2eb20-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2eb20-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2eb20-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="2eb20-106">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2eb20-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2eb20-107">Prerequisites</span></span>
<span data-ttu-id="2eb20-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2eb20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2eb20-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2eb20-110">Permission type</span></span>|<span data-ttu-id="2eb20-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2eb20-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2eb20-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2eb20-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2eb20-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2eb20-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2eb20-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2eb20-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2eb20-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2eb20-115">Not supported.</span></span>|
|<span data-ttu-id="2eb20-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2eb20-116">Application</span></span>|<span data-ttu-id="2eb20-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2eb20-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2eb20-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2eb20-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="2eb20-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2eb20-119">Request headers</span></span>
|<span data-ttu-id="2eb20-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2eb20-120">Header</span></span>|<span data-ttu-id="2eb20-121">Wert</span><span class="sxs-lookup"><span data-stu-id="2eb20-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2eb20-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2eb20-122">Authorization</span></span>|<span data-ttu-id="2eb20-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2eb20-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2eb20-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2eb20-124">Accept</span></span>|<span data-ttu-id="2eb20-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2eb20-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2eb20-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2eb20-126">Request body</span></span>
<span data-ttu-id="2eb20-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) an.</span><span class="sxs-lookup"><span data-stu-id="2eb20-127">In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

<span data-ttu-id="2eb20-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="2eb20-128">The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>

|<span data-ttu-id="2eb20-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2eb20-129">Property</span></span>|<span data-ttu-id="2eb20-130">Typ</span><span class="sxs-lookup"><span data-stu-id="2eb20-130">Type</span></span>|<span data-ttu-id="2eb20-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2eb20-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2eb20-132">id</span><span class="sxs-lookup"><span data-stu-id="2eb20-132">id</span></span>|<span data-ttu-id="2eb20-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2eb20-133">String</span></span>|<span data-ttu-id="2eb20-134">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="2eb20-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="2eb20-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="2eb20-135">userDisplayName</span></span>|<span data-ttu-id="2eb20-136">String</span><span class="sxs-lookup"><span data-stu-id="2eb20-136">String</span></span>|<span data-ttu-id="2eb20-137">Anzeigename des Benutzers, dessen Zustimmung die Entität darstellt</span><span class="sxs-lookup"><span data-stu-id="2eb20-137">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="2eb20-138">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="2eb20-138">acceptedVersion</span></span>|<span data-ttu-id="2eb20-139">Int32</span><span class="sxs-lookup"><span data-stu-id="2eb20-139">Int32</span></span>|<span data-ttu-id="2eb20-140">Die Versionsnummer der neuesten Version der Geschäftsbedingungen, die der Benutzer akzeptiert hat</span><span class="sxs-lookup"><span data-stu-id="2eb20-140">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="2eb20-141">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="2eb20-141">acceptedDateTime</span></span>|<span data-ttu-id="2eb20-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2eb20-142">DateTimeOffset</span></span>|<span data-ttu-id="2eb20-143">Datum und Uhrzeit der letzten Zustimmung zu den Bedingungen durch den Benutzer</span><span class="sxs-lookup"><span data-stu-id="2eb20-143">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="2eb20-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="2eb20-144">Response</span></span>
<span data-ttu-id="2eb20-145">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2eb20-145">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2eb20-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2eb20-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="2eb20-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2eb20-147">Request</span></span>
<span data-ttu-id="2eb20-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2eb20-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2eb20-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="2eb20-149">Response</span></span>
<span data-ttu-id="2eb20-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2eb20-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




