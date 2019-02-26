---
title: eBookInstallSummary aktualisieren
description: Aktualisieren der Eigenschaften des eBookInstallSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3dc5b97046c0075af20623935d25b4fbba1d9765
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162895"
---
# <a name="update-ebookinstallsummary"></a><span data-ttu-id="62df7-103">eBookInstallSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="62df7-103">Update eBookInstallSummary</span></span>

> <span data-ttu-id="62df7-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="62df7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62df7-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="62df7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62df7-106">Aktualisieren der Eigenschaften des [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="62df7-106">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62df7-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="62df7-107">Prerequisites</span></span>
<span data-ttu-id="62df7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="62df7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="62df7-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="62df7-110">Permission type</span></span>|<span data-ttu-id="62df7-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="62df7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62df7-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="62df7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="62df7-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62df7-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="62df7-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="62df7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62df7-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="62df7-115">Not supported.</span></span>|
|<span data-ttu-id="62df7-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="62df7-116">Application</span></span>|<span data-ttu-id="62df7-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="62df7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62df7-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="62df7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="62df7-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="62df7-119">Request headers</span></span>
|<span data-ttu-id="62df7-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="62df7-120">Header</span></span>|<span data-ttu-id="62df7-121">Wert</span><span class="sxs-lookup"><span data-stu-id="62df7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62df7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="62df7-122">Authorization</span></span>|<span data-ttu-id="62df7-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="62df7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62df7-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="62df7-124">Accept</span></span>|<span data-ttu-id="62df7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="62df7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62df7-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="62df7-126">Request body</span></span>
<span data-ttu-id="62df7-127">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="62df7-127">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="62df7-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="62df7-128">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span></span>

|<span data-ttu-id="62df7-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="62df7-129">Property</span></span>|<span data-ttu-id="62df7-130">Typ</span><span class="sxs-lookup"><span data-stu-id="62df7-130">Type</span></span>|<span data-ttu-id="62df7-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="62df7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62df7-132">id</span><span class="sxs-lookup"><span data-stu-id="62df7-132">id</span></span>|<span data-ttu-id="62df7-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="62df7-133">String</span></span>|<span data-ttu-id="62df7-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="62df7-134">Key of the entity.</span></span>|
|<span data-ttu-id="62df7-135">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="62df7-135">installedDeviceCount</span></span>|<span data-ttu-id="62df7-136">Int32</span><span class="sxs-lookup"><span data-stu-id="62df7-136">Int32</span></span>|<span data-ttu-id="62df7-137">Die Anzahl der Geräte, auf denen das Buch erfolgreich installiert wurde.</span><span class="sxs-lookup"><span data-stu-id="62df7-137">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="62df7-138">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="62df7-138">failedDeviceCount</span></span>|<span data-ttu-id="62df7-139">Int32</span><span class="sxs-lookup"><span data-stu-id="62df7-139">Int32</span></span>|<span data-ttu-id="62df7-140">Die Anzahl der Geräte, auf denen die Installation des Buchs fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="62df7-140">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="62df7-141">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="62df7-141">notInstalledDeviceCount</span></span>|<span data-ttu-id="62df7-142">Int32</span><span class="sxs-lookup"><span data-stu-id="62df7-142">Int32</span></span>|<span data-ttu-id="62df7-143">Die Anzahl von Geräten, auf denen das Buch nicht installiert ist.</span><span class="sxs-lookup"><span data-stu-id="62df7-143">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="62df7-144">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="62df7-144">installedUserCount</span></span>|<span data-ttu-id="62df7-145">Int32</span><span class="sxs-lookup"><span data-stu-id="62df7-145">Int32</span></span>|<span data-ttu-id="62df7-146">Die Anzahl der Benutzer, deren Geräte das Buch erfolgreich installiert haben.</span><span class="sxs-lookup"><span data-stu-id="62df7-146">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="62df7-147">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="62df7-147">failedUserCount</span></span>|<span data-ttu-id="62df7-148">Int32</span><span class="sxs-lookup"><span data-stu-id="62df7-148">Int32</span></span>|<span data-ttu-id="62df7-149">Die Anzahl der Benutzer, die mindestens ein Gerät besitzen, auf dem die Installation des Buchs fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="62df7-149">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="62df7-150">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="62df7-150">notInstalledUserCount</span></span>|<span data-ttu-id="62df7-151">Int32</span><span class="sxs-lookup"><span data-stu-id="62df7-151">Int32</span></span>|<span data-ttu-id="62df7-152">Die Anzahl der Benutzer, die das Buch nicht installiert haben.</span><span class="sxs-lookup"><span data-stu-id="62df7-152">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="62df7-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="62df7-153">Response</span></span>
<span data-ttu-id="62df7-154">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="62df7-154">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62df7-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="62df7-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="62df7-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="62df7-156">Request</span></span>
<span data-ttu-id="62df7-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="62df7-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
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

### <a name="response"></a><span data-ttu-id="62df7-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="62df7-158">Response</span></span>
<span data-ttu-id="62df7-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="62df7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




