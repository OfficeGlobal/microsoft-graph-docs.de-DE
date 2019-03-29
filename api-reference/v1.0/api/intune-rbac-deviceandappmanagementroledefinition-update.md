---
title: deviceAndAppManagementRoleDefinition aktualisieren
description: Aktualisieren der Eigenschaften eines deviceAndAppManagementRoleDefinition-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dfcc2f315f528588739a780ea7f70b0207cab67d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30961798"
---
# <a name="update-deviceandappmanagementroledefinition"></a><span data-ttu-id="25585-103">deviceAndAppManagementRoleDefinition aktualisieren</span><span class="sxs-lookup"><span data-stu-id="25585-103">Update deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="25585-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="25585-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25585-105">Aktualisieren der Eigenschaften eines [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="25585-105">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25585-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="25585-106">Prerequisites</span></span>
<span data-ttu-id="25585-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25585-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25585-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="25585-109">Permission type</span></span>|<span data-ttu-id="25585-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="25585-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25585-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="25585-111">Delegated (work or school account)</span></span>|<span data-ttu-id="25585-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25585-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="25585-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="25585-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25585-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="25585-114">Not supported.</span></span>|
|<span data-ttu-id="25585-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="25585-115">Application</span></span>|<span data-ttu-id="25585-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="25585-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25585-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="25585-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="25585-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="25585-118">Request headers</span></span>
|<span data-ttu-id="25585-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="25585-119">Header</span></span>|<span data-ttu-id="25585-120">Wert</span><span class="sxs-lookup"><span data-stu-id="25585-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25585-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="25585-121">Authorization</span></span>|<span data-ttu-id="25585-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="25585-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25585-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="25585-123">Accept</span></span>|<span data-ttu-id="25585-124">application/json</span><span class="sxs-lookup"><span data-stu-id="25585-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25585-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="25585-125">Request body</span></span>
<span data-ttu-id="25585-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="25585-126">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

<span data-ttu-id="25585-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="25585-127">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>

|<span data-ttu-id="25585-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="25585-128">Property</span></span>|<span data-ttu-id="25585-129">Typ</span><span class="sxs-lookup"><span data-stu-id="25585-129">Type</span></span>|<span data-ttu-id="25585-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="25585-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25585-131">id</span><span class="sxs-lookup"><span data-stu-id="25585-131">id</span></span>|<span data-ttu-id="25585-132">String</span><span class="sxs-lookup"><span data-stu-id="25585-132">String</span></span>|<span data-ttu-id="25585-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="25585-133">Key of the entity.</span></span> <span data-ttu-id="25585-134">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="25585-134">This is read-only and automatically generated.</span></span> <span data-ttu-id="25585-135">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="25585-135">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="25585-136">displayName</span><span class="sxs-lookup"><span data-stu-id="25585-136">displayName</span></span>|<span data-ttu-id="25585-137">String</span><span class="sxs-lookup"><span data-stu-id="25585-137">String</span></span>|<span data-ttu-id="25585-138">Anzeigename der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="25585-138">Display Name of the Role definition.</span></span> <span data-ttu-id="25585-139">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="25585-139">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="25585-140">description</span><span class="sxs-lookup"><span data-stu-id="25585-140">description</span></span>|<span data-ttu-id="25585-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="25585-141">String</span></span>|<span data-ttu-id="25585-142">Beschreibung der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="25585-142">Description of the Role definition.</span></span> <span data-ttu-id="25585-143">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="25585-143">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="25585-144">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="25585-144">rolePermissions</span></span>|<span data-ttu-id="25585-145">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="25585-145">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="25585-146">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="25585-146">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="25585-147">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="25585-147">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="25585-148">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="25585-148">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="25585-149">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="25585-149">isBuiltIn</span></span>|<span data-ttu-id="25585-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="25585-150">Boolean</span></span>|<span data-ttu-id="25585-151">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="25585-151">Type of Role.</span></span> <span data-ttu-id="25585-152">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="25585-152">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="25585-153">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="25585-153">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="25585-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="25585-154">Response</span></span>
<span data-ttu-id="25585-155">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="25585-155">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25585-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="25585-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="25585-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="25585-157">Request</span></span>
<span data-ttu-id="25585-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="25585-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
Content-type: application/json
Content-length: 602

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="25585-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="25585-159">Response</span></span>
<span data-ttu-id="25585-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="25585-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 651

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "id": "bca1dfb5-dfb5-bca1-b5df-a1bcb5dfa1bc",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```



