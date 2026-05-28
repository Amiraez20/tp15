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

## Génération du PDF
Le rapport a été pensé pour être compilé avec LaTeX.

Commande :
```bash
python /home/oai/skills/pdfs/scripts/latex_to_pdf.py rapport_tp_ssl_pinning.tex -o rapport_tp_ssl_pinning.pdf --engine pdflatex
```

## Vérifications conseillées
- contrôler que le PDF s’ouvre correctement ;
- vérifier que les figures ne sont pas coupées ;
- confirmer que la table des matières et les légendes s’affichent correctement.

## Remarques
- Le TP doit être utilisé uniquement dans un cadre légal et autorisé.
- Le nom affiché dans le rapport est **Ezbiri Amira**.
