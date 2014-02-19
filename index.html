<!DOCTYPE HTML>
<html manifest="" lang="en-US">
<head>
    <meta charset="UTF-8">
	<meta name="apple-mobile-web-app-capable" content="yes">
	<meta name="apple-mobile-web-app-status-bar-style" content="black">
	<meta name="apple-mobile-web-app-title" content="Park and Go London">
	<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0, user-scalable=no, minimal-ui">
    <title>ParkAndGo</title>
    <style type="text/css">
         /**
         * Example of an initial loading indicator.
         * It is recommended to keep this as minimal as possible to provide instant feedback
         * while other resources are still being loaded for the first time
         */
        html, body {
            height: 100%;
            background-color: #1985D0
        }

    </style>
		
    <!-- The line below must be kept intact for Sencha Command to build your application -->
    <script type="text/javascript" src="https://maps.googleapis.com/maps/api/js?key=AIzaSyA-YiurRX6GixuExPSrQgbcOwcUWinAn54&sensor=true&libraries=geometry,places"></script>
	<script src="http://www.mapquestapi.com/sdk/js/v7.0.s/mqa.toolkit.js?key=Fmjtd%7Cluur21utnq%2Cbg%3Do5-90tggy"></script>

    <script type="text/javascript">/**
 * Sencha Blink - Testing
 * @author Jacky Nguyen <jacky@sencha.com>
 */
(function(global) {
    var head = global.document.head,
        Ext = global.Ext;

    if (typeof Ext == 'undefined') {
        global.Ext = Ext = {};
    }

    function write(content) {
        document.write(content);
    }

    function addMeta(name, content) {
        var meta = document.createElement('meta');

        meta.setAttribute('name', name);
        meta.setAttribute('content', content);
        head.appendChild(meta);
    }

    Ext.blink = function(options) {
        var scripts = options.js || [],
            styleSheets = options.css || [],
            i, ln, path, platform, theme;

        if (navigator.userAgent.match(/IEMobile\/10\.0/)) {
            var msViewportStyle = document.createElement("style");
            msViewportStyle.appendChild(
                document.createTextNode(
                    "@media screen and (orientation: portrait) {" +
                        "@-ms-viewport {width: 320px !important;}" +
                    "}" +
                    "@media screen and (orientation: landscape) {" +
                        "@-ms-viewport {width: 560px !important;}" +
                    "}"
                )
            );
            document.getElementsByTagName("head")[0].appendChild(msViewportStyle);
        }
        addMeta('viewport', 'width=device-width, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0, user-scalable=no');
        addMeta('apple-mobile-web-app-capable', 'yes');
        addMeta('apple-touch-fullscreen', 'yes');

        Ext.microloaded = true;

        var filterPlatform = window.Ext.filterPlatform = function(platform) {
            var profileMatch = false,
                ua = navigator.userAgent,
                j, jln, exclude;

            platform = [].concat(platform);

            function isPhone(ua) {
                var isMobile = /Mobile(\/|\s)/.test(ua);

                // Either:
                // - iOS but not iPad
                // - Android 2
                // - Android with "Mobile" in the UA

                return /(iPhone|iPod)/.test(ua) ||
                          (!/(Silk)/.test(ua) && (/(Android)/.test(ua) && (/(Android 2)/.test(ua) || isMobile))) ||
                          (/(BlackBerry|BB)/.test(ua) && isMobile) ||
                          /(Windows Phone)/.test(ua);
            }

            function isTablet(ua) {
                return !isPhone(ua) && (/iPad/.test(ua) || /Android|Silk/.test(ua) || /(RIM Tablet OS)/.test(ua) ||
                    (/MSIE 10/.test(ua) && /; Touch/.test(ua)));
            }

            // Check if the ?platform parameter is set in the URL
            var paramsString = window.location.search.substr(1),
                paramsArray = paramsString.split("&"),
                params = {},
                testPlatform, i;

            for (i = 0; i < paramsArray.length; i++) {
                var tmpArray = paramsArray[i].split("=");
                params[tmpArray[0]] = tmpArray[1];
            }

            testPlatform = params.platform;
            if (testPlatform) {
                return platform.indexOf(testPlatform) != -1;
            }

            for (j = 0, jln = platform.length; j < jln; j++) {
                switch (platform[j]) {
                    case 'phone':
                        profileMatch = isPhone(ua);
                        break;
                    case 'tablet':
                        profileMatch = isTablet(ua);
                        break;
                    case 'desktop':
                        profileMatch = !isPhone(ua) && !isTablet(ua);
                        break;
                    case 'ios':
                        profileMatch = /(iPad|iPhone|iPod)/.test(ua);
                        break;
                    case 'android':
                        profileMatch = /(Android|Silk)/.test(ua);
                        break;
                    case 'blackberry':
                        profileMatch = /(BlackBerry|BB)/.test(ua);
                        break;
                    case 'safari':
                        profileMatch = /Safari/.test(ua) && !(/(BlackBerry|BB)/.test(ua));
                        break;
                    case 'chrome':
                        profileMatch = /Chrome/.test(ua);
                        break;
                    case 'ie10':
                        profileMatch = /MSIE 10/.test(ua);
                        break;
                    case 'windows':
                        profileMatch = /MSIE 10/.test(ua) || /Trident/.test(ua);
                        break;
                    case 'tizen':
                        profileMatch = /Tizen/.test(ua);
                        break;
                    case 'firefox':
                        profileMatch = /Firefox/.test(ua);
                }
                if (profileMatch) {
                    return true;
                }
            }
            return false;
        };

        for (i = 0,ln = styleSheets.length; i < ln; i++) {
            path = styleSheets[i];

            if (typeof path != 'string') {
                platform = path.platform;
                exclude = path.exclude;
                theme = path.theme;
                path = path.path;
            }

            if (platform) {
                if (!filterPlatform(platform) || filterPlatform(exclude)) {
                    continue;
                }
                Ext.theme = {
                    name: theme || 'Default'
                };
            }
            write('<link rel="stylesheet" href="'+path+'">');
        }

        for (i = 0,ln = scripts.length; i < ln; i++) {
            path = scripts[i];

            if (typeof path != 'string') {
                platform = path.platform;
                exclude = path.exclude;
                path = path.path;
            }

            if (platform) {
                if (!filterPlatform(platform) || filterPlatform(exclude)) {
                    continue;
                }
            }

            write('<script src="'+path+'"></'+'script>');
        }
    }

})(this);Ext.blink({"id":"ad99aca1-a58b-450f-a89b-bff51cde7a6d","js":[{"path":"app.js","update":"delta"},{"path":"resources/js/underscore.js","update":"delta"},{"path":"resources/js/globals.js","update":"delta"}],"css":[{"path":"touch/resources/css/cupertino.css","update":"delta","platform":["ios"],"exclude":["android","firefox","chrome"]},{"path":"touch/resources/css/mountainview.css","update":"delta","platform":["andriod","chrome"]},{"path":"touch/resources/css/mountain-view-light.css","update":"delta","platform":["android","firefox","chrome"],"exclude":["ios"]},{"path":"resources/css/main.css","update":"delta"}]});</script>
</head>
<body>
    <div id="appLoadingIndicator">
        <div></div>
        <div></div>
        <div></div>
    </div>
</body>
</html>
