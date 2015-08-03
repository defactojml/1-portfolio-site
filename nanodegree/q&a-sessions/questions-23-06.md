
# Q & A - Testing on Mobile devices (June 23rd session)

Context: trying to remote debug the portfolio site (only available on localhost) for both iPhone & Samsung devices


### Remote debugging iphone  5 - safari on mac (using safari’s web inspector)
I have been successfull remote debuging a "public" page (for which the url was entered in the iphone). [See this article - ios section](http://www.smashingmagazine.com/2014/09/03/testing-mobile-emulators-simulators-remote-debugging/2/)

![iphone-safari.png]


I have not been able to publish a localhost page to my iphone5 

**Any idea on how to solve the problem in this context?**

### Remote debugging iphone 5 - chrome on mac (using ios-webkit-debug-proxy)
This does not seem to work with my setup :

- macbook pro on yosemite
- iphone 5 on iOS 8.3

Once i type the following 

			ios_webkit_debug_proxy




I get 

		
		Listing devices on :9221

Then 

        Connected :9222 to iPhone de jean-michel 
        Invalid message _rpc_applicationUpdated: <dict>
	    <key>WIRApplicationBundleIdentifierKey</key>
	    <string>com.apple.mobilesafari</string>
	    <key>WIRApplicationNameKey</key>
	    <string>Safari</string>
	    <key>WIRIsApplicationProxyKey</key>
	    <false/>
	    <key>WIRIsApplicationActiveKey</key>
	    <integer>1</integer>
	    <key>WIRApplicationIdentifierKey</key>
	    <string>PID:322</string>
        </dict>
        
        Disconnected :9222 from iPhone de jean-michel (077a4e140286fcf4b6ca31a0bb7d3ef1c5c89185)

 
 This looks similar to the issue raised to this [post] (https://github.com/google/ios-webkit-debug-proxy/issues/72)
    
    
**Any idea on how to solve the problem in this context?**



## Remote debugging samsung s5 - chrome on mac
I have been successfull remote debuging a localhost page on port 8080 (hosted on apache)
[Ref] (https://developer.chrome.com/devtools/docs/remote-debugging)

I have **not** been successfull remote debuging a localhost page on port 63342 (default port used by webstorm) 

**Any idea on how to solve the problem in this context?**

susan-coach@udacity.com