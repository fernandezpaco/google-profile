# cordova-google-signin
Polymer component for getting user profile info from google

```html
 <cordova-google-signin 
    id="cordovasignin" 
    client_id="your-client-id"
    client_secret= "your-secret-key">
  </cordova-google-signin>

  <google-profile token="{{tok}}" userinfo="{{userinfo}}"></google-profile>

  <img src="{{userinfo.picture}}"></img>

  <script type="text/javascript">
	document.addEventListener("deviceready", onDeviceReady, false);
	function onDeviceReady() {	    
	    window.open = cordova.InAppBrowser.open;
	    document.querySelector("#cordovasignin").signIn();
	}
  </script>
```