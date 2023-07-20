# Google Tag Manager tag template for chatbot.com bot widgets

An unofficial template for Chatbot.com widgets to be added in Google Tag Manager with just a single Chatbot ID field required.

This tag template uses the Google Tag Manager template sandbox JavaScript API within to perform the same function as the vanilla JavaScript widget embed provided by chatbot.com without needing to use Custom HTML.

**Default JavaScript embed widget code**

```html
<!-- Start of ChatBot (www.chatbot.com) code -->
<script type="text/javascript">
    window.__be = window.__be || {};
    window.__be.id = "<YOUR BOT ID>";
    (function() {
        var be = document.createElement('script'); be.type = 'text/javascript'; be.async = true;
        be.src = ('https:' == document.location.protocol ? 'https://' : 'http://') + 'cdn.chatbot.com/widget/plugin.js';
        var s = document.getElementsByTagName('script')[0]; s.parentNode.insertBefore(be, s);
    })();
</script>
<!-- End of ChatBot code -->
```

**Google Tag Manager template**

![image](https://github.com/nottinghamcollege/chatbot-widget-gtm-template/assets/8067792/3bcf6c96-4dfd-4bf0-b13b-4dd479ff962b)

A valid bot ID is required for the tag to function.

The tag template injects the `https://cdn.chatbot.com/widget/plugin.js` script and handles the `__be` window variable.

