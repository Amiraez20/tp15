# TP - Bypass SSL pinning avec Frida

**Rédigé par : Ezbiri Amira**

## Objectif
Mettre en place un laboratoire Android pour observer du trafic HTTPS via un proxy TLS, puis neutraliser les mécanismes de SSL pinning avec Frida.

## Contenu du TP
- installation et vérification de Frida côté PC ;
- démarrage de `frida-server` sur Android ;
- configuration d’un proxy TLS (Burp Suite ou mitmproxy) ;
- installation du certificat CA du proxy sur l’appareil ;
- hooks Java Frida sur `TrustManager`, Conscrypt, OkHttp et WebView ;
- diagnostic d’un pinning natif éventuel ;
- validation via capture du trafic HTTPS déchiffré.


## Captures incluses
- `burp_proxy_listener.png`
- `adb_proxy_settings.png`
- `burp_ca_certificate.png`
- `frida_ps_uai.png`
- `frida_hook_logs.png`
- `frida_hook_logs_2.png`
- `burp_traffic_capture.png`



**Ezbiri Amira**.
