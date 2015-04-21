# Unity-Android-Ads-Plugin
Unity Android Ads Plugin Currently supports Admob, Charboost, Heyzap and Leadbolt ads.
Ads Supported  are:
* Admob Banner
* Admob Interstitial
* Leadbolt Interstitial
* Chartboost Interstitial
* Heyzap Interstitial
* AdBuddiz Interstitial

# Steps to integerate
1. Import the provided unity package to your unity3d project.
2. Get an object of 'AdsManager' class.
3. Assign the Ad IDs
4. Call 'Initialize()' method on 'AdsManager'.
5. Show the ads.

# Code sample for initialization
		AdsManager manager = AdsManager.SharedObject();
		manager.admobBannerID = "";
		manager.showBannerAtTop = false;
		manager.admobIntertitialID = "";
		manager.ChartboostAppID = "";
		manager.ChartboostAppSignature = "";
		manager.LeadboltInterstitialID = "";
		manager.HeyzapPublisherID = "";
		manager.AdBuddizPublisherKey = "";
		manager.Initialize();
		
# Code sample for showing ads
		AdsManager manager = AdsManager.SharedObject();
		manager.ShowBanner ();
		manager.ShowChartboostInterstitial ();
		
# Public Methods
		ShowBanner()			// Show Admob Banner
		HideBanner()			// Hide Admob Banner
		ShowAdmobInterstitial()		// Show Admob Interstitial
		HideAdmobInterstitial()		// Prevent Admob Interstitial from showing if its not already shown
		ShowChartboostInterstitial()	// Show Chartboost Interstitial
		HideChartboostInterstitial()	// Prevent Chartboost Interstitial from showing if its not already shown
		ShowHeyzapInterstitial()	// Show Heyzap Interstitial
		HideHeyzapInterstitial()	// Prevent Heyzap Interstitial from showing if its not already shown
		ShowLeadboltInterstitial()	// Show Leadbolt Interstitial
		HideLeadboltInterstitial()	// Prevent Leadbolt Interstitial from showing if its not already shown
		ShowAdBuddizInterstitial()	// Show AdBuddiz Interstitial
		HideAdBuddizInterstitial()	// Prevent AdBuddiz Interstitial from showing if its not already shown
		ShowAutoAd()			// Show Random Ads

# Public Properties
		testMode		// Enable/Disable Test/Logger mode
		admobBannerID		// Admob Banner ID
		admobIntertitialID	// Admob Interstitial ID
		ChartboostAppID		// Chartboost AppID
		ChartboostAppSignature	// Chartboost App Signature
		LeadboltInterstitialID	// Leadbolt Interstitial ID
		HeyzapPublisherID	// Heyzap Publisher ID
		AdBuddizPublisherKey	// AdBuddiz Publisher ID
		showBannerAtTop		// Whether to show banner at top or bottom
