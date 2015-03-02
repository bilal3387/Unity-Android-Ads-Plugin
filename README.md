# Unity-Android-Ads-Plugin
Unity Android Ads Plugin Currently support Admob, Charboost, Heyzap and Leadbolt ads.
Ads Supported  are:
* Admob Banner
* Admob Interstitial
* Leadbolt Interstitial
* Chartboost Interstitial
* Heyzap Interstitial

# Steps to integerate
1. Import the provided unity package to your unity3d project.
2. Get an object of 'AdsManager' class.
3. Assign the Ad IDs
4. Call 'Initialize()' method on 'AdsManager' and you are good to go.

# Code sample for initialization
		AdsManager manager = AdsManager.SharedObject();
		manager.admobBannerID = "ca-app-pub-XXXXXXXXXX/XXXXX";
		manager.showBannerAtTop = false;
		manager.admobIntertitialID = "ca-app-pub-XXXXXXXXXXXXX/XXXXXX";
		manager.ChartboostAppID = "XXXXXXXXXXXXXXXXXXXXX";
		manager.ChartboostAppSignature = "XXXXXXXXXXXXXXXX";
		manager.LeadboltInterstitialID = "XXXXXXXXX";
		manager.HeyzapPublisherID = "XXXXXXXXXXXXXXXX";
		manager.Initialize();
		
# Code sample for showing ads
		AdsManager manager = AdsManager.SharedObject();
		manager.ShowBanner ();
		manager.ShowChartboostInterstitial ();
		
# Public Methods
		ShowBanner ()
		HideBanner ();
		ShowAdmobInterstitial ()
		HideAdmobInterstitial ()
		ShowChartboostInterstitial ()
		HideChartboostInterstitial ()
		ShowHeyzapInterstitial ()
		HideHeyzapInterstitial ()
		ShowLeadboltInterstial ()
