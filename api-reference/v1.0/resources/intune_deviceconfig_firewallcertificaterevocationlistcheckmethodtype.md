# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="fc73b-101">firewallCertificateRevocationListCheckMethodType Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="fc73b-101">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="fc73b-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fc73b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc73b-103">Mögliche Werte für firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="fc73b-103">Possible values for firewallCertificateRevocationListCheckMethod</span></span>
## <a name="members"></a><span data-ttu-id="fc73b-104">Elemente</span><span class="sxs-lookup"><span data-stu-id="fc73b-104">Members</span></span>
|<span data-ttu-id="fc73b-105">Element</span><span class="sxs-lookup"><span data-stu-id="fc73b-105">Member</span></span>|<span data-ttu-id="fc73b-106">Wert</span><span class="sxs-lookup"><span data-stu-id="fc73b-106">Value</span></span>|<span data-ttu-id="fc73b-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc73b-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc73b-108">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="fc73b-108">deviceDefault</span></span>|<span data-ttu-id="fc73b-109">0</span><span class="sxs-lookup"><span data-stu-id="fc73b-109">0%</span></span>|<span data-ttu-id="fc73b-110">Von Intune wurde kein Wert konfiguriert, den vom Benutzer konfigurierten Standartwerd für das Gerät nicht außer Kraft setzen</span><span class="sxs-lookup"><span data-stu-id="fc73b-110">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="fc73b-111">keine</span><span class="sxs-lookup"><span data-stu-id="fc73b-111">none</span></span>|<span data-ttu-id="fc73b-112">1</span><span class="sxs-lookup"><span data-stu-id="fc73b-112">-1</span></span>|<span data-ttu-id="fc73b-113">Zertifikatsperrliste nicht prüfen</span><span class="sxs-lookup"><span data-stu-id="fc73b-113">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="fc73b-114">Versuch</span><span class="sxs-lookup"><span data-stu-id="fc73b-114">attempt</span></span>|<span data-ttu-id="fc73b-115">2</span><span class="sxs-lookup"><span data-stu-id="fc73b-115">-2</span></span>|<span data-ttu-id="fc73b-116">CRL-Überprüfung versuchen und Zertifikat nur zulassen, wenn das Zertifikat von der Überprüfung bestätigt wird</span><span class="sxs-lookup"><span data-stu-id="fc73b-116">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="fc73b-117">erfordert</span><span class="sxs-lookup"><span data-stu-id="fc73b-117">Require</span></span>|<span data-ttu-id="fc73b-118">3</span><span class="sxs-lookup"><span data-stu-id="fc73b-118">-3</span></span>|<span data-ttu-id="fc73b-119">Erfolgreiche CRL-Überprüfung anfordern, bevor ein Zertifikat zugelassen wird</span><span class="sxs-lookup"><span data-stu-id="fc73b-119">Require a successful CRL check before allowing a certificate</span></span>|








