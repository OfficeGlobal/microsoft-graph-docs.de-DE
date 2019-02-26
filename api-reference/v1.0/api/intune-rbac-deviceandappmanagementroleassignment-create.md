---
title: DeviceAndAppManagementRoleAssignment erstellen
description: Erstellen eines neuen deviceAndAppManagementRoleAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c83c8521fc4c72b2dd0e96a607efa0f1bb9de8a0
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255647"
---
# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="b2b67-103">DeviceAndAppManagementRoleAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="b2b67-103">Create deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="b2b67-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b2b67-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2b67-105">Erstellen eines neuen [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b2b67-105">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2b67-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b2b67-106">Prerequisites</span></span>
<span data-ttu-id="b2b67-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b2b67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b2b67-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b2b67-109">Permission type</span></span>|<span data-ttu-id="b2b67-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b2b67-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2b67-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b2b67-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b2b67-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2b67-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="b2b67-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b2b67-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2b67-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b2b67-114">Not supported.</span></span>|
|<span data-ttu-id="b2b67-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b2b67-115">Application</span></span>|<span data-ttu-id="b2b67-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b2b67-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2b67-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b2b67-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="b2b67-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b2b67-118">Request headers</span></span>
|<span data-ttu-id="b2b67-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b2b67-119">Header</span></span>|<span data-ttu-id="b2b67-120">Wert</span><span class="sxs-lookup"><span data-stu-id="b2b67-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2b67-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2b67-121">Authorization</span></span>|<span data-ttu-id="b2b67-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b2b67-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2b67-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b2b67-123">Accept</span></span>|<span data-ttu-id="b2b67-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b2b67-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2b67-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b2b67-125">Request body</span></span>
<span data-ttu-id="b2b67-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs deviceAndAppManagementRoleAssignment an.</span><span class="sxs-lookup"><span data-stu-id="b2b67-126">In the request body, supply a JSON representation for the deviceAndAppManagementRoleAssignment object.</span></span>

<span data-ttu-id="b2b67-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceAndAppManagementRoleAssignment erstellen.</span><span class="sxs-lookup"><span data-stu-id="b2b67-127">The following table shows the properties that are required when you create the deviceAndAppManagementRoleAssignment.</span></span>

|<span data-ttu-id="b2b67-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b2b67-128">Property</span></span>|<span data-ttu-id="b2b67-129">Typ</span><span class="sxs-lookup"><span data-stu-id="b2b67-129">Type</span></span>|<span data-ttu-id="b2b67-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b2b67-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2b67-131">id</span><span class="sxs-lookup"><span data-stu-id="b2b67-131">id</span></span>|<span data-ttu-id="b2b67-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b2b67-132">String</span></span>|<span data-ttu-id="b2b67-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b2b67-133">Key of the entity.</span></span> <span data-ttu-id="b2b67-134">Dies ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="b2b67-134">This is read-only and automatically generated.</span></span> <span data-ttu-id="b2b67-135">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b2b67-135">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="b2b67-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b2b67-136">displayName</span></span>|<span data-ttu-id="b2b67-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b2b67-137">String</span></span>|<span data-ttu-id="b2b67-138">Der Anzeigename der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="b2b67-138">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="b2b67-139">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b2b67-139">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="b2b67-140">description</span><span class="sxs-lookup"><span data-stu-id="b2b67-140">description</span></span>|<span data-ttu-id="b2b67-141">String</span><span class="sxs-lookup"><span data-stu-id="b2b67-141">String</span></span>|<span data-ttu-id="b2b67-142">Beschreibung der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="b2b67-142">Description of the Role Assignment.</span></span> <span data-ttu-id="b2b67-143">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b2b67-143">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="b2b67-144">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="b2b67-144">resourceScopes</span></span>|<span data-ttu-id="b2b67-145">String collection</span><span class="sxs-lookup"><span data-stu-id="b2b67-145">String collection</span></span>|<span data-ttu-id="b2b67-146">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="b2b67-146">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="b2b67-147">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b2b67-147">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="b2b67-148">Geerbt von [RoleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b2b67-148">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="b2b67-149">members</span><span class="sxs-lookup"><span data-stu-id="b2b67-149">members</span></span>|<span data-ttu-id="b2b67-150">String collection</span><span class="sxs-lookup"><span data-stu-id="b2b67-150">String collection</span></span>|<span data-ttu-id="b2b67-151">Die Liste der IDs der Rollenmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="b2b67-151">The list of ids of role member security groups.</span></span> <span data-ttu-id="b2b67-152">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b2b67-152">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="b2b67-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="b2b67-153">Response</span></span>
<span data-ttu-id="b2b67-154">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b2b67-154">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2b67-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b2b67-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2b67-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b2b67-156">Request</span></span>
<span data-ttu-id="b2b67-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b2b67-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments
Content-type: application/json
Content-length: 258

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="b2b67-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="b2b67-158">Response</span></span>
<span data-ttu-id="b2b67-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b2b67-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 307

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```



