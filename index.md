<html>
    Helloooooo
    <head>
        <title>Test</title>
        <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
        <script type="text/javascript">
        console.error("-----------------------Hello world! from TEL !!!!!!!!!!! ******");
        
        
        try {
            navigatorObject = window.navigator
            var appName = navigatorObject.appName;
            console.error("******************* Application name : ",appName);
            /*console.error("******************* Application name : ",navigator.appName);
            console.error("******************* appCodeName : ",navigator.appCodeName); 
            console.error("*******************appVersion : ",navigator.appVersion);
            console.error("*******************cookieEnabled : ",navigator.cookieEnabled);
            console.error("******************* geolocation : ",navigator.geolocation);
            console.error("*******************language : ",navigator.language);
            console.error("*******************onLine : ",navigator.onLine);
            console.error("*******************platform : ",navigator.platform);
            console.error("*******************product : ",navigator.product);
            console.error("*******************userAgent : ",navigator.userAgent);
            console.error("*******************javaEnabled() : ",navigator.javaEnabled()); */
            //console.error("*******************taintEnabled() : ",navigator.taintEnabled());
            
            const constraints = {
                audio: true,
                //video: true
            };
            navigator.mediaDevices.getUserMedia(constraints).then(handleSuccess).catch(handleError);
           
        }
        catch {
            console.error("++++++++++++++++++++++++ navigator.mediaDevices.getUserMedia is not supported;");
        }
        
        function handleSuccess() {
            console.error('navigator.MediaDevices.getUserMedia success ');
        }
        
        function handleError(error) {
            console.error('navigator.MediaDevices.getUserMedia error: ', error.message, error.name);
        }
        
        try {
             const constraints = {
                audio: true,
                //video: true
             };
             navigator.getUserMedia(constraints).then(handleSuccess1).catch(handleError1);
        }
        
        catch {
            console.error("-------------------------------- navigator.getUserMedia is not supported;");
        }
                 
        function handleSuccess1() {
            console.error(' handleSuccess1 - navigator.MediaDevices.getUserMedia success ');
        }
        
        function handleError1(error) {
            console.error('handleError1 - navigator.MediaDevices.getUserMedia error: ', error.message, error.name);
        }
        </script>
    </head>
    <body>
    
    </body>
</html>
