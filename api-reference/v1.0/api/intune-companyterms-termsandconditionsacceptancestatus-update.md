---
title: Aktualisieren von „termsAndConditionsAcceptanceStatus“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs termsAndConditionsAcceptanceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 224c582425261aab53525c1ebe30cb9f2e889167
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252210"
---
# <a name="update-termsandconditionsacceptancestatus"></a><span data-ttu-id="2f987-103">Aktualisieren von „termsAndConditionsAcceptanceStatus“</span><span class="sxs-lookup"><span data-stu-id="2f987-103">Update termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="2f987-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2f987-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f987-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="2f987-105">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f987-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2f987-106">Prerequisites</span></span>
<span data-ttu-id="2f987-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2f987-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2f987-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2f987-109">Permission type</span></span>|<span data-ttu-id="2f987-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2f987-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f987-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2f987-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2f987-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f987-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2f987-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2f987-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f987-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f987-114">Not supported.</span></span>|
|<span data-ttu-id="2f987-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2f987-115">Application</span></span>|<span data-ttu-id="2f987-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2f987-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f987-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f987-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="2f987-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2f987-118">Request headers</span></span>
|<span data-ttu-id="2f987-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2f987-119">Header</span></span>|<span data-ttu-id="2f987-120">Wert</span><span class="sxs-lookup"><span data-stu-id="2f987-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f987-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f987-121">Authorization</span></span>|<span data-ttu-id="2f987-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2f987-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f987-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2f987-123">Accept</span></span>|<span data-ttu-id="2f987-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2f987-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f987-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2f987-125">Request body</span></span>
<span data-ttu-id="2f987-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) an.</span><span class="sxs-lookup"><span data-stu-id="2f987-126">In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

<span data-ttu-id="2f987-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="2f987-127">The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>

|<span data-ttu-id="2f987-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2f987-128">Property</span></span>|<span data-ttu-id="2f987-129">Typ</span><span class="sxs-lookup"><span data-stu-id="2f987-129">Type</span></span>|<span data-ttu-id="2f987-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2f987-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f987-131">id</span><span class="sxs-lookup"><span data-stu-id="2f987-131">id</span></span>|<span data-ttu-id="2f987-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2f987-132">String</span></span>|<span data-ttu-id="2f987-133">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="2f987-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="2f987-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="2f987-134">userDisplayName</span></span>|<span data-ttu-id="2f987-135">String</span><span class="sxs-lookup"><span data-stu-id="2f987-135">String</span></span>|<span data-ttu-id="2f987-136">Anzeigename des Benutzers, dessen Zustimmung die Entität darstellt</span><span class="sxs-lookup"><span data-stu-id="2f987-136">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="2f987-137">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="2f987-137">acceptedVersion</span></span>|<span data-ttu-id="2f987-138">Int32</span><span class="sxs-lookup"><span data-stu-id="2f987-138">Int32</span></span>|<span data-ttu-id="2f987-139">Die Versionsnummer der neuesten Version der Geschäftsbedingungen, die der Benutzer akzeptiert hat</span><span class="sxs-lookup"><span data-stu-id="2f987-139">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="2f987-140">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f987-140">acceptedDateTime</span></span>|<span data-ttu-id="2f987-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f987-141">DateTimeOffset</span></span>|<span data-ttu-id="2f987-142">Datum und Uhrzeit der letzten Zustimmung zu den Bedingungen durch den Benutzer</span><span class="sxs-lookup"><span data-stu-id="2f987-142">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="2f987-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f987-143">Response</span></span>
<span data-ttu-id="2f987-144">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2f987-144">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f987-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f987-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f987-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f987-146">Request</span></span>
<span data-ttu-id="2f987-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2f987-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="2f987-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f987-148">Response</span></span>
<span data-ttu-id="2f987-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2f987-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



