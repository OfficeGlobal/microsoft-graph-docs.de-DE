---
title: eBookInstallSummary aktualisieren
description: Aktualisieren der Eigenschaften des eBookInstallSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ef685cf8ed1f38a762e5063492fdfb0d33e0d220
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251643"
---
# <a name="update-ebookinstallsummary"></a><span data-ttu-id="a41e8-103">eBookInstallSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a41e8-103">Update eBookInstallSummary</span></span>

> <span data-ttu-id="a41e8-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a41e8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a41e8-105">Aktualisieren der Eigenschaften des [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a41e8-105">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a41e8-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a41e8-106">Prerequisites</span></span>
<span data-ttu-id="a41e8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a41e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a41e8-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a41e8-109">Permission type</span></span>|<span data-ttu-id="a41e8-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a41e8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a41e8-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a41e8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a41e8-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a41e8-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a41e8-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a41e8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a41e8-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a41e8-114">Not supported.</span></span>|
|<span data-ttu-id="a41e8-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a41e8-115">Application</span></span>|<span data-ttu-id="a41e8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a41e8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a41e8-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a41e8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="a41e8-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a41e8-118">Request headers</span></span>
|<span data-ttu-id="a41e8-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a41e8-119">Header</span></span>|<span data-ttu-id="a41e8-120">Wert</span><span class="sxs-lookup"><span data-stu-id="a41e8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a41e8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a41e8-121">Authorization</span></span>|<span data-ttu-id="a41e8-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a41e8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a41e8-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a41e8-123">Accept</span></span>|<span data-ttu-id="a41e8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a41e8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a41e8-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a41e8-125">Request body</span></span>
<span data-ttu-id="a41e8-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="a41e8-126">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="a41e8-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="a41e8-127">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span></span>

|<span data-ttu-id="a41e8-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a41e8-128">Property</span></span>|<span data-ttu-id="a41e8-129">Typ</span><span class="sxs-lookup"><span data-stu-id="a41e8-129">Type</span></span>|<span data-ttu-id="a41e8-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a41e8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a41e8-131">id</span><span class="sxs-lookup"><span data-stu-id="a41e8-131">id</span></span>|<span data-ttu-id="a41e8-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a41e8-132">String</span></span>|<span data-ttu-id="a41e8-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a41e8-133">Key of the entity.</span></span>|
|<span data-ttu-id="a41e8-134">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a41e8-134">installedDeviceCount</span></span>|<span data-ttu-id="a41e8-135">Int32</span><span class="sxs-lookup"><span data-stu-id="a41e8-135">Int32</span></span>|<span data-ttu-id="a41e8-136">Die Anzahl der Geräte, auf denen das Buch erfolgreich installiert wurde.</span><span class="sxs-lookup"><span data-stu-id="a41e8-136">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="a41e8-137">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a41e8-137">failedDeviceCount</span></span>|<span data-ttu-id="a41e8-138">Int32</span><span class="sxs-lookup"><span data-stu-id="a41e8-138">Int32</span></span>|<span data-ttu-id="a41e8-139">Die Anzahl der Geräte, auf denen die Installation des Buchs fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="a41e8-139">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="a41e8-140">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a41e8-140">notInstalledDeviceCount</span></span>|<span data-ttu-id="a41e8-141">Int32</span><span class="sxs-lookup"><span data-stu-id="a41e8-141">Int32</span></span>|<span data-ttu-id="a41e8-142">Die Anzahl von Geräten, auf denen das Buch nicht installiert ist.</span><span class="sxs-lookup"><span data-stu-id="a41e8-142">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="a41e8-143">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="a41e8-143">installedUserCount</span></span>|<span data-ttu-id="a41e8-144">Int32</span><span class="sxs-lookup"><span data-stu-id="a41e8-144">Int32</span></span>|<span data-ttu-id="a41e8-145">Die Anzahl der Benutzer, deren Geräte das Buch erfolgreich installiert haben.</span><span class="sxs-lookup"><span data-stu-id="a41e8-145">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="a41e8-146">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="a41e8-146">failedUserCount</span></span>|<span data-ttu-id="a41e8-147">Int32</span><span class="sxs-lookup"><span data-stu-id="a41e8-147">Int32</span></span>|<span data-ttu-id="a41e8-148">Die Anzahl der Benutzer, die mindestens ein Gerät besitzen, auf dem die Installation des Buchs fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="a41e8-148">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="a41e8-149">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="a41e8-149">notInstalledUserCount</span></span>|<span data-ttu-id="a41e8-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a41e8-150">Int32</span></span>|<span data-ttu-id="a41e8-151">Die Anzahl der Benutzer, die das Buch nicht installiert haben.</span><span class="sxs-lookup"><span data-stu-id="a41e8-151">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="a41e8-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="a41e8-152">Response</span></span>
<span data-ttu-id="a41e8-153">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a41e8-153">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a41e8-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a41e8-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="a41e8-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a41e8-155">Request</span></span>
<span data-ttu-id="a41e8-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a41e8-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
Content-type: application/json
Content-length: 236

{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```

### <a name="response"></a><span data-ttu-id="a41e8-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="a41e8-157">Response</span></span>
<span data-ttu-id="a41e8-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a41e8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "9708ad78-ad78-9708-78ad-089778ad0897",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```



