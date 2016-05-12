# MagTek uDynamo Card Reader Plugin #

Allow using the MagTek uDynamo Card Reader with https://build.phonegap.com

Minimal working config.xml:

 ```
<?xml version='1.0' encoding='utf-8'?>
<widget id="de.beon-support.emat" version="1.0" xmlns="http://www.w3.org/ns/widgets" xmlns:gap="http://phonegap.com/ns/1.0" xmlns:android="http://schemas.android.com/apk/res/android">
    ...
    <plugin name="cordova-plugin-media" spec="2.3.0" />
    <plugin spec="https://github.com/fsalomon/CardReaderPlugin.git" />
    <preference name="phonegap-version" value="cli-6.1.0" />
    ...
    <platform name="android">
        <allow-intent href="market:*" />
    </platform>
    <platform name="ios">
        <preference name="deployment-target" value="7.0" />
        <allow-intent href="itms:*" />
        <allow-intent href="itms-apps:*" />
    </platform>
</widget>
 ```
