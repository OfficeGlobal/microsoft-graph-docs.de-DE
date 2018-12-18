---
title: deviceAndAppManagementRoleDefinition erstellen
description: Erstellen eines neuen deviceAndAppManagementRoleDefinition-Objekts.
author: tfitzmac
ms.openlocfilehash: ad338b53aa49d140e36754d36a92f1eda4a6000a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348517"
---
# <a name="create-deviceandappmanagementroledefinition"></a><span data-ttu-id="fb803-103">deviceAndAppManagementRoleDefinition erstellen</span><span class="sxs-lookup"><span data-stu-id="fb803-103">Create deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="fb803-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fb803-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb803-105">Erstellen eines neuen [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="fb803-105">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fb803-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fb803-106">Prerequisites</span></span>
<span data-ttu-id="fb803-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb803-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb803-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fb803-109">Permission type</span></span>|<span data-ttu-id="fb803-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fb803-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb803-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fb803-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fb803-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb803-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="fb803-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fb803-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb803-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fb803-114">Not supported.</span></span>|
|<span data-ttu-id="fb803-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fb803-115">Application</span></span>|<span data-ttu-id="fb803-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fb803-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb803-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fb803-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="fb803-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fb803-118">Request headers</span></span>
|<span data-ttu-id="fb803-119">Header</span><span class="sxs-lookup"><span data-stu-id="fb803-119">Header</span></span>|<span data-ttu-id="fb803-120">Wert</span><span class="sxs-lookup"><span data-stu-id="fb803-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb803-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="fb803-121">Authorization</span></span>|<span data-ttu-id="fb803-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fb803-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb803-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fb803-123">Accept</span></span>|<span data-ttu-id="fb803-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fb803-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb803-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fb803-125">Request body</span></span>
<span data-ttu-id="fb803-126">Geben Sie im Anforderungstext eine JSON-Darstellung des deviceAndAppManagementRoleDefinition-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="fb803-126">In the request body, supply a JSON representation for the deviceAndAppManagementRoleDefinition object.</span></span>

<span data-ttu-id="fb803-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceAndAppManagementRoleDefinition erstellen.</span><span class="sxs-lookup"><span data-stu-id="fb803-127">The following table shows the properties that are required when you create the deviceAndAppManagementRoleDefinition.</span></span>

|<span data-ttu-id="fb803-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fb803-128">Property</span></span>|<span data-ttu-id="fb803-129">Typ</span><span class="sxs-lookup"><span data-stu-id="fb803-129">Type</span></span>|<span data-ttu-id="fb803-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fb803-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb803-131">id</span><span class="sxs-lookup"><span data-stu-id="fb803-131">id</span></span>|<span data-ttu-id="fb803-132">String</span><span class="sxs-lookup"><span data-stu-id="fb803-132">String</span></span>|<span data-ttu-id="fb803-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="fb803-133">Key of the entity.</span></span> <span data-ttu-id="fb803-134">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="fb803-134">This is read-only and automatically generated.</span></span> <span data-ttu-id="fb803-135">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="fb803-135">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="fb803-136">displayName</span><span class="sxs-lookup"><span data-stu-id="fb803-136">displayName</span></span>|<span data-ttu-id="fb803-137">String</span><span class="sxs-lookup"><span data-stu-id="fb803-137">String</span></span>|<span data-ttu-id="fb803-138">Anzeigename der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="fb803-138">Display Name of the Role definition.</span></span> <span data-ttu-id="fb803-139">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="fb803-139">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="fb803-140">description</span><span class="sxs-lookup"><span data-stu-id="fb803-140">description</span></span>|<span data-ttu-id="fb803-141">String</span><span class="sxs-lookup"><span data-stu-id="fb803-141">String</span></span>|<span data-ttu-id="fb803-142">Beschreibung der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="fb803-142">Description of the Role definition.</span></span> <span data-ttu-id="fb803-143">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="fb803-143">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="fb803-144">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="fb803-144">rolePermissions</span></span>|<span data-ttu-id="fb803-145">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="fb803-145">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="fb803-146">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="fb803-146">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="fb803-147">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="fb803-147">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="fb803-148">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="fb803-148">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="fb803-149">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="fb803-149">isBuiltIn</span></span>|<span data-ttu-id="fb803-150">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="fb803-150">Boolean</span></span>|<span data-ttu-id="fb803-151">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="fb803-151">Type of Role.</span></span> <span data-ttu-id="fb803-152">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="fb803-152">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="fb803-153">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="fb803-153">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="fb803-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="fb803-154">Response</span></span>
<span data-ttu-id="fb803-155">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fb803-155">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb803-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fb803-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="fb803-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fb803-157">Request</span></span>
<span data-ttu-id="fb803-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fb803-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
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

### <a name="response"></a><span data-ttu-id="fb803-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="fb803-159">Response</span></span>
<span data-ttu-id="fb803-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fb803-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



