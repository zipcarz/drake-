drake-
======
 Android-SSL-TrustKiller
2		--------
3		-Bypass SSL certificate pinning for most applications on a device.
2	+=======================
3	+
4	+Blackbox tool to bypass SSL certificate pinning for most applications 
5	+running on a device.
4	6	 
5	7	 Description
6		--------
8	+-----------
9	+
7	10	 This tool leverages Cydia Substrate to hook various methods 
8	11	 in order to bypass certificate pinning by accepting
9	12	 any SSL certificate.
10	13	 
11	14	 Usage
12		--------
13		-* Install Android-SSL-TrustKiller.apk on a device where Cydia Substrate is installed with:
15	+-----
16	+
17	+* Ensure that Cydia Substrate has been deployed on your test device. The installer requires a rooted device and can be found on the Google Play store at https://play.google.com/store/apps/details?id=com.saurik.substrate&hl=en 
18	+* Download the pre-compiled APK available at https://github.com/iSECPartners/Android-SSL-TrustKiller/releases
19	+* Install the APK package on the device:
14	20	 
15	21	         adb install Android-SSL-TrustKiller.apk
16	22	 
17		-* Cydia Substrate can be found on Google Play 
18		-(https://play.google.com/store/apps/details?id=com.saurik.substrate&hl=en) 
19		-and requires a rooted device.
20		-* Add the CA of your proxy tool to the device.
23	+* Add the CA certificate of your proxy tool to the device's trust store.
21	24	 
22	25	 Notes
23		--------
24		-* Use on test device only as it bypasses cert validation for any app doing certificate pinning on the device
26	+-----
27	+
28	+Use on test devices only as it disables certificate validation for any app doing certificate pinning on the device.
25	29	 
26	30	 License
27	31	 -------
...	...	@@ -31,4 +35,4 @@ See ./LICENSE.
31	35	 Authors
32	36	 -------
33	37	 
34		-* Marc Blanchou
38	+Marc Blanchou
