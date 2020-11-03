# Android 7.0+ Charles https proxy unknown

 - https://www.charlesproxy.com/documentation/using-charles/ssl-certificates/
 - https://developer.android.google.cn/training/articles/security-config.html

# Rooted Phone Fix

```
#  openssl x509 -subject_hash_old -in /sdcard/Download/charles-proxy-ssl-proxying-certificate.pem.crt

3a76fabb
-----BEGIN CERTIFICATE-----
...
-----END CERTIFICATE-----

# mount -o rw,remount /
# cp /sdcard/Download/charles-proxy-ssl-proxying-certificate.pem.crt /system/etc/security/cacerts/3a76fabb  .0
#

```
