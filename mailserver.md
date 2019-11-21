---
title: mailserver
description: 
published: true
date: 2019-11-21T14:02:33.799Z
tags: mailserver
---

A       mail            78.47.69.68

CNAME   autoconfig      mail.wtmh.dev
CNAME   autodiscover    mail.wtmh.dev

MX      wtmh.dev        mail.wtmh.dev

SRV     wtmh.dev        0 1 443 mail.wtmh.dev
SRV     wtmh.dev        0 1 993 mail.wtmh.dev
SRV     wtmh.dev        0 1 143 mail.wtmh.dev
SRV     wtmh.dev        0 1 995 mail.wtmh.dev
SRV     wtmh.dev        0 1 110 mail.wtmh.dev
SRV     wtmh.dev        0 1 465 mail.wtmh.dev
SRV     wtmh.dev        0 1 587 mail.wtmh.dev

TXT     _caldavs._tcp   path=/SOGo/dav/
TXT     _carddavs._tcp  path=/SOGo/dav/
TXT     _dmarc          v=DMARC1; p=reject; rua=mailto:authfail-reports@wtmh.dev
TXT     mail._domainkey v=DKIM1; k=rsa; p=MIICIjANBgkqhkiG9w0BAQEFAAOCAg8AMIICCgKCAgEAxhXmXahtZBdPGJ/sNTZOFdcdC5LGE3U66WgyUB0VWbIiHUbrxgIl1GcVCTANzoXImEic2xIAjqlHzoBhFJbWExmg8C2ErxfgH+/sTW4nZ5jsXQZIKCtef5I+Te2EJZ5rw9ldMWTLuX94Fb7iwaS98vZcKJfmB3sVu7jlWOYiFDALBBcAVRTFjaFDXP1GQxzGrYwMmPf3atL9iX4JO94RRPMi7uMb0jr7oOxynPyEXj3hx6BF9H/NW8BsPpRh5yyKRakBRtG3RSeeMce6ImBnJn3c1z9QO04FuiZjqoNKtTsx214+SMhiHv4sVow/0PXt3SZI/KfzuliuyrrVDPxsrkd/4huZL6f0xvVcJPkKZZ+2nyiQvBE/pKQvFG/UCqJ0kwmzIdnm1udWMgZWD5qNXa+lMJrHJ09Yd4vUapH3SpvY6qM0WT8XkiXpt2Sd2AQCQJnUU+UZYvnrKjOvimqchAh4cO0nGxTKwr+KcxCYnM27neorKaGKAZXGgayGoPLsILie3UdfAJ7FN9R9tVnV65RQYgBkugKa2A9l96VO7bCeTH3AlbBrr7dMoiOdVtzXvdKKC5XBsq5G7JUXO+RzQeZ/tuKTiV1b9gm4beW+LgCEuMeqZSakp5PpG7kwLdy4NFBqO8/1iWqSspYnC9BZ/HtGfpZFCxj0WhIJ5W/jES0CAwEAAQ==
TXT     wtmh.dev        v=spf1 mx ip4:116.203.146.147 ~all

-----------------------------


A       eml            78.47.69.68

CNAME   autoconfig      eml.gos.ooo
CNAME   autodiscover    eml.gos.ooo

MX      gos.ooo         eml.gos.ooo

SRV     _autodiscover   gos.ooo        0 1 443 eml.gos.ooo
SRV     _autodiscover   gos.ooo        0 1 993 eml.gos.ooo
SRV     _autodiscover   gos.ooo        0 1 143 eml.gos.ooo
SRV     _autodiscover   gos.ooo        0 1 995 eml.gos.ooo
SRV     _autodiscover   gos.ooo        0 1 110 eml.gos.ooo
SRV     _autodiscover   gos.ooo        0 1 465 eml.gos.ooo
SRV     _autodiscover   gos.ooo        0 1 587 eml.gos.ooo

TXT     _caldavs._tcp   path=/SOGo/dav/
TXT     _carddavs._tcp  path=/SOGo/dav/
TXT     _dmarc          v=DMARC1; p=reject; rua=mailto:authfail-reports@gos.ooo
TXT     mail._domainkey v=DKIM1; k=rsa; p=MIGfMA0GCSqGSIb3DQEBAQUAA4GNADCBiQKBgQDKQr/5GLZoGc6yStL+JL4zryOrDcxlBudjTvp1R4S67+BMPEwh2xCwEBKRhxVF0sSaUy58QLBjruKXq9jyk1BFP1fhuhGTcT1+Wa+Ocx9zqnznqlj2FtG7g7fZ91SD45NSlRoIL90Pk769j3kxgpadFcOtCenwXbM8F0B36SlatQIDAQAB
TXT     gos.ooo        v=spf1 mx ip4:78.47.69.68 ~all  // v=spf1 mx ~all

