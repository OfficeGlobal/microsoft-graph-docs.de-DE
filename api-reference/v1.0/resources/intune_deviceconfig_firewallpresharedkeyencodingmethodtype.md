# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="04308-101">FirewallPreSharedKeyEncodingMethodType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="04308-101">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="04308-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="04308-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04308-103">Mögliche Werte für firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="04308-103">Possible values for firewallPreSharedKeyEncodingMethod</span></span>
## <a name="members"></a><span data-ttu-id="04308-104">Elemente</span><span class="sxs-lookup"><span data-stu-id="04308-104">Members</span></span>
|<span data-ttu-id="04308-105">Element</span><span class="sxs-lookup"><span data-stu-id="04308-105">Member</span></span>|<span data-ttu-id="04308-106">Wert</span><span class="sxs-lookup"><span data-stu-id="04308-106">Value</span></span>|<span data-ttu-id="04308-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04308-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04308-108">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="04308-108">deviceDefault</span></span>|<span data-ttu-id="04308-109">0</span><span class="sxs-lookup"><span data-stu-id="04308-109">0%</span></span>|<span data-ttu-id="04308-110">Von Intune wurde kein Wert konfiguriert, den vom Benutzer konfigurierten Standardwert für das Gerät nicht außer Kraft setzen</span><span class="sxs-lookup"><span data-stu-id="04308-110">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="04308-111">keine</span><span class="sxs-lookup"><span data-stu-id="04308-111">none</span></span>|<span data-ttu-id="04308-112">1</span><span class="sxs-lookup"><span data-stu-id="04308-112">-1</span></span>|<span data-ttu-id="04308-113">Vorinstallierter Schlüssel ist nicht codiert.</span><span class="sxs-lookup"><span data-stu-id="04308-113">Preshared key is not encoded.</span></span> <span data-ttu-id="04308-114">Stattdessen wird er in seinem Breitzeichen-Format gespeichert</span><span class="sxs-lookup"><span data-stu-id="04308-114">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="04308-115">utF8</span><span class="sxs-lookup"><span data-stu-id="04308-115">utf-8</span></span>|<span data-ttu-id="04308-116">2</span><span class="sxs-lookup"><span data-stu-id="04308-116">-2</span></span>|<span data-ttu-id="04308-117">Vorinstallierter Schlüssel mit UTF-8-Codierung</span><span class="sxs-lookup"><span data-stu-id="04308-117">Encode the preshared key using UTF-8</span></span>|








